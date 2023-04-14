# Comparing `tmp/nucleus_client-0.8.0.tar.gz` & `tmp/nucleus_client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nucleus_client-0.8.0.tar", last modified: Thu May  7 15:15:59 2020, max compression
+gzip compressed data, was "dist/nucleus_client-0.9.0.tar", last modified: Mon Mar  1 18:17:17 2021, max compression
```

## Comparing `nucleus_client-0.8.0.tar` & `nucleus_client-0.9.0.tar`

### file list

```diff
@@ -1,446 +1,490 @@
-drwxr-xr-x   0 cbuechter (1821784841) 2054214907        0 2020-05-07 15:15:59.000000 nucleus_client-0.8.0/
--rw-r--r--   0 cbuechter (1821784841) 2054214907      370 2020-05-07 15:15:59.000000 nucleus_client-0.8.0/PKG-INFO
--rw-r--r--   0 cbuechter (1821784841) 2054214907    33320 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/README.md
-drwxr-xr-x   0 cbuechter (1821784841) 2054214907        0 2020-05-07 15:15:59.000000 nucleus_client-0.8.0/nucleus_client/
--rw-r--r--   0 cbuechter (1821784841) 2054214907    15364 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/nucleus_client/__init__.py
-drwxr-xr-x   0 cbuechter (1821784841) 2054214907        0 2020-05-07 15:15:59.000000 nucleus_client-0.8.0/nucleus_client/api/
--rw-r--r--   0 cbuechter (1821784841) 2054214907      141 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/nucleus_client/api/__init__.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907   560561 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/nucleus_client/api/default_api.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    24922 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/nucleus_client/api_client.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     8213 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/nucleus_client/configuration.py
-drwxr-xr-x   0 cbuechter (1821784841) 2054214907        0 2020-05-07 15:15:59.000000 nucleus_client-0.8.0/nucleus_client/models/
--rw-r--r--   0 cbuechter (1821784841) 2054214907    15134 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/nucleus_client/models/__init__.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     8687 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/activity.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4571 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/add_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    13975 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/aggregation_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    13395 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/aggregation_parameterized_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    11893 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/aggregation_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    21340 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/aggregation_task_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     7717 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/api_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4262 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/array_explode_many_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5520 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/array_explode_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5792 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/array_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    17679 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/base_page.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    12732 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/base_templated_page.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     8212 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/base_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3016 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/batch_receipt.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9720 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/binomial_logistic_regression_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4908 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/block.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5065 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/block_full.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4930 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/block_type.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4438 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/boolean_bucket_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4765 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/boolean_bucket_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4652 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/boolean_cast_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3986 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/boolean_constant_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5023 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/boolean_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4403 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/boolean_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    15085 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/client.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     7574 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/client_features.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5268 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/client_package.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5234 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/client_settings.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3606 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/client_settings_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    14251 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/client_sso.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9499 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/client_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3966 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/coalesce_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3993 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/collection_size_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3883 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/column_mapping.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3163 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/count_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     8564 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/create_custom_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4649 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/cumulative_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3736 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/cumulative_metric_order_by.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4805 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/cumulative_sum_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3885 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_selector.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    12828 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3809 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_base.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4476 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_dimension.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5591 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5285 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_filter_value.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3525 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_interval.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3768 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_lookup.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6735 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     8485 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_metric_calc.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4523 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_metric_order_by.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3883 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_mode.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3816 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_period_to_date.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4461 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_sort.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3865 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/data_view_unique_limit.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    10315 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/dataset.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3554 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/dataset_error.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4007 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/dataset_metadata.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6363 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/dataset_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3712 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/date_dimension.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     8430 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/date_time_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4450 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/date_time_filter_component.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4663 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_constant_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3282 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_current_date_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3317 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_current_timestamp_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5776 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_diff_from_column_date_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4919 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_diff_from_now_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5776 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_diff_from_static_date_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6120 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_diff_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4739 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_format_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6757 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_offset_column_value_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6616 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_offset_static_value_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6960 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_offset_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     7049 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_range_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4781 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_select_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    14531 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/datetime_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3747 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/dimension.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4742 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/divide_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    13339 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/download.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3565 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/download_error.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    13491 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/download_v1.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    13446 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/download_v2.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3069 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/drop_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4681 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/druid_write_config.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     8081 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/entity_batch.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5821 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/entity_batch_health.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9550 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3731 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/filter_map.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4612 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/filter_preset.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4695 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/geo_data.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6756 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/goal.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3831 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/goal_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6841 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/individual_data_selector.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9882 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/integration.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4757 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/integration_batch_history_receipt.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6729 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/integration_dataset.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3799 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/integration_sync_history_receipt.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5044 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/integration_type.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4409 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/integration_type_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6051 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/nucleus_client/models/integration_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     7212 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/job.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6671 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/job_overview.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4536 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/join.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4736 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/join_relationship.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3765 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/loader_settings.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4296 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/map_explode_many_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5558 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/map_explode_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5734 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/map_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4646 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/multiply_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     2981 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/new_user_token.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3030 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/non_null_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9548 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/normal_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    10157 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/notify_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5920 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_binary_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5405 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_binary_value_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4426 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_bucket_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4750 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_bucket_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4637 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_cast_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3978 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_constant_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4709 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_default_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5007 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    20633 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3960 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/number_unary_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3025 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/or_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    19212 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/page.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4614 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/page_filter_preferences.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    19608 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/page_full.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9476 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/page_preferences.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6841 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/page_preferences_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     2966 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/page_publications.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6413 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/page_template.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5329 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/page_template_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4556 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/page_view.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6603 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/partner_batch.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     8125 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/partner_post_data.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3992 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/password_change_request.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3114 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/password_reset_change.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3058 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/password_reset_request.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5862 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/percentile_lookup_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     7147 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/post_data.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5435 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/refresh_interval.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4482 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/refresh_schedule.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3650 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/refresh_state.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3905 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/rename_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     7611 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/role.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5794 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/role_permission.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3593 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/role_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    11161 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/sarimax_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9223 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/sarimax_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     2937 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/sarimax_task_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5756 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/schema.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4908 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/schema_field.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     2967 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/schema_field_metadata.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3557 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/schema_schema.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     2321 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/settings_spec.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4468 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/snapshot_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4517 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/sort.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4420 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_bucket_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4744 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_bucket_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4667 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_casing_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3972 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_constant_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5498 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_default_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4760 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_distance_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4967 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_extract_url_component_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5001 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4748 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_format_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5815 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_lookup_state_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4814 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_regexp_extract_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5601 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_regexp_replace_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3982 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_soundex_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5387 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_split_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5647 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_substring_index_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5974 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_substring_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4769 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_to_datetime_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3960 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_to_num_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    15228 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5346 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/string_trim_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3691 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/sub_nav.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4646 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/subtract_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    14978 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/templated_page.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     7342 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/term.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    11253 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_aggregation_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9219 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_aggregation_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4817 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_difference_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4817 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_growth_rate_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5691 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    10997 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_metric_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9003 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_metric_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3578 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_mode.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    17922 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_netforum_stats_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6720 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/time_step_renewal_rate_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    11902 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/top_n_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9932 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/top_n_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3058 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/top_n_task_partition.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3788 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/top_n_task_sort.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    10391 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3016 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/unary_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3777 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/unique_limit.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3584 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/update_api_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     5313 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/update_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3664 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/user_activation.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4472 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/user_role.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     6858 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/user_token.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     7396 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/view.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     3521 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/view_error.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     9002 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/virtual_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    12597 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/widget.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    12914 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/widget_full.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4949 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/widget_type.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4498 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/write_config.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4961 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/write_config_druid_override.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     4545 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/nucleus_client/models/write_config_override.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    13176 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/nucleus_client/rest.py
-drwxr-xr-x   0 cbuechter (1821784841) 2054214907        0 2020-05-07 15:15:59.000000 nucleus_client-0.8.0/nucleus_client.egg-info/
--rw-r--r--   0 cbuechter (1821784841) 2054214907      370 2020-05-07 15:15:58.000000 nucleus_client-0.8.0/nucleus_client.egg-info/PKG-INFO
--rw-r--r--   0 cbuechter (1821784841) 2054214907    16455 2020-05-07 15:15:58.000000 nucleus_client-0.8.0/nucleus_client.egg-info/SOURCES.txt
--rw-r--r--   0 cbuechter (1821784841) 2054214907        1 2020-05-07 15:15:58.000000 nucleus_client-0.8.0/nucleus_client.egg-info/dependency_links.txt
--rw-r--r--   0 cbuechter (1821784841) 2054214907       48 2020-05-07 15:15:58.000000 nucleus_client-0.8.0/nucleus_client.egg-info/requires.txt
--rw-r--r--   0 cbuechter (1821784841) 2054214907       20 2020-05-07 15:15:58.000000 nucleus_client-0.8.0/nucleus_client.egg-info/top_level.txt
--rw-r--r--   0 cbuechter (1821784841) 2054214907       38 2020-05-07 15:15:59.000000 nucleus_client-0.8.0/setup.cfg
--rw-r--r--   0 cbuechter (1821784841) 2054214907      991 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/setup.py
-drwxr-xr-x   0 cbuechter (1821784841) 2054214907        0 2020-05-07 15:15:59.000000 nucleus_client-0.8.0/test/
--rw-r--r--   0 cbuechter (1821784841) 2054214907        0 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/test/__init__.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      860 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_activity.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      870 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_add_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      976 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_aggregation_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1024 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_aggregation_parameterized_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      918 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_aggregation_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_aggregation_task_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      854 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_api_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1002 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_array_explode_many_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_array_explode_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      910 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_array_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      862 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_base_page.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      936 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_base_templated_page.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      862 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_base_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_batch_receipt.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1042 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_binomial_logistic_regression_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      836 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_block.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      870 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_block_full.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      870 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_block_type.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      952 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_boolean_bucket_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      976 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_boolean_bucket_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      960 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_boolean_cast_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      992 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_boolean_constant_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      902 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_boolean_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      926 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_boolean_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      844 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_client.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      910 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_client_features.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      902 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_client_package.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      910 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_client_settings.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      960 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_client_settings_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      870 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_client_sso.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_client_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      934 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_coalesce_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      984 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_collection_size_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      902 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_column_mapping.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      886 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_count_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      986 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_create_custom_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      926 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_cumulative_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      986 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_cumulative_metric_order_by.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      952 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_cumulative_sum_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_selector.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      862 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      896 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_base.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      936 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_dimension.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      912 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      954 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_filter_value.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      928 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_interval.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      912 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_lookup.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      912 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      946 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_metric_calc.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      972 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_metric_order_by.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      896 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_mode.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      964 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_period_to_date.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      896 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_sort.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      954 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_data_view_unique_limit.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      852 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_dataset.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_dataset_error.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      918 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_dataset_metadata.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      902 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_dataset_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      902 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_date_dimension.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      912 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_date_time_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      986 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_date_time_filter_component.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1000 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_constant_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1026 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_current_date_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1066 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_current_timestamp_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1086 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_diff_from_column_date_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1028 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_diff_from_now_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1086 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_diff_from_static_date_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_diff_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      984 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_format_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1076 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_offset_column_value_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1076 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_offset_static_value_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      984 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_offset_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      976 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_range_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      984 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_select_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      934 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_datetime_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907    23477 2020-05-07 15:14:02.000000 nucleus_client-0.8.0/test/test_default_api.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      868 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_dimension.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_divide_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      860 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_download.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      902 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_download_error.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      878 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_download_v1.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      878 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_download_v2.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      902 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_drop_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      928 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_druid_write_config.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      886 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_entity_batch.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      936 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_entity_batch_health.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      844 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      870 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_filter_map.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_filter_preset.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      854 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_geo_data.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      828 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_goal.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      878 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_goal_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      976 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_individual_data_selector.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      884 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_integration.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1042 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_integration_batch_history_receipt.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      942 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_integration_dataset.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1034 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_integration_sync_history_receipt.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      918 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_integration_type.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:00.000000 nucleus_client-0.8.0/test/test_integration_type_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      934 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_integration_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      820 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_job.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      886 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_job_overview.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      828 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_join.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      926 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_join_relationship.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      910 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_loader_settings.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      986 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_map_explode_many_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      952 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_map_explode_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_map_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      910 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_multiply_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      896 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_new_user_token.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      904 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_non_null_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      878 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_normal_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      878 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_notify_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_binary_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1010 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_binary_value_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      944 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_bucket_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_bucket_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      952 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_cast_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      984 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_constant_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      976 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_default_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      918 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      960 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_number_unary_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      862 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_or_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      828 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_page.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_page_filter_preferences.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      862 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_page_full.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      918 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_page_preferences.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_page_preferences_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      926 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_page_publications.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_page_template.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      944 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_page_template_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      862 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_page_view.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_partner_batch.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      920 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_partner_post_data.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_password_change_request.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      952 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_password_reset_change.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      960 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_password_reset_request.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      976 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_percentile_lookup_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      862 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_post_data.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      918 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_refresh_interval.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      918 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_refresh_schedule.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_refresh_state.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      918 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_rename_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      828 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_role.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      910 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_role_permission.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      878 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_role_update.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      944 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_sarimax_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      886 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_sarimax_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      936 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_sarimax_task_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      844 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_schema.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      886 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_schema_field.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      952 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_schema_field_metadata.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_schema_schema.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_settings_spec.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      952 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_snapshot_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      828 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_sort.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      944 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_bucket_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_bucket_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_casing_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      984 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_constant_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      976 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_default_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      984 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_distance_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1076 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_extract_url_component_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      894 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_filter.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      968 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_format_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1010 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_lookup_state_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1026 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_regexp_extract_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1026 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_regexp_replace_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      976 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_soundex_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      960 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_split_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1034 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_substring_index_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      992 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_substring_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1002 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_to_datetime_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      962 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_to_num_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      918 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      952 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_string_trim_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      846 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_sub_nav.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      910 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_subtract_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      902 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_templated_page.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      828 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_term.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1044 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_aggregation_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      986 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_aggregation_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      994 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_difference_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      996 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_growth_rate_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      912 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1004 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_metric_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      946 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_metric_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      896 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_mode.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1020 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_netforum_stats_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907     1004 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_time_step_renewal_rate_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      922 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_top_n_dataset_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      864 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_top_n_task.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      938 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_top_n_task_partition.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      898 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_top_n_task_sort.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      868 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_transform.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      886 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_unary_metric.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      886 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_unique_limit.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      904 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_update_api_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      878 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_update_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      910 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_user_activation.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      862 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_user_role.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      870 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_user_token.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      828 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_view.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      870 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_view_error.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      886 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_virtual_user.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      844 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_widget.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      878 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_widget_full.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      878 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_widget_type.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      886 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_write_config.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      994 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_write_config_druid_override.py
--rw-r--r--   0 cbuechter (1821784841) 2054214907      952 2020-05-07 15:14:01.000000 nucleus_client-0.8.0/test/test_write_config_override.py
+drwxr-xr-x   0 cbuechter   (501) staff       (20)        0 2021-03-01 18:17:17.000000 nucleus_client-0.9.0/
+-rw-r--r--   0 cbuechter   (501) staff       (20)      370 2021-03-01 18:17:17.000000 nucleus_client-0.9.0/PKG-INFO
+-rw-r--r--   0 cbuechter   (501) staff       (20)    36624 2021-03-01 18:10:34.000000 nucleus_client-0.9.0/README.md
+drwxr-xr-x   0 cbuechter   (501) staff       (20)        0 2021-03-01 18:17:16.000000 nucleus_client-0.9.0/nucleus_client/
+-rw-r--r--   0 cbuechter   (501) staff       (20)    16738 2021-03-01 18:10:34.000000 nucleus_client-0.9.0/nucleus_client/__init__.py
+drwxr-xr-x   0 cbuechter   (501) staff       (20)        0 2021-03-01 18:17:16.000000 nucleus_client-0.9.0/nucleus_client/api/
+-rw-r--r--   0 cbuechter   (501) staff       (20)      141 2021-03-01 18:10:34.000000 nucleus_client-0.9.0/nucleus_client/api/__init__.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)   627590 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/api/default_api.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    24922 2021-03-01 18:10:34.000000 nucleus_client-0.9.0/nucleus_client/api_client.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     8213 2021-03-01 18:10:34.000000 nucleus_client-0.9.0/nucleus_client/configuration.py
+drwxr-xr-x   0 cbuechter   (501) staff       (20)        0 2021-03-01 18:17:16.000000 nucleus_client-0.9.0/nucleus_client/models/
+-rw-r--r--   0 cbuechter   (501) staff       (20)    16508 2021-03-01 18:10:34.000000 nucleus_client-0.9.0/nucleus_client/models/__init__.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     8687 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/activity.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4571 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/add_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    13975 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/aggregation_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    13395 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/aggregation_parameterized_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    11893 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/aggregation_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    22112 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/aggregation_task_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7717 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/api_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4262 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/array_explode_many_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5520 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/array_explode_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5792 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/array_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    19235 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/base_page.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    12732 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/base_templated_page.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     8212 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/base_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3016 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/batch_receipt.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9720 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/binomial_logistic_regression_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4908 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/block.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5065 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/block_full.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4930 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/block_type.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4438 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/boolean_bucket_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4765 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/boolean_bucket_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4652 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/boolean_cast_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3986 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/boolean_constant_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5023 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/boolean_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4403 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/boolean_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    15085 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/client.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     8362 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/client_features.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5268 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/client_package.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7564 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/client_settings.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3606 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/client_settings_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    14251 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/client_sso.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9499 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/client_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3966 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/coalesce_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3993 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/collection_size_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3883 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/column_mapping.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3163 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/count_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     8564 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/create_custom_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4649 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/cumulative_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3736 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/cumulative_metric_order_by.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4805 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/cumulative_sum_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3885 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_selector.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    13976 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3809 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_base.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4476 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_dimension.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5591 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5285 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_filter_value.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3525 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_interval.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3768 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_lookup.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7600 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     8485 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_metric_calc.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4523 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_metric_order_by.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3883 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_mode.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3816 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_period_to_date.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4461 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_sort.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3865 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/data_view_unique_limit.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    10972 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/dataset.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3554 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/dataset_error.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4007 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/dataset_metadata.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6363 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/dataset_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3712 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/date_dimension.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     8430 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/date_time_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4450 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/date_time_filter_component.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4663 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_constant_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3282 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_current_date_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3317 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_current_timestamp_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5776 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_diff_from_column_date_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4919 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_diff_from_now_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5776 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_diff_from_static_date_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6120 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_diff_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4739 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_format_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6757 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_offset_column_value_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6616 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_offset_static_value_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6960 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_offset_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7049 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_range_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4781 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_select_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    14531 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/datetime_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3747 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/dimension.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4742 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/divide_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    13339 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/download.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3565 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/download_error.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    13491 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/download_v1.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    13446 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/download_v2.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3069 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/drop_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4681 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/druid_write_config.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4467 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/email_address.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6551 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/email_report_config.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     8081 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/entity_batch.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5821 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/entity_batch_health.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9550 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3731 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/filter_map.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4612 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/filter_preset.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4695 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/geo_data.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6756 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/goal.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3831 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/goal_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6841 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/individual_data_selector.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9882 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/integration.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4757 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/integration_batch_history_receipt.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6729 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/integration_dataset.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3799 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/integration_sync_history_receipt.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5044 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/integration_type.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4409 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/nucleus_client/models/integration_type_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6051 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/integration_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7212 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/job.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6671 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/job_overview.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4536 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/join.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4736 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/join_relationship.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4432 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/link.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3765 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/loader_settings.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4296 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/map_explode_many_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5558 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/map_explode_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5734 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/map_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4646 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/multiply_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     2981 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/new_user_token.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3030 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/non_null_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9548 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/normal_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    10157 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/notify_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5920 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_binary_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5405 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_binary_value_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4426 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_bucket_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4750 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_bucket_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4637 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_cast_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3978 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_constant_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4709 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_default_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5007 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    20633 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3960 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/number_unary_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3903 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/options.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3025 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/or_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    20736 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/page.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4614 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/page_filter_preferences.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    21164 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/page_full.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9476 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/page_preferences.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6841 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/page_preferences_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     2966 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/page_publications.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6413 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/page_template.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5329 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/page_template_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4556 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/page_view.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6603 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/partner_batch.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     8125 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/partner_post_data.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3992 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/password_change_request.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3114 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/password_reset_change.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3058 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/password_reset_request.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5679 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/percentage_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5862 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/percentile_lookup_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7147 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/post_data.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5020 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/prolearn_base_object.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5827 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/prolearn_callback.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7365 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/prolearn_course.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4021 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/prolearn_credit.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7802 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/prolearn_credit_type.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    18117 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/prolearn_registration.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    15760 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/prolearn_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5435 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/refresh_interval.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5187 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/refresh_schedule.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3650 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/refresh_state.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3905 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/rename_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3916 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/rename_transform2.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7654 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/report.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5761 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/report_add.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9460 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/report_config.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7344 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/report_config_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3543 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/report_error.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4874 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/report_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7611 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/role.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5794 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/role_permission.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3593 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/role_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    11161 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/sarimax_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9223 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/sarimax_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     2937 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/sarimax_task_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5756 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/schema.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4908 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/schema_field.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     2967 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/schema_field_metadata.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3557 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/schema_schema.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     2321 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/settings_spec.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4468 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/snapshot_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4517 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/sort.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4420 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_bucket_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4744 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_bucket_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4667 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_casing_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3972 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_constant_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5498 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_default_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4760 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_distance_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4967 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_extract_url_component_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5001 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4748 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_format_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5815 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_lookup_state_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4814 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_regexp_extract_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5601 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_regexp_replace_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3982 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_soundex_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5387 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_split_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5647 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_substring_index_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5974 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_substring_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4769 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_to_datetime_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3960 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_to_num_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    15228 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5346 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/string_trim_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3691 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/sub_nav.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4646 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/subtract_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    14978 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/templated_page.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7342 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/term.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    11253 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_aggregation_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9219 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_aggregation_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4817 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_difference_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4817 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_growth_rate_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5691 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    10997 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_metric_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9003 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_metric_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3578 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_mode.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    17922 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_netforum_stats_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6720 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/time_step_renewal_rate_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    11902 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/top_n_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9932 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/top_n_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3058 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/top_n_task_partition.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3788 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/top_n_task_sort.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    11055 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3016 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/unary_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3777 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/unique_limit.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3584 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/update_api_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5313 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/update_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    14199 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/upload.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6994 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/upload_field.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3664 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/user_activation.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4472 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/user_role.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     6858 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/user_token.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     7396 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/view.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3521 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/view_error.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     9002 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/virtual_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    13173 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/widget.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    13506 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/widget_full.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4949 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/widget_type.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     3881 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/write_backup.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     5851 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/write_config.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4961 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/write_config_druid_override.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     4545 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/nucleus_client/models/write_config_override.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    13176 2021-03-01 18:10:34.000000 nucleus_client-0.9.0/nucleus_client/rest.py
+drwxr-xr-x   0 cbuechter   (501) staff       (20)        0 2021-03-01 18:17:16.000000 nucleus_client-0.9.0/nucleus_client.egg-info/
+-rw-r--r--   0 cbuechter   (501) staff       (20)      370 2021-03-01 18:17:16.000000 nucleus_client-0.9.0/nucleus_client.egg-info/PKG-INFO
+-rw-r--r--   0 cbuechter   (501) staff       (20)    17939 2021-03-01 18:17:16.000000 nucleus_client-0.9.0/nucleus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 cbuechter   (501) staff       (20)        1 2021-03-01 18:17:16.000000 nucleus_client-0.9.0/nucleus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 cbuechter   (501) staff       (20)       48 2021-03-01 18:17:16.000000 nucleus_client-0.9.0/nucleus_client.egg-info/requires.txt
+-rw-r--r--   0 cbuechter   (501) staff       (20)       20 2021-03-01 18:17:16.000000 nucleus_client-0.9.0/nucleus_client.egg-info/top_level.txt
+-rw-r--r--   0 cbuechter   (501) staff       (20)       38 2021-03-01 18:17:17.000000 nucleus_client-0.9.0/setup.cfg
+-rw-r--r--   0 cbuechter   (501) staff       (20)      991 2021-03-01 18:10:34.000000 nucleus_client-0.9.0/setup.py
+drwxr-xr-x   0 cbuechter   (501) staff       (20)        0 2021-03-01 18:17:17.000000 nucleus_client-0.9.0/test/
+-rw-r--r--   0 cbuechter   (501) staff       (20)        0 2021-03-01 18:10:34.000000 nucleus_client-0.9.0/test/__init__.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      860 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_activity.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      870 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_add_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      976 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_aggregation_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1024 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_aggregation_parameterized_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      918 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_aggregation_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_aggregation_task_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      854 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_api_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1002 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_array_explode_many_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_array_explode_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_array_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      862 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_base_page.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      936 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_base_templated_page.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      862 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_base_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_batch_receipt.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1042 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_binomial_logistic_regression_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      836 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_block.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      870 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_block_full.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      870 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_block_type.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      952 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_boolean_bucket_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      976 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_boolean_bucket_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      960 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_boolean_cast_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      992 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_boolean_constant_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      902 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_boolean_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      926 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_boolean_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      844 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_client.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_client_features.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      902 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_client_package.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_client_settings.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      960 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_client_settings_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      870 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_client_sso.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_client_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      934 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_coalesce_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      984 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_collection_size_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      902 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_column_mapping.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_count_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      986 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_create_custom_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      926 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_cumulative_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      986 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_cumulative_metric_order_by.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      952 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_cumulative_sum_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_selector.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      862 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      896 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_base.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      936 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_dimension.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      912 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      954 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_filter_value.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      928 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_interval.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      912 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_lookup.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      912 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      946 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_metric_calc.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      972 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_metric_order_by.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      896 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_mode.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      964 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_period_to_date.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      896 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_sort.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      954 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_data_view_unique_limit.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      852 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_dataset.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_dataset_error.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      918 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_dataset_metadata.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      902 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_dataset_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      902 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_date_dimension.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      912 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_date_time_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      986 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_date_time_filter_component.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1000 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_constant_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1026 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_current_date_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1066 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_current_timestamp_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1086 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_diff_from_column_date_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1028 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_diff_from_now_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1086 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_diff_from_static_date_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_diff_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      984 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_format_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1076 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_offset_column_value_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1076 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_offset_static_value_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      984 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_offset_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      976 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_range_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      984 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_select_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      934 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_datetime_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)    26133 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_default_api.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      868 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_dimension.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_divide_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      860 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_download.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      902 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_download_error.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      878 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_download_v1.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      878 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_download_v2.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      902 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_drop_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      928 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_druid_write_config.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_email_address.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      936 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_email_report_config.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_entity_batch.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      936 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_entity_batch_health.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      844 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      870 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_filter_map.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_filter_preset.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      854 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_geo_data.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      828 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_goal.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      878 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_goal_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      976 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_individual_data_selector.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      884 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_integration.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1042 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_integration_batch_history_receipt.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      942 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_integration_dataset.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1034 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_integration_sync_history_receipt.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      918 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_integration_type.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:32.000000 nucleus_client-0.9.0/test/test_integration_type_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      934 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_integration_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      820 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_job.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_job_overview.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      828 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_join.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      926 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_join_relationship.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      828 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_link.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_loader_settings.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      986 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_map_explode_many_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      952 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_map_explode_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_map_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_multiply_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      896 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_new_user_token.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      904 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_non_null_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      878 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_normal_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      878 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_notify_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_binary_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1010 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_binary_value_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      944 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_bucket_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_bucket_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      952 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_cast_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      984 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_constant_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      976 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_default_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      918 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      960 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_number_unary_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      852 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_options.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      862 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_or_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      828 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_page.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_page_filter_preferences.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      862 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_page_full.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      918 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_page_preferences.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_page_preferences_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      926 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_page_publications.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_page_template.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      944 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_page_template_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      862 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_page_view.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_partner_batch.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      920 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_partner_post_data.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_password_change_request.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      952 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_password_reset_change.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      960 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_password_reset_request.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      926 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_percentage_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      976 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_percentile_lookup_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      862 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_post_data.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      944 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_prolearn_base_object.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      926 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_prolearn_callback.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_prolearn_course.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_prolearn_credit.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      944 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_prolearn_credit_type.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      958 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_prolearn_registration.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_prolearn_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      918 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_refresh_interval.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      918 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_refresh_schedule.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_refresh_state.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      918 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_rename_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      926 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_rename_transform2.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      844 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_report.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      870 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_report_add.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_report_config.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      944 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_report_config_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_report_error.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_report_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      828 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_role.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_role_permission.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      878 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_role_update.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      944 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_sarimax_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_sarimax_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      936 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_sarimax_task_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      844 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_schema.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_schema_field.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      952 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_schema_field_metadata.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_schema_schema.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_settings_spec.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      952 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_snapshot_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      828 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_sort.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      944 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_bucket_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_bucket_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_casing_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      984 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_constant_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      976 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_default_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      984 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_distance_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1076 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_extract_url_component_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      894 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_filter.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      968 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_format_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1010 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_lookup_state_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1026 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_regexp_extract_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1026 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_regexp_replace_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      976 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_soundex_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      960 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_split_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1034 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_substring_index_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      992 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_substring_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1002 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_to_datetime_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      962 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_to_num_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      918 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      952 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_string_trim_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      846 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_sub_nav.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_subtract_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      902 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_templated_page.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      828 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_term.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1044 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_aggregation_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      986 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_aggregation_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      994 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_difference_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      996 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_growth_rate_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      912 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1004 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_metric_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      946 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_metric_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      896 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_mode.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1020 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_netforum_stats_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)     1004 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_time_step_renewal_rate_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      922 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_top_n_dataset_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      864 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_top_n_task.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      938 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_top_n_task_partition.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      898 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_top_n_task_sort.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      868 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_transform.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_unary_metric.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_unique_limit.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      904 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_update_api_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      878 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_update_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      844 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_upload.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_upload_field.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      910 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_user_activation.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      862 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_user_role.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      870 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_user_token.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      828 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_view.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      870 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_view_error.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_virtual_user.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      844 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_widget.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      878 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_widget_full.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      878 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_widget_type.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_write_backup.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      886 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_write_config.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      994 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_write_config_druid_override.py
+-rw-r--r--   0 cbuechter   (501) staff       (20)      952 2021-03-01 18:10:33.000000 nucleus_client-0.9.0/test/test_write_config_override.py
```

### Comparing `nucleus_client-0.8.0/README.md` & `nucleus_client-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # nucleus_client
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v1
-- Package version: 0.8.0
+- Package version: 0.9.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -91,23 +91,28 @@
 *DefaultApi* | [**add_download_request_0**](docs/DefaultApi.md#add_download_request_0) | **POST** /download-requests/v2 | Adds a new (pending) download request
 *DefaultApi* | [**add_entity_batch**](docs/DefaultApi.md#add_entity_batch) | **POST** /entity-batches | Adds a new entity batch, and queues a task to process it
 *DefaultApi* | [**add_full_page**](docs/DefaultApi.md#add_full_page) | **POST** /pages/full | Creates a page without removing blocks, widgets, or block_order attributes
 *DefaultApi* | [**add_geodata**](docs/DefaultApi.md#add_geodata) | **POST** /geodata | Adds a new geo mapping
 *DefaultApi* | [**add_goal**](docs/DefaultApi.md#add_goal) | **POST** /goals | Adds a new goal
 *DefaultApi* | [**add_higher_logic_activity**](docs/DefaultApi.md#add_higher_logic_activity) | **POST** /callbacks/higher-logic | Higher Logic callback
 *DefaultApi* | [**add_integration**](docs/DefaultApi.md#add_integration) | **POST** /integrations | Adds a new integration
+*DefaultApi* | [**add_integration_sync_request**](docs/DefaultApi.md#add_integration_sync_request) | **POST** /admin/integration-sync-requests/ | Run a sync integration      Responses:          204: The sync request was successfully queued
 *DefaultApi* | [**add_integration_type**](docs/DefaultApi.md#add_integration_type) | **POST** /integration-types | Add a new integration type
 *DefaultApi* | [**add_page**](docs/DefaultApi.md#add_page) | **POST** /pages | Creates a page from a page template
 *DefaultApi* | [**add_page_publication**](docs/DefaultApi.md#add_page_publication) | **POST** /page-publications/{page_id} | Updates page with publication information      Responses:          201: Page was updated with publication information
 *DefaultApi* | [**add_page_template**](docs/DefaultApi.md#add_page_template) | **POST** /page-templates | Add a new page template
 *DefaultApi* | [**add_partner_batch**](docs/DefaultApi.md#add_partner_batch) | **POST** /entity-batches/partner-batches | Adds a new partner batch, and queues a task to process it
 *DefaultApi* | [**add_password_reset_request**](docs/DefaultApi.md#add_password_reset_request) | **POST** /password-reset-requests | Creates a new request to reset a user&#39;s password
+*DefaultApi* | [**add_prolearn_activity**](docs/DefaultApi.md#add_prolearn_activity) | **POST** /callbacks/prolearn | Prolearn callback
+*DefaultApi* | [**add_report**](docs/DefaultApi.md#add_report) | **POST** /reports | Add a new report
+*DefaultApi* | [**add_report_config**](docs/DefaultApi.md#add_report_config) | **POST** /report-configs | Add a new report_config
 *DefaultApi* | [**add_role**](docs/DefaultApi.md#add_role) | **POST** /roles | Adds a new role
 *DefaultApi* | [**add_role_permission**](docs/DefaultApi.md#add_role_permission) | **POST** /role-permissions | Adds a new permission to a role
 *DefaultApi* | [**add_term**](docs/DefaultApi.md#add_term) | **POST** /terms | Adds a new term
+*DefaultApi* | [**add_upload_request**](docs/DefaultApi.md#add_upload_request) | **POST** /upload-requests | Adds a new (pending) upload request
 *DefaultApi* | [**add_user**](docs/DefaultApi.md#add_user) | **POST** /users | Adds a new user
 *DefaultApi* | [**add_user_0**](docs/DefaultApi.md#add_user_0) | **POST** /users/admin-notify | Notifies administrator that user has been added or deleted
 *DefaultApi* | [**add_user_1**](docs/DefaultApi.md#add_user_1) | **POST** /users/{user_id&gt;/token} | Adds a new user token
 *DefaultApi* | [**add_user_role**](docs/DefaultApi.md#add_user_role) | **POST** /user-roles | Add a user to a role
 *DefaultApi* | [**add_view**](docs/DefaultApi.md#add_view) | **POST** /views | Adds a new view
 *DefaultApi* | [**add_widget_type**](docs/DefaultApi.md#add_widget_type) | **POST** /widget-types | Adds a new widget type
 *DefaultApi* | [**change_password**](docs/DefaultApi.md#change_password) | **POST** /password-changes/{user_id} | Changes a users password
@@ -121,14 +126,16 @@
 *DefaultApi* | [**delete_goal**](docs/DefaultApi.md#delete_goal) | **DELETE** /goals/{goal_id} | Deletes a goal by id
 *DefaultApi* | [**delete_integration**](docs/DefaultApi.md#delete_integration) | **DELETE** /integrations/{integration_id} | Deletes an integration by ID
 *DefaultApi* | [**delete_page**](docs/DefaultApi.md#delete_page) | **DELETE** /pages/{page_id} | Deletes a page by ID
 *DefaultApi* | [**delete_page_preference**](docs/DefaultApi.md#delete_page_preference) | **DELETE** /page-preferences/page-id-{page_id} | Deletes page preferences for the authenticated user
 *DefaultApi* | [**delete_page_publication**](docs/DefaultApi.md#delete_page_publication) | **DELETE** /page-publications/{page_id} | Deletes publication information for a page      Responses:          204: Page publication information was successfully deleted
 *DefaultApi* | [**delete_page_template**](docs/DefaultApi.md#delete_page_template) | **DELETE** /page-templates/{page_template_id} | Deletes a page template by ID
 *DefaultApi* | [**delete_page_template_by_slug**](docs/DefaultApi.md#delete_page_template_by_slug) | **DELETE** /page-templates/slug-{slug} | Deletes all page templates with the specified slug
+*DefaultApi* | [**delete_report**](docs/DefaultApi.md#delete_report) | **DELETE** /reports/{report_id} | Deletes a report by ID
+*DefaultApi* | [**delete_report_config**](docs/DefaultApi.md#delete_report_config) | **DELETE** /report-configs/{report_config_id} | Deletes a report_config by ID
 *DefaultApi* | [**delete_role**](docs/DefaultApi.md#delete_role) | **DELETE** /roles/{role_id} | Deletes a role by ID
 *DefaultApi* | [**delete_role_permission**](docs/DefaultApi.md#delete_role_permission) | **DELETE** /role-permissions/{role_permission_id} | Deletes a permission for a specific role by ID
 *DefaultApi* | [**delete_schema**](docs/DefaultApi.md#delete_schema) | **DELETE** /schemas/{client_id} | Deletes the schema associated with an activity      Responses:          204: Schema was successfully deleted
 *DefaultApi* | [**delete_term**](docs/DefaultApi.md#delete_term) | **DELETE** /terms/{term_id} | Deletes a term by ID
 *DefaultApi* | [**delete_user**](docs/DefaultApi.md#delete_user) | **DELETE** /users/{user_id} | Deletes an active user by ID
 *DefaultApi* | [**delete_user_0**](docs/DefaultApi.md#delete_user_0) | **DELETE** /users/{token_id} | Deletes an active user token by ID
 *DefaultApi* | [**delete_user_role**](docs/DefaultApi.md#delete_user_role) | **DELETE** /user-roles/{user_id} | Deletes a user from a role by user ID
@@ -153,20 +160,24 @@
 *DefaultApi* | [**get_jobs_overview**](docs/DefaultApi.md#get_jobs_overview) | **GET** /admin/jobs/overview | Gets an overview of data processing jobs
 *DefaultApi* | [**get_page**](docs/DefaultApi.md#get_page) | **GET** /pages/{page_id} | Gets a page by ID
 *DefaultApi* | [**get_page_by_slug**](docs/DefaultApi.md#get_page_by_slug) | **GET** /pages/slug-{slug} | Gets a page by slug
 *DefaultApi* | [**get_page_preference**](docs/DefaultApi.md#get_page_preference) | **GET** /page-preferences/page-id-{page_id} | Gets page preferences for the authenticated user
 *DefaultApi* | [**get_page_template**](docs/DefaultApi.md#get_page_template) | **GET** /page-templates/{page_template_id} | Gets a page template by ID
 *DefaultApi* | [**get_page_template_by_slug**](docs/DefaultApi.md#get_page_template_by_slug) | **GET** /page-templates/slug-{slug} | Gets a page template by slug
 *DefaultApi* | [**get_password_reset_by_key**](docs/DefaultApi.md#get_password_reset_by_key) | **GET** /password-resets/{reset_key} | Gets a user by the reset key associated with them
+*DefaultApi* | [**get_report**](docs/DefaultApi.md#get_report) | **GET** /reports/{report_id} | Get a report by ID
+*DefaultApi* | [**get_report_config**](docs/DefaultApi.md#get_report_config) | **GET** /report-configs/{report_config_id} | Get a report_config by ID
+*DefaultApi* | [**get_report_config_by_name**](docs/DefaultApi.md#get_report_config_by_name) | **GET** /report-configs/name-{report_config_name} | Get a report_config by name
 *DefaultApi* | [**get_role**](docs/DefaultApi.md#get_role) | **GET** /roles/{role_id} | Gets a role by ID
 *DefaultApi* | [**get_role_by_name**](docs/DefaultApi.md#get_role_by_name) | **GET** /roles/name-{role_name} | Gets a role by name
 *DefaultApi* | [**get_role_by_slug**](docs/DefaultApi.md#get_role_by_slug) | **GET** /roles/slug-{role_slug} | Gets a role slug
 *DefaultApi* | [**get_role_permission**](docs/DefaultApi.md#get_role_permission) | **GET** /role-permissions/{role_permission_id} | Gets a permission for a specific role by ID
 *DefaultApi* | [**get_schema**](docs/DefaultApi.md#get_schema) | **GET** /schemas/{schema_id} | Get a schema by ID
 *DefaultApi* | [**get_term_by_term**](docs/DefaultApi.md#get_term_by_term) | **GET** /terms/term-{term} | Gets a term by term
+*DefaultApi* | [**get_upload_request**](docs/DefaultApi.md#get_upload_request) | **GET** /upload-requests/{upload_id} | Gets an upload request by id
 *DefaultApi* | [**get_user**](docs/DefaultApi.md#get_user) | **GET** /users/{user_id} | Gets a user by ID
 *DefaultApi* | [**get_user_activation_by_key**](docs/DefaultApi.md#get_user_activation_by_key) | **GET** /user-activations/{activation_key} | Gets the user associated with an activation key
 *DefaultApi* | [**get_user_by_email**](docs/DefaultApi.md#get_user_by_email) | **GET** /users/email-{email} | Gets a user by email address
 *DefaultApi* | [**get_user_by_idtoken**](docs/DefaultApi.md#get_user_by_idtoken) | **GET** /users/{user_id&gt;/token} | List active tokens associated with a user
 *DefaultApi* | [**get_view**](docs/DefaultApi.md#get_view) | **GET** /views/{view_id} | Get a view by ID
 *DefaultApi* | [**get_view_by_keys**](docs/DefaultApi.md#get_view_by_keys) | **GET** /views/view-hashes-{hash_keys} | Get a list of views by hash key
 *DefaultApi* | [**get_widget_type**](docs/DefaultApi.md#get_widget_type) | **GET** /widget-types/{widget_type_id} | Get widget type by ID
@@ -187,18 +198,21 @@
 *DefaultApi* | [**list_integration_types**](docs/DefaultApi.md#list_integration_types) | **GET** /integration-types | List all integration types
 *DefaultApi* | [**list_integrations**](docs/DefaultApi.md#list_integrations) | **GET** /integrations | List all integrations associated with a client
 *DefaultApi* | [**list_maintenance**](docs/DefaultApi.md#list_maintenance) | **GET** /admin/maintenance/delete-datasource | Cleanup for a dataset      Responses:          202: Delete task was successfully queued
 *DefaultApi* | [**list_page_preferences**](docs/DefaultApi.md#list_page_preferences) | **GET** /page-preferences | List all page preferences associated with a client for the authenticated user
 *DefaultApi* | [**list_page_templates**](docs/DefaultApi.md#list_page_templates) | **GET** /page-templates | List all page templates
 *DefaultApi* | [**list_pages**](docs/DefaultApi.md#list_pages) | **GET** /pages | List all pages associated with a client
 *DefaultApi* | [**list_pages_by_page_template**](docs/DefaultApi.md#list_pages_by_page_template) | **GET** /pages/page-template-slug-{page_template_slug} | List all pages associated with a particular page template and optionally client
+*DefaultApi* | [**list_report_configs**](docs/DefaultApi.md#list_report_configs) | **GET** /report-configs | List all report_configs associated with a client
+*DefaultApi* | [**list_reports**](docs/DefaultApi.md#list_reports) | **GET** /reports | List all reports associated with a client
 *DefaultApi* | [**list_role_permissions**](docs/DefaultApi.md#list_role_permissions) | **GET** /role-permissions | List all permissions for a specific role
 *DefaultApi* | [**list_roles**](docs/DefaultApi.md#list_roles) | **GET** /roles | List roles associated with a client
 *DefaultApi* | [**list_schemas**](docs/DefaultApi.md#list_schemas) | **GET** /schemas | List all schemas associated with a client
 *DefaultApi* | [**list_terms**](docs/DefaultApi.md#list_terms) | **GET** /terms | List all terms associated with a client
+*DefaultApi* | [**list_upload_requests**](docs/DefaultApi.md#list_upload_requests) | **GET** /upload-requests | Gets all unexpired upload requests for the authenticated user
 *DefaultApi* | [**list_user_roles**](docs/DefaultApi.md#list_user_roles) | **GET** /user-roles/{user_id} | List all roles for a specific user
 *DefaultApi* | [**list_users**](docs/DefaultApi.md#list_users) | **GET** /users | List active users associated with a client
 *DefaultApi* | [**list_views**](docs/DefaultApi.md#list_views) | **GET** /views | List metadata for all views associated with a client
 *DefaultApi* | [**list_widget_types**](docs/DefaultApi.md#list_widget_types) | **GET** /widget-types | List all widget types
 *DefaultApi* | [**load_client_package**](docs/DefaultApi.md#load_client_package) | **POST** /client-packages/load | Imports data for a client into the current environment
 *DefaultApi* | [**me**](docs/DefaultApi.md#me) | **GET** /users/me | Get data about the authenticated user
 *DefaultApi* | [**query**](docs/DefaultApi.md#query) | **POST** /data-views | Performs a query against an existing dataset
@@ -212,14 +226,16 @@
 *DefaultApi* | [**update_client_setting**](docs/DefaultApi.md#update_client_setting) | **PATCH** /client-settings/client-id-{client_id} | Insert or update new client-specific settings
 *DefaultApi* | [**update_dataset**](docs/DefaultApi.md#update_dataset) | **PATCH** /datasets/{dataset_id} | Updates an existing dataset
 *DefaultApi* | [**update_geodata**](docs/DefaultApi.md#update_geodata) | **PATCH** /geodata/update | Updates an existing geo type
 *DefaultApi* | [**update_goal**](docs/DefaultApi.md#update_goal) | **PATCH** /goals/{goal_id} | Updates an existing goal
 *DefaultApi* | [**update_integration**](docs/DefaultApi.md#update_integration) | **PATCH** /integrations/{integration_id} | Updates an existing integration
 *DefaultApi* | [**update_integration_type**](docs/DefaultApi.md#update_integration_type) | **PATCH** /integration-types/{integration_type_id} | Updates an existing integration type
 *DefaultApi* | [**update_page_preference**](docs/DefaultApi.md#update_page_preference) | **PATCH** /page-preferences/page-id-{page_id} | Add or update a page preference
+*DefaultApi* | [**update_report**](docs/DefaultApi.md#update_report) | **PATCH** /reports/{report_id} | Updates an existing report
+*DefaultApi* | [**update_report_config**](docs/DefaultApi.md#update_report_config) | **PATCH** /report-configs/{report_config_id} | Updates an existing report_config
 *DefaultApi* | [**update_role**](docs/DefaultApi.md#update_role) | **PATCH** /roles/{role_id} | Updates an existing role
 *DefaultApi* | [**update_term**](docs/DefaultApi.md#update_term) | **PATCH** /terms/{term_id} | Updates an existing term
 *DefaultApi* | [**update_user**](docs/DefaultApi.md#update_user) | **PATCH** /users/{user_id} | Updates an existing user
 *DefaultApi* | [**update_widget_type**](docs/DefaultApi.md#update_widget_type) | **PATCH** /widget-types/{widget_type_id} | Updates an existing widget type
 
 
 ## Documentation For Models
@@ -303,14 +319,16 @@
  - [DivideMetric](docs/DivideMetric.md)
  - [Download](docs/Download.md)
  - [DownloadError](docs/DownloadError.md)
  - [DownloadV1](docs/DownloadV1.md)
  - [DownloadV2](docs/DownloadV2.md)
  - [DropTransform](docs/DropTransform.md)
  - [DruidWriteConfig](docs/DruidWriteConfig.md)
+ - [EmailAddress](docs/EmailAddress.md)
+ - [EmailReportConfig](docs/EmailReportConfig.md)
  - [EntityBatch](docs/EntityBatch.md)
  - [EntityBatchHealth](docs/EntityBatchHealth.md)
  - [Filter](docs/Filter.md)
  - [FilterMap](docs/FilterMap.md)
  - [FilterPreset](docs/FilterPreset.md)
  - [GeoData](docs/GeoData.md)
  - [Goal](docs/Goal.md)
@@ -323,14 +341,15 @@
  - [IntegrationType](docs/IntegrationType.md)
  - [IntegrationTypeUpdate](docs/IntegrationTypeUpdate.md)
  - [IntegrationUpdate](docs/IntegrationUpdate.md)
  - [Job](docs/Job.md)
  - [JobOverview](docs/JobOverview.md)
  - [Join](docs/Join.md)
  - [JoinRelationship](docs/JoinRelationship.md)
+ - [Link](docs/Link.md)
  - [LoaderSettings](docs/LoaderSettings.md)
  - [MapExplodeManyTransform](docs/MapExplodeManyTransform.md)
  - [MapExplodeTransform](docs/MapExplodeTransform.md)
  - [MapTransform](docs/MapTransform.md)
  - [MultiplyMetric](docs/MultiplyMetric.md)
  - [NewUserToken](docs/NewUserToken.md)
  - [NonNullFilter](docs/NonNullFilter.md)
@@ -342,14 +361,15 @@
  - [NumberBucketTransform](docs/NumberBucketTransform.md)
  - [NumberCastTransform](docs/NumberCastTransform.md)
  - [NumberConstantTransform](docs/NumberConstantTransform.md)
  - [NumberDefaultTransform](docs/NumberDefaultTransform.md)
  - [NumberFilter](docs/NumberFilter.md)
  - [NumberTransform](docs/NumberTransform.md)
  - [NumberUnaryTransform](docs/NumberUnaryTransform.md)
+ - [Options](docs/Options.md)
  - [OrFilter](docs/OrFilter.md)
  - [Page](docs/Page.md)
  - [PageFilterPreferences](docs/PageFilterPreferences.md)
  - [PageFull](docs/PageFull.md)
  - [PagePreferences](docs/PagePreferences.md)
  - [PagePreferencesUpdate](docs/PagePreferencesUpdate.md)
  - [PagePublications](docs/PagePublications.md)
@@ -357,20 +377,35 @@
  - [PageTemplateUpdate](docs/PageTemplateUpdate.md)
  - [PageView](docs/PageView.md)
  - [PartnerBatch](docs/PartnerBatch.md)
  - [PartnerPostData](docs/PartnerPostData.md)
  - [PasswordChangeRequest](docs/PasswordChangeRequest.md)
  - [PasswordResetChange](docs/PasswordResetChange.md)
  - [PasswordResetRequest](docs/PasswordResetRequest.md)
+ - [PercentageMetric](docs/PercentageMetric.md)
  - [PercentileLookupMetric](docs/PercentileLookupMetric.md)
  - [PostData](docs/PostData.md)
+ - [ProlearnBaseObject](docs/ProlearnBaseObject.md)
+ - [ProlearnCallback](docs/ProlearnCallback.md)
+ - [ProlearnCourse](docs/ProlearnCourse.md)
+ - [ProlearnCredit](docs/ProlearnCredit.md)
+ - [ProlearnCreditType](docs/ProlearnCreditType.md)
+ - [ProlearnRegistration](docs/ProlearnRegistration.md)
+ - [ProlearnUser](docs/ProlearnUser.md)
  - [RefreshInterval](docs/RefreshInterval.md)
  - [RefreshSchedule](docs/RefreshSchedule.md)
  - [RefreshState](docs/RefreshState.md)
  - [RenameTransform](docs/RenameTransform.md)
+ - [RenameTransform2](docs/RenameTransform2.md)
+ - [Report](docs/Report.md)
+ - [ReportAdd](docs/ReportAdd.md)
+ - [ReportConfig](docs/ReportConfig.md)
+ - [ReportConfigUpdate](docs/ReportConfigUpdate.md)
+ - [ReportError](docs/ReportError.md)
+ - [ReportUpdate](docs/ReportUpdate.md)
  - [Role](docs/Role.md)
  - [RolePermission](docs/RolePermission.md)
  - [RoleUpdate](docs/RoleUpdate.md)
  - [SarimaxDatasetTask](docs/SarimaxDatasetTask.md)
  - [SarimaxTask](docs/SarimaxTask.md)
  - [SarimaxTaskMetric](docs/SarimaxTaskMetric.md)
  - [Schema](docs/Schema.md)
@@ -419,23 +454,26 @@
  - [TopNTaskPartition](docs/TopNTaskPartition.md)
  - [TopNTaskSort](docs/TopNTaskSort.md)
  - [Transform](docs/Transform.md)
  - [UnaryMetric](docs/UnaryMetric.md)
  - [UniqueLimit](docs/UniqueLimit.md)
  - [UpdateApiUser](docs/UpdateApiUser.md)
  - [UpdateUser](docs/UpdateUser.md)
+ - [Upload](docs/Upload.md)
+ - [UploadField](docs/UploadField.md)
  - [UserActivation](docs/UserActivation.md)
  - [UserRole](docs/UserRole.md)
  - [UserToken](docs/UserToken.md)
  - [View](docs/View.md)
  - [ViewError](docs/ViewError.md)
  - [VirtualUser](docs/VirtualUser.md)
  - [Widget](docs/Widget.md)
  - [WidgetFull](docs/WidgetFull.md)
  - [WidgetType](docs/WidgetType.md)
+ - [WriteBackup](docs/WriteBackup.md)
  - [WriteConfig](docs/WriteConfig.md)
  - [WriteConfigDruidOverride](docs/WriteConfigDruidOverride.md)
  - [WriteConfigOverride](docs/WriteConfigOverride.md)
 
 
 ## Documentation For Authorization
```

### Comparing `nucleus_client-0.8.0/nucleus_client/__init__.py` & `nucleus_client-0.9.0/nucleus_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     OpenAPI spec version: v1
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 # import apis into sdk package
 from nucleus_client.api.default_api import DefaultApi
 
 # import ApiClient
 from nucleus_client.api_client import ApiClient
 from nucleus_client.configuration import Configuration
@@ -102,14 +102,16 @@
 from nucleus_client.models.divide_metric import DivideMetric
 from nucleus_client.models.download import Download
 from nucleus_client.models.download_error import DownloadError
 from nucleus_client.models.download_v1 import DownloadV1
 from nucleus_client.models.download_v2 import DownloadV2
 from nucleus_client.models.drop_transform import DropTransform
 from nucleus_client.models.druid_write_config import DruidWriteConfig
+from nucleus_client.models.email_address import EmailAddress
+from nucleus_client.models.email_report_config import EmailReportConfig
 from nucleus_client.models.entity_batch import EntityBatch
 from nucleus_client.models.entity_batch_health import EntityBatchHealth
 from nucleus_client.models.filter import Filter
 from nucleus_client.models.filter_map import FilterMap
 from nucleus_client.models.filter_preset import FilterPreset
 from nucleus_client.models.geo_data import GeoData
 from nucleus_client.models.goal import Goal
@@ -122,14 +124,15 @@
 from nucleus_client.models.integration_type import IntegrationType
 from nucleus_client.models.integration_type_update import IntegrationTypeUpdate
 from nucleus_client.models.integration_update import IntegrationUpdate
 from nucleus_client.models.job import Job
 from nucleus_client.models.job_overview import JobOverview
 from nucleus_client.models.join import Join
 from nucleus_client.models.join_relationship import JoinRelationship
+from nucleus_client.models.link import Link
 from nucleus_client.models.loader_settings import LoaderSettings
 from nucleus_client.models.map_explode_many_transform import MapExplodeManyTransform
 from nucleus_client.models.map_explode_transform import MapExplodeTransform
 from nucleus_client.models.map_transform import MapTransform
 from nucleus_client.models.multiply_metric import MultiplyMetric
 from nucleus_client.models.new_user_token import NewUserToken
 from nucleus_client.models.non_null_filter import NonNullFilter
@@ -141,14 +144,15 @@
 from nucleus_client.models.number_bucket_transform import NumberBucketTransform
 from nucleus_client.models.number_cast_transform import NumberCastTransform
 from nucleus_client.models.number_constant_transform import NumberConstantTransform
 from nucleus_client.models.number_default_transform import NumberDefaultTransform
 from nucleus_client.models.number_filter import NumberFilter
 from nucleus_client.models.number_transform import NumberTransform
 from nucleus_client.models.number_unary_transform import NumberUnaryTransform
+from nucleus_client.models.options import Options
 from nucleus_client.models.or_filter import OrFilter
 from nucleus_client.models.page import Page
 from nucleus_client.models.page_filter_preferences import PageFilterPreferences
 from nucleus_client.models.page_full import PageFull
 from nucleus_client.models.page_preferences import PagePreferences
 from nucleus_client.models.page_preferences_update import PagePreferencesUpdate
 from nucleus_client.models.page_publications import PagePublications
@@ -156,20 +160,35 @@
 from nucleus_client.models.page_template_update import PageTemplateUpdate
 from nucleus_client.models.page_view import PageView
 from nucleus_client.models.partner_batch import PartnerBatch
 from nucleus_client.models.partner_post_data import PartnerPostData
 from nucleus_client.models.password_change_request import PasswordChangeRequest
 from nucleus_client.models.password_reset_change import PasswordResetChange
 from nucleus_client.models.password_reset_request import PasswordResetRequest
+from nucleus_client.models.percentage_metric import PercentageMetric
 from nucleus_client.models.percentile_lookup_metric import PercentileLookupMetric
 from nucleus_client.models.post_data import PostData
+from nucleus_client.models.prolearn_base_object import ProlearnBaseObject
+from nucleus_client.models.prolearn_callback import ProlearnCallback
+from nucleus_client.models.prolearn_course import ProlearnCourse
+from nucleus_client.models.prolearn_credit import ProlearnCredit
+from nucleus_client.models.prolearn_credit_type import ProlearnCreditType
+from nucleus_client.models.prolearn_registration import ProlearnRegistration
+from nucleus_client.models.prolearn_user import ProlearnUser
 from nucleus_client.models.refresh_interval import RefreshInterval
 from nucleus_client.models.refresh_schedule import RefreshSchedule
 from nucleus_client.models.refresh_state import RefreshState
 from nucleus_client.models.rename_transform import RenameTransform
+from nucleus_client.models.rename_transform2 import RenameTransform2
+from nucleus_client.models.report import Report
+from nucleus_client.models.report_add import ReportAdd
+from nucleus_client.models.report_config import ReportConfig
+from nucleus_client.models.report_config_update import ReportConfigUpdate
+from nucleus_client.models.report_error import ReportError
+from nucleus_client.models.report_update import ReportUpdate
 from nucleus_client.models.role import Role
 from nucleus_client.models.role_permission import RolePermission
 from nucleus_client.models.role_update import RoleUpdate
 from nucleus_client.models.sarimax_dataset_task import SarimaxDatasetTask
 from nucleus_client.models.sarimax_task import SarimaxTask
 from nucleus_client.models.sarimax_task_metric import SarimaxTaskMetric
 from nucleus_client.models.schema import Schema
@@ -218,19 +237,22 @@
 from nucleus_client.models.top_n_task_partition import TopNTaskPartition
 from nucleus_client.models.top_n_task_sort import TopNTaskSort
 from nucleus_client.models.transform import Transform
 from nucleus_client.models.unary_metric import UnaryMetric
 from nucleus_client.models.unique_limit import UniqueLimit
 from nucleus_client.models.update_api_user import UpdateApiUser
 from nucleus_client.models.update_user import UpdateUser
+from nucleus_client.models.upload import Upload
+from nucleus_client.models.upload_field import UploadField
 from nucleus_client.models.user_activation import UserActivation
 from nucleus_client.models.user_role import UserRole
 from nucleus_client.models.user_token import UserToken
 from nucleus_client.models.view import View
 from nucleus_client.models.view_error import ViewError
 from nucleus_client.models.virtual_user import VirtualUser
 from nucleus_client.models.widget import Widget
 from nucleus_client.models.widget_full import WidgetFull
 from nucleus_client.models.widget_type import WidgetType
+from nucleus_client.models.write_backup import WriteBackup
 from nucleus_client.models.write_config import WriteConfig
 from nucleus_client.models.write_config_druid_override import WriteConfigDruidOverride
 from nucleus_client.models.write_config_override import WriteConfigOverride
```

### Comparing `nucleus_client-0.8.0/nucleus_client/api/default_api.py` & `nucleus_client-0.9.0/nucleus_client/api/default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1502,14 +1502,120 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def add_integration_sync_request(self, client_id, integration_id, **kwargs):  # noqa: E501
+        """Run a sync integration      Responses:          204: The sync request was successfully queued  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_integration_sync_request(client_id, integration_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param str integration_id: (required)
+        :param str sync_method:
+        :param str param1:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.add_integration_sync_request_with_http_info(client_id, integration_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.add_integration_sync_request_with_http_info(client_id, integration_id, **kwargs)  # noqa: E501
+            return data
+
+    def add_integration_sync_request_with_http_info(self, client_id, integration_id, **kwargs):  # noqa: E501
+        """Run a sync integration      Responses:          204: The sync request was successfully queued  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_integration_sync_request_with_http_info(client_id, integration_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param str integration_id: (required)
+        :param str sync_method:
+        :param str param1:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['client_id', 'integration_id', 'sync_method', 'param1']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method add_integration_sync_request" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `add_integration_sync_request`")  # noqa: E501
+        # verify the required parameter 'integration_id' is set
+        if ('integration_id' not in local_var_params or
+                local_var_params['integration_id'] is None):
+            raise ValueError("Missing the required parameter `integration_id` when calling `add_integration_sync_request`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+        if 'integration_id' in local_var_params:
+            query_params.append(('integration_id', local_var_params['integration_id']))  # noqa: E501
+        if 'sync_method' in local_var_params:
+            query_params.append(('sync_method', local_var_params['sync_method']))  # noqa: E501
+        if 'param1' in local_var_params:
+            query_params.append(('param1', local_var_params['param1']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/admin/integration-sync-requests/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def add_integration_type(self, **kwargs):  # noqa: E501
         """Add a new integration type  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.add_integration_type(async_req=True)
         >>> result = thread.get()
@@ -2102,14 +2208,316 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def add_prolearn_activity(self, client_id, integration_id, **kwargs):  # noqa: E501
+        """Prolearn callback  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_prolearn_activity(client_id, integration_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param str integration_id: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.add_prolearn_activity_with_http_info(client_id, integration_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.add_prolearn_activity_with_http_info(client_id, integration_id, **kwargs)  # noqa: E501
+            return data
+
+    def add_prolearn_activity_with_http_info(self, client_id, integration_id, **kwargs):  # noqa: E501
+        """Prolearn callback  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_prolearn_activity_with_http_info(client_id, integration_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param str integration_id: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['client_id', 'integration_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method add_prolearn_activity" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `add_prolearn_activity`")  # noqa: E501
+        # verify the required parameter 'integration_id' is set
+        if ('integration_id' not in local_var_params or
+                local_var_params['integration_id'] is None):
+            raise ValueError("Missing the required parameter `integration_id` when calling `add_prolearn_activity`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+        if 'integration_id' in local_var_params:
+            query_params.append(('integration_id', local_var_params['integration_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # Authentication setting
+        auth_settings = ['api_key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/callbacks/prolearn', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def add_report(self, client_id, **kwargs):  # noqa: E501
+        """Add a new report  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_report(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param ReportAdd body:
+        :return: Report
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.add_report_with_http_info(client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.add_report_with_http_info(client_id, **kwargs)  # noqa: E501
+            return data
+
+    def add_report_with_http_info(self, client_id, **kwargs):  # noqa: E501
+        """Add a new report  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_report_with_http_info(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param ReportAdd body:
+        :return: Report
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['client_id', 'body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method add_report" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `add_report`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in local_var_params:
+            body_params = local_var_params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/reports', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Report',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def add_report_config(self, client_id, **kwargs):  # noqa: E501
+        """Add a new report_config  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_report_config(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param ReportConfig body:
+        :return: ReportConfig
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.add_report_config_with_http_info(client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.add_report_config_with_http_info(client_id, **kwargs)  # noqa: E501
+            return data
+
+    def add_report_config_with_http_info(self, client_id, **kwargs):  # noqa: E501
+        """Add a new report_config  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_report_config_with_http_info(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param ReportConfig body:
+        :return: ReportConfig
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['client_id', 'body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method add_report_config" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `add_report_config`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in local_var_params:
+            body_params = local_var_params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/report-configs', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ReportConfig',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def add_role(self, client_id, **kwargs):  # noqa: E501
         """Adds a new role  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.add_role(client_id, async_req=True)
         >>> result = thread.get()
@@ -2412,14 +2820,116 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def add_upload_request(self, client_id, **kwargs):  # noqa: E501
+        """Adds a new (pending) upload request  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_upload_request(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param Upload body:
+        :return: Upload
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.add_upload_request_with_http_info(client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.add_upload_request_with_http_info(client_id, **kwargs)  # noqa: E501
+            return data
+
+    def add_upload_request_with_http_info(self, client_id, **kwargs):  # noqa: E501
+        """Adds a new (pending) upload request  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_upload_request_with_http_info(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param Upload body:
+        :return: Upload
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['client_id', 'body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method add_upload_request" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `add_upload_request`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in local_var_params:
+            body_params = local_var_params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/upload-requests', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Upload',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def add_user(self, **kwargs):  # noqa: E501
         """Adds a new user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.add_user(async_req=True)
         >>> result = thread.get()
@@ -4470,14 +4980,210 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def delete_report(self, report_id, client_id, **kwargs):  # noqa: E501
+        """Deletes a report by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_report(report_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_id: (required)
+        :param str client_id: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.delete_report_with_http_info(report_id, client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.delete_report_with_http_info(report_id, client_id, **kwargs)  # noqa: E501
+            return data
+
+    def delete_report_with_http_info(self, report_id, client_id, **kwargs):  # noqa: E501
+        """Deletes a report by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_report_with_http_info(report_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_id: (required)
+        :param str client_id: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['report_id', 'client_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_report" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'report_id' is set
+        if ('report_id' not in local_var_params or
+                local_var_params['report_id'] is None):
+            raise ValueError("Missing the required parameter `report_id` when calling `delete_report`")  # noqa: E501
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `delete_report`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'report_id' in local_var_params:
+            path_params['report_id'] = local_var_params['report_id']  # noqa: E501
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/reports/{report_id}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_report_config(self, report_config_id, client_id, **kwargs):  # noqa: E501
+        """Deletes a report_config by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_report_config(report_config_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_config_id: (required)
+        :param str client_id: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.delete_report_config_with_http_info(report_config_id, client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.delete_report_config_with_http_info(report_config_id, client_id, **kwargs)  # noqa: E501
+            return data
+
+    def delete_report_config_with_http_info(self, report_config_id, client_id, **kwargs):  # noqa: E501
+        """Deletes a report_config by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_report_config_with_http_info(report_config_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_config_id: (required)
+        :param str client_id: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['report_config_id', 'client_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_report_config" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'report_config_id' is set
+        if ('report_config_id' not in local_var_params or
+                local_var_params['report_config_id'] is None):
+            raise ValueError("Missing the required parameter `report_config_id` when calling `delete_report_config`")  # noqa: E501
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `delete_report_config`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'report_config_id' in local_var_params:
+            path_params['report_config_id'] = local_var_params['report_config_id']  # noqa: E501
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/report-configs/{report_config_id}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def delete_role(self, role_id, client_id, **kwargs):  # noqa: E501
         """Deletes a role by ID  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_role(role_id, client_id, async_req=True)
         >>> result = thread.get()
@@ -6127,15 +6833,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json', 'text/csv'])  # noqa: E501
+            ['text/csv'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basic', 'jwt']  # noqa: E501
 
         return self.api_client.call_api(
             '/downloads/{download_id}', 'GET',
             path_params,
@@ -7622,14 +8328,320 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_report(self, report_id, client_id, **kwargs):  # noqa: E501
+        """Get a report by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_report(report_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_id: (required)
+        :param str client_id: (required)
+        :return: Report
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_report_with_http_info(report_id, client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_report_with_http_info(report_id, client_id, **kwargs)  # noqa: E501
+            return data
+
+    def get_report_with_http_info(self, report_id, client_id, **kwargs):  # noqa: E501
+        """Get a report by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_report_with_http_info(report_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_id: (required)
+        :param str client_id: (required)
+        :return: Report
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['report_id', 'client_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_report" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'report_id' is set
+        if ('report_id' not in local_var_params or
+                local_var_params['report_id'] is None):
+            raise ValueError("Missing the required parameter `report_id` when calling `get_report`")  # noqa: E501
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `get_report`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'report_id' in local_var_params:
+            path_params['report_id'] = local_var_params['report_id']  # noqa: E501
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/reports/{report_id}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Report',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_report_config(self, report_config_id, client_id, **kwargs):  # noqa: E501
+        """Get a report_config by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_report_config(report_config_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_config_id: (required)
+        :param str client_id: (required)
+        :return: ReportConfig
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_report_config_with_http_info(report_config_id, client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_report_config_with_http_info(report_config_id, client_id, **kwargs)  # noqa: E501
+            return data
+
+    def get_report_config_with_http_info(self, report_config_id, client_id, **kwargs):  # noqa: E501
+        """Get a report_config by ID  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_report_config_with_http_info(report_config_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_config_id: (required)
+        :param str client_id: (required)
+        :return: ReportConfig
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['report_config_id', 'client_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_report_config" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'report_config_id' is set
+        if ('report_config_id' not in local_var_params or
+                local_var_params['report_config_id'] is None):
+            raise ValueError("Missing the required parameter `report_config_id` when calling `get_report_config`")  # noqa: E501
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `get_report_config`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'report_config_id' in local_var_params:
+            path_params['report_config_id'] = local_var_params['report_config_id']  # noqa: E501
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/report-configs/{report_config_id}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ReportConfig',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_report_config_by_name(self, report_config_name, client_id, **kwargs):  # noqa: E501
+        """Get a report_config by name  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_report_config_by_name(report_config_name, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_config_name: (required)
+        :param str client_id: (required)
+        :return: ReportConfig
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_report_config_by_name_with_http_info(report_config_name, client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_report_config_by_name_with_http_info(report_config_name, client_id, **kwargs)  # noqa: E501
+            return data
+
+    def get_report_config_by_name_with_http_info(self, report_config_name, client_id, **kwargs):  # noqa: E501
+        """Get a report_config by name  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_report_config_by_name_with_http_info(report_config_name, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_config_name: (required)
+        :param str client_id: (required)
+        :return: ReportConfig
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['report_config_name', 'client_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_report_config_by_name" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'report_config_name' is set
+        if ('report_config_name' not in local_var_params or
+                local_var_params['report_config_name'] is None):
+            raise ValueError("Missing the required parameter `report_config_name` when calling `get_report_config_by_name`")  # noqa: E501
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `get_report_config_by_name`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'report_config_name' in local_var_params:
+            path_params['report_config_name'] = local_var_params['report_config_name']  # noqa: E501
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/report-configs/name-{report_config_name}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ReportConfig',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_role(self, role_id, client_id, **kwargs):  # noqa: E501
         """Gets a role by ID  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_role(role_id, client_id, async_req=True)
         >>> result = thread.get()
@@ -8242,14 +9254,116 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_upload_request(self, upload_id, client_id, **kwargs):  # noqa: E501
+        """Gets an upload request by id  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_upload_request(upload_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str upload_id: (required)
+        :param str client_id: (required)
+        :return: Upload
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_upload_request_with_http_info(upload_id, client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_upload_request_with_http_info(upload_id, client_id, **kwargs)  # noqa: E501
+            return data
+
+    def get_upload_request_with_http_info(self, upload_id, client_id, **kwargs):  # noqa: E501
+        """Gets an upload request by id  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_upload_request_with_http_info(upload_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str upload_id: (required)
+        :param str client_id: (required)
+        :return: Upload
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['upload_id', 'client_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_upload_request" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'upload_id' is set
+        if ('upload_id' not in local_var_params or
+                local_var_params['upload_id'] is None):
+            raise ValueError("Missing the required parameter `upload_id` when calling `get_upload_request`")  # noqa: E501
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `get_upload_request`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'upload_id' in local_var_params:
+            path_params['upload_id'] = local_var_params['upload_id']  # noqa: E501
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/upload-requests/{upload_id}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Upload',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_user(self, user_id, **kwargs):  # noqa: E501
         """Gets a user by ID  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_user(user_id, async_req=True)
         >>> result = thread.get()
@@ -9123,15 +10237,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json', 'text/csv'])  # noqa: E501
+            ['text/csv'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['api_key', 'basic', 'jwt']  # noqa: E501
 
         return self.api_client.call_api(
             '/activities', 'GET',
             path_params,
@@ -10934,14 +12048,202 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def list_report_configs(self, client_id, **kwargs):  # noqa: E501
+        """List all report_configs associated with a client  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_report_configs(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :return: list[ReportConfig]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.list_report_configs_with_http_info(client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.list_report_configs_with_http_info(client_id, **kwargs)  # noqa: E501
+            return data
+
+    def list_report_configs_with_http_info(self, client_id, **kwargs):  # noqa: E501
+        """List all report_configs associated with a client  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_report_configs_with_http_info(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :return: list[ReportConfig]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['client_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_report_configs" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `list_report_configs`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/report-configs', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[ReportConfig]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def list_reports(self, client_id, **kwargs):  # noqa: E501
+        """List all reports associated with a client  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_reports(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :return: list[Report]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.list_reports_with_http_info(client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.list_reports_with_http_info(client_id, **kwargs)  # noqa: E501
+            return data
+
+    def list_reports_with_http_info(self, client_id, **kwargs):  # noqa: E501
+        """List all reports associated with a client  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_reports_with_http_info(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :return: list[Report]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['client_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_reports" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `list_reports`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/reports', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[Report]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def list_role_permissions(self, client_id, role_id, **kwargs):  # noqa: E501
         """List all permissions for a specific role  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_role_permissions(client_id, role_id, async_req=True)
         >>> result = thread.get()
@@ -11330,14 +12632,108 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def list_upload_requests(self, client_id, **kwargs):  # noqa: E501
+        """Gets all unexpired upload requests for the authenticated user  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_upload_requests(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param str status:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.list_upload_requests_with_http_info(client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.list_upload_requests_with_http_info(client_id, **kwargs)  # noqa: E501
+            return data
+
+    def list_upload_requests_with_http_info(self, client_id, **kwargs):  # noqa: E501
+        """Gets all unexpired upload requests for the authenticated user  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_upload_requests_with_http_info(client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str client_id: (required)
+        :param str status:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['client_id', 'status']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_upload_requests" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `list_upload_requests`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+        if 'status' in local_var_params:
+            query_params.append(('status', local_var_params['status']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/upload-requests', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def list_user_roles(self, user_id, client_id, **kwargs):  # noqa: E501
         """List all roles for a specific user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_user_roles(user_id, client_id, async_req=True)
         >>> result = thread.get()
@@ -13449,14 +14845,226 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_report(self, report_id, client_id, **kwargs):  # noqa: E501
+        """Updates an existing report  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_report(report_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_id: (required)
+        :param str client_id: (required)
+        :param ReportUpdate body:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.update_report_with_http_info(report_id, client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_report_with_http_info(report_id, client_id, **kwargs)  # noqa: E501
+            return data
+
+    def update_report_with_http_info(self, report_id, client_id, **kwargs):  # noqa: E501
+        """Updates an existing report  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_report_with_http_info(report_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_id: (required)
+        :param str client_id: (required)
+        :param ReportUpdate body:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['report_id', 'client_id', 'body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_report" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'report_id' is set
+        if ('report_id' not in local_var_params or
+                local_var_params['report_id'] is None):
+            raise ValueError("Missing the required parameter `report_id` when calling `update_report`")  # noqa: E501
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `update_report`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'report_id' in local_var_params:
+            path_params['report_id'] = local_var_params['report_id']  # noqa: E501
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in local_var_params:
+            body_params = local_var_params['body']
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/reports/{report_id}', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_report_config(self, report_config_id, client_id, **kwargs):  # noqa: E501
+        """Updates an existing report_config  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_report_config(report_config_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_config_id: (required)
+        :param str client_id: (required)
+        :param ReportConfigUpdate body:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.update_report_config_with_http_info(report_config_id, client_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_report_config_with_http_info(report_config_id, client_id, **kwargs)  # noqa: E501
+            return data
+
+    def update_report_config_with_http_info(self, report_config_id, client_id, **kwargs):  # noqa: E501
+        """Updates an existing report_config  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_report_config_with_http_info(report_config_id, client_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str report_config_id: (required)
+        :param str client_id: (required)
+        :param ReportConfigUpdate body:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['report_config_id', 'client_id', 'body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_report_config" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'report_config_id' is set
+        if ('report_config_id' not in local_var_params or
+                local_var_params['report_config_id'] is None):
+            raise ValueError("Missing the required parameter `report_config_id` when calling `update_report_config`")  # noqa: E501
+        # verify the required parameter 'client_id' is set
+        if ('client_id' not in local_var_params or
+                local_var_params['client_id'] is None):
+            raise ValueError("Missing the required parameter `client_id` when calling `update_report_config`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'report_config_id' in local_var_params:
+            path_params['report_config_id'] = local_var_params['report_config_id']  # noqa: E501
+
+        query_params = []
+        if 'client_id' in local_var_params:
+            query_params.append(('client_id', local_var_params['client_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in local_var_params:
+            body_params = local_var_params['body']
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key', 'jwt']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/report-configs/{report_config_id}', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `nucleus_client-0.8.0/nucleus_client/api_client.py` & `nucleus_client-0.9.0/nucleus_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.8.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.9.0/python'
 
     def __del__(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
             self._pool = None
```

### Comparing `nucleus_client-0.8.0/nucleus_client/configuration.py` & `nucleus_client-0.9.0/nucleus_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,9 +248,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 0.8.0".\
+               "SDK Package Version: 0.9.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/__init__.py` & `nucleus_client-0.9.0/nucleus_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,16 @@
 from nucleus_client.models.divide_metric import DivideMetric
 from nucleus_client.models.download import Download
 from nucleus_client.models.download_error import DownloadError
 from nucleus_client.models.download_v1 import DownloadV1
 from nucleus_client.models.download_v2 import DownloadV2
 from nucleus_client.models.drop_transform import DropTransform
 from nucleus_client.models.druid_write_config import DruidWriteConfig
+from nucleus_client.models.email_address import EmailAddress
+from nucleus_client.models.email_report_config import EmailReportConfig
 from nucleus_client.models.entity_batch import EntityBatch
 from nucleus_client.models.entity_batch_health import EntityBatchHealth
 from nucleus_client.models.filter import Filter
 from nucleus_client.models.filter_map import FilterMap
 from nucleus_client.models.filter_preset import FilterPreset
 from nucleus_client.models.geo_data import GeoData
 from nucleus_client.models.goal import Goal
@@ -113,14 +115,15 @@
 from nucleus_client.models.integration_type import IntegrationType
 from nucleus_client.models.integration_type_update import IntegrationTypeUpdate
 from nucleus_client.models.integration_update import IntegrationUpdate
 from nucleus_client.models.job import Job
 from nucleus_client.models.job_overview import JobOverview
 from nucleus_client.models.join import Join
 from nucleus_client.models.join_relationship import JoinRelationship
+from nucleus_client.models.link import Link
 from nucleus_client.models.loader_settings import LoaderSettings
 from nucleus_client.models.map_explode_many_transform import MapExplodeManyTransform
 from nucleus_client.models.map_explode_transform import MapExplodeTransform
 from nucleus_client.models.map_transform import MapTransform
 from nucleus_client.models.multiply_metric import MultiplyMetric
 from nucleus_client.models.new_user_token import NewUserToken
 from nucleus_client.models.non_null_filter import NonNullFilter
@@ -132,14 +135,15 @@
 from nucleus_client.models.number_bucket_transform import NumberBucketTransform
 from nucleus_client.models.number_cast_transform import NumberCastTransform
 from nucleus_client.models.number_constant_transform import NumberConstantTransform
 from nucleus_client.models.number_default_transform import NumberDefaultTransform
 from nucleus_client.models.number_filter import NumberFilter
 from nucleus_client.models.number_transform import NumberTransform
 from nucleus_client.models.number_unary_transform import NumberUnaryTransform
+from nucleus_client.models.options import Options
 from nucleus_client.models.or_filter import OrFilter
 from nucleus_client.models.page import Page
 from nucleus_client.models.page_filter_preferences import PageFilterPreferences
 from nucleus_client.models.page_full import PageFull
 from nucleus_client.models.page_preferences import PagePreferences
 from nucleus_client.models.page_preferences_update import PagePreferencesUpdate
 from nucleus_client.models.page_publications import PagePublications
@@ -147,20 +151,35 @@
 from nucleus_client.models.page_template_update import PageTemplateUpdate
 from nucleus_client.models.page_view import PageView
 from nucleus_client.models.partner_batch import PartnerBatch
 from nucleus_client.models.partner_post_data import PartnerPostData
 from nucleus_client.models.password_change_request import PasswordChangeRequest
 from nucleus_client.models.password_reset_change import PasswordResetChange
 from nucleus_client.models.password_reset_request import PasswordResetRequest
+from nucleus_client.models.percentage_metric import PercentageMetric
 from nucleus_client.models.percentile_lookup_metric import PercentileLookupMetric
 from nucleus_client.models.post_data import PostData
+from nucleus_client.models.prolearn_base_object import ProlearnBaseObject
+from nucleus_client.models.prolearn_callback import ProlearnCallback
+from nucleus_client.models.prolearn_course import ProlearnCourse
+from nucleus_client.models.prolearn_credit import ProlearnCredit
+from nucleus_client.models.prolearn_credit_type import ProlearnCreditType
+from nucleus_client.models.prolearn_registration import ProlearnRegistration
+from nucleus_client.models.prolearn_user import ProlearnUser
 from nucleus_client.models.refresh_interval import RefreshInterval
 from nucleus_client.models.refresh_schedule import RefreshSchedule
 from nucleus_client.models.refresh_state import RefreshState
 from nucleus_client.models.rename_transform import RenameTransform
+from nucleus_client.models.rename_transform2 import RenameTransform2
+from nucleus_client.models.report import Report
+from nucleus_client.models.report_add import ReportAdd
+from nucleus_client.models.report_config import ReportConfig
+from nucleus_client.models.report_config_update import ReportConfigUpdate
+from nucleus_client.models.report_error import ReportError
+from nucleus_client.models.report_update import ReportUpdate
 from nucleus_client.models.role import Role
 from nucleus_client.models.role_permission import RolePermission
 from nucleus_client.models.role_update import RoleUpdate
 from nucleus_client.models.sarimax_dataset_task import SarimaxDatasetTask
 from nucleus_client.models.sarimax_task import SarimaxTask
 from nucleus_client.models.sarimax_task_metric import SarimaxTaskMetric
 from nucleus_client.models.schema import Schema
@@ -209,19 +228,22 @@
 from nucleus_client.models.top_n_task_partition import TopNTaskPartition
 from nucleus_client.models.top_n_task_sort import TopNTaskSort
 from nucleus_client.models.transform import Transform
 from nucleus_client.models.unary_metric import UnaryMetric
 from nucleus_client.models.unique_limit import UniqueLimit
 from nucleus_client.models.update_api_user import UpdateApiUser
 from nucleus_client.models.update_user import UpdateUser
+from nucleus_client.models.upload import Upload
+from nucleus_client.models.upload_field import UploadField
 from nucleus_client.models.user_activation import UserActivation
 from nucleus_client.models.user_role import UserRole
 from nucleus_client.models.user_token import UserToken
 from nucleus_client.models.view import View
 from nucleus_client.models.view_error import ViewError
 from nucleus_client.models.virtual_user import VirtualUser
 from nucleus_client.models.widget import Widget
 from nucleus_client.models.widget_full import WidgetFull
 from nucleus_client.models.widget_type import WidgetType
+from nucleus_client.models.write_backup import WriteBackup
 from nucleus_client.models.write_config import WriteConfig
 from nucleus_client.models.write_config_druid_override import WriteConfigDruidOverride
 from nucleus_client.models.write_config_override import WriteConfigOverride
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/activity.py` & `nucleus_client-0.9.0/nucleus_client/models/activity.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/add_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/add_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/aggregation_dataset_task.py` & `nucleus_client-0.9.0/nucleus_client/models/aggregation_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/aggregation_parameterized_task.py` & `nucleus_client-0.9.0/nucleus_client/models/aggregation_parameterized_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/aggregation_task.py` & `nucleus_client-0.9.0/nucleus_client/models/aggregation_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/aggregation_task_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/aggregation_task_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         'cumulative_count': 'UnaryMetric',
         'cumulative_sum': 'CumulativeSumMetric',
         'divide': 'DivideMetric',
         'implode': 'UnaryMetric',
         'kurtosis': 'UnaryMetric',
         'min': 'UnaryMetric',
         'multiply': 'MultiplyMetric',
+        'percentage': 'PercentageMetric',
         'percentile_lookup': 'PercentileLookupMetric',
         'sample_standard_deviation': 'UnaryMetric',
         'sample_stddev': 'UnaryMetric',
         'skewness': 'UnaryMetric',
         'standard_deviation': 'UnaryMetric',
         'stddev': 'UnaryMetric',
         'subtract': 'SubtractMetric',
@@ -71,26 +72,27 @@
         'cumulative_count': 'cumulative_count',
         'cumulative_sum': 'cumulative_sum',
         'divide': 'divide',
         'implode': 'implode',
         'kurtosis': 'kurtosis',
         'min': 'min',
         'multiply': 'multiply',
+        'percentage': 'percentage',
         'percentile_lookup': 'percentile_lookup',
         'sample_standard_deviation': 'sample_standard_deviation',
         'sample_stddev': 'sample_stddev',
         'skewness': 'skewness',
         'standard_deviation': 'standard_deviation',
         'stddev': 'stddev',
         'subtract': 'subtract',
         'sum': 'sum',
         'variance': 'variance'
     }
 
-    def __init__(self, add=None, average=None, avg=None, collect=None, collect_set=None, count=None, count_distinct=None, count_distinct_approx=None, cumulative=None, cumulative_count=None, cumulative_sum=None, divide=None, implode=None, kurtosis=None, min=None, multiply=None, percentile_lookup=None, sample_standard_deviation=None, sample_stddev=None, skewness=None, standard_deviation=None, stddev=None, subtract=None, sum=None, variance=None):  # noqa: E501
+    def __init__(self, add=None, average=None, avg=None, collect=None, collect_set=None, count=None, count_distinct=None, count_distinct_approx=None, cumulative=None, cumulative_count=None, cumulative_sum=None, divide=None, implode=None, kurtosis=None, min=None, multiply=None, percentage=None, percentile_lookup=None, sample_standard_deviation=None, sample_stddev=None, skewness=None, standard_deviation=None, stddev=None, subtract=None, sum=None, variance=None):  # noqa: E501
         """AggregationTaskMetric - a model defined in OpenAPI"""  # noqa: E501
 
         self._add = None
         self._average = None
         self._avg = None
         self._collect = None
         self._collect_set = None
@@ -101,14 +103,15 @@
         self._cumulative_count = None
         self._cumulative_sum = None
         self._divide = None
         self._implode = None
         self._kurtosis = None
         self._min = None
         self._multiply = None
+        self._percentage = None
         self._percentile_lookup = None
         self._sample_standard_deviation = None
         self._sample_stddev = None
         self._skewness = None
         self._standard_deviation = None
         self._stddev = None
         self._subtract = None
@@ -144,14 +147,16 @@
             self.implode = implode
         if kurtosis is not None:
             self.kurtosis = kurtosis
         if min is not None:
             self.min = min
         if multiply is not None:
             self.multiply = multiply
+        if percentage is not None:
+            self.percentage = percentage
         if percentile_lookup is not None:
             self.percentile_lookup = percentile_lookup
         if sample_standard_deviation is not None:
             self.sample_standard_deviation = sample_standard_deviation
         if sample_stddev is not None:
             self.sample_stddev = sample_stddev
         if skewness is not None:
@@ -500,14 +505,35 @@
         :param multiply: The multiply of this AggregationTaskMetric.  # noqa: E501
         :type: MultiplyMetric
         """
 
         self._multiply = multiply
 
     @property
+    def percentage(self):
+        """Gets the percentage of this AggregationTaskMetric.  # noqa: E501
+
+
+        :return: The percentage of this AggregationTaskMetric.  # noqa: E501
+        :rtype: PercentageMetric
+        """
+        return self._percentage
+
+    @percentage.setter
+    def percentage(self, percentage):
+        """Sets the percentage of this AggregationTaskMetric.
+
+
+        :param percentage: The percentage of this AggregationTaskMetric.  # noqa: E501
+        :type: PercentageMetric
+        """
+
+        self._percentage = percentage
+
+    @property
     def percentile_lookup(self):
         """Gets the percentile_lookup of this AggregationTaskMetric.  # noqa: E501
 
 
         :return: The percentile_lookup of this AggregationTaskMetric.  # noqa: E501
         :rtype: PercentileLookupMetric
         """
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/api_user.py` & `nucleus_client-0.9.0/nucleus_client/models/api_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/array_explode_many_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/array_explode_many_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/array_explode_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/array_explode_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/array_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/array_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/base_page.py` & `nucleus_client-0.9.0/nucleus_client/models/base_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,22 +29,24 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'id': 'str',
         'block_order': 'list[str]',
+        'block_order_by_width': 'dict(str, object)',
         'client_id': 'str',
         'colors': 'dict(str, object)',
         'data_table_mode': 'str',
         'dt_u': 'datetime',
         'editor_properties': 'dict(str, object)',
         'filter_excludes': 'list[str]',
         'filter_mode': 'str',
         'filters': 'list[Filter]',
+        'options': 'Options',
         'page_template_id': 'str',
         'page_template_slug': 'str',
         'publication_properties': 'PagePublications',
         'section_title': 'str',
         'section_title_template': 'list[dict(str, object)]',
         'slug': 'str',
         'sub_nav': 'SubNav',
@@ -53,48 +55,52 @@
         'use_druid': 'bool',
         'user_id': 'str'
     }
 
     attribute_map = {
         'id': '_id',
         'block_order': 'block_order',
+        'block_order_by_width': 'block_order_by_width',
         'client_id': 'client_id',
         'colors': 'colors',
         'data_table_mode': 'data_table_mode',
         'dt_u': 'dt_u',
         'editor_properties': 'editor_properties',
         'filter_excludes': 'filter_excludes',
         'filter_mode': 'filter_mode',
         'filters': 'filters',
+        'options': 'options',
         'page_template_id': 'page_template_id',
         'page_template_slug': 'page_template_slug',
         'publication_properties': 'publication_properties',
         'section_title': 'section_title',
         'section_title_template': 'section_title_template',
         'slug': 'slug',
         'sub_nav': 'sub_nav',
         'title': 'title',
         'title_template': 'title_template',
         'use_druid': 'use_druid',
         'user_id': 'user_id'
     }
 
-    def __init__(self, id=None, block_order=None, client_id=None, colors=None, data_table_mode=None, dt_u=None, editor_properties=None, filter_excludes=None, filter_mode=None, filters=None, page_template_id=None, page_template_slug=None, publication_properties=None, section_title=None, section_title_template=None, slug=None, sub_nav=None, title=None, title_template=None, use_druid=None, user_id=None):  # noqa: E501
+    def __init__(self, id=None, block_order=None, block_order_by_width=None, client_id=None, colors=None, data_table_mode=None, dt_u=None, editor_properties=None, filter_excludes=None, filter_mode=None, filters=None, options=None, page_template_id=None, page_template_slug=None, publication_properties=None, section_title=None, section_title_template=None, slug=None, sub_nav=None, title=None, title_template=None, use_druid=None, user_id=None):  # noqa: E501
         """BasePage - a model defined in OpenAPI"""  # noqa: E501
 
         self._id = None
         self._block_order = None
+        self._block_order_by_width = None
         self._client_id = None
         self._colors = None
         self._data_table_mode = None
         self._dt_u = None
         self._editor_properties = None
         self._filter_excludes = None
         self._filter_mode = None
         self._filters = None
+        self._options = None
         self._page_template_id = None
         self._page_template_slug = None
         self._publication_properties = None
         self._section_title = None
         self._section_title_template = None
         self._slug = None
         self._sub_nav = None
@@ -104,14 +110,16 @@
         self._user_id = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if block_order is not None:
             self.block_order = block_order
+        if block_order_by_width is not None:
+            self.block_order_by_width = block_order_by_width
         self.client_id = client_id
         if colors is not None:
             self.colors = colors
         if data_table_mode is not None:
             self.data_table_mode = data_table_mode
         if dt_u is not None:
             self.dt_u = dt_u
@@ -119,14 +127,16 @@
             self.editor_properties = editor_properties
         if filter_excludes is not None:
             self.filter_excludes = filter_excludes
         if filter_mode is not None:
             self.filter_mode = filter_mode
         if filters is not None:
             self.filters = filters
+        if options is not None:
+            self.options = options
         if page_template_id is not None:
             self.page_template_id = page_template_id
         if page_template_slug is not None:
             self.page_template_slug = page_template_slug
         if publication_properties is not None:
             self.publication_properties = publication_properties
         if section_title is not None:
@@ -183,14 +193,35 @@
         :param block_order: The block_order of this BasePage.  # noqa: E501
         :type: list[str]
         """
 
         self._block_order = block_order
 
     @property
+    def block_order_by_width(self):
+        """Gets the block_order_by_width of this BasePage.  # noqa: E501
+
+
+        :return: The block_order_by_width of this BasePage.  # noqa: E501
+        :rtype: dict(str, object)
+        """
+        return self._block_order_by_width
+
+    @block_order_by_width.setter
+    def block_order_by_width(self, block_order_by_width):
+        """Sets the block_order_by_width of this BasePage.
+
+
+        :param block_order_by_width: The block_order_by_width of this BasePage.  # noqa: E501
+        :type: dict(str, object)
+        """
+
+        self._block_order_by_width = block_order_by_width
+
+    @property
     def client_id(self):
         """Gets the client_id of this BasePage.  # noqa: E501
 
 
         :return: The client_id of this BasePage.  # noqa: E501
         :rtype: str
         """
@@ -353,14 +384,35 @@
         :param filters: The filters of this BasePage.  # noqa: E501
         :type: list[Filter]
         """
 
         self._filters = filters
 
     @property
+    def options(self):
+        """Gets the options of this BasePage.  # noqa: E501
+
+
+        :return: The options of this BasePage.  # noqa: E501
+        :rtype: Options
+        """
+        return self._options
+
+    @options.setter
+    def options(self, options):
+        """Sets the options of this BasePage.
+
+
+        :param options: The options of this BasePage.  # noqa: E501
+        :type: Options
+        """
+
+        self._options = options
+
+    @property
     def page_template_id(self):
         """Gets the page_template_id of this BasePage.  # noqa: E501
 
 
         :return: The page_template_id of this BasePage.  # noqa: E501
         :rtype: str
         """
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/base_templated_page.py` & `nucleus_client-0.9.0/nucleus_client/models/base_templated_page.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/base_user.py` & `nucleus_client-0.9.0/nucleus_client/models/base_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/batch_receipt.py` & `nucleus_client-0.9.0/nucleus_client/models/batch_receipt.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/binomial_logistic_regression_task.py` & `nucleus_client-0.9.0/nucleus_client/models/binomial_logistic_regression_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/block.py` & `nucleus_client-0.9.0/nucleus_client/models/block.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/block_full.py` & `nucleus_client-0.9.0/nucleus_client/models/block_full.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/block_type.py` & `nucleus_client-0.9.0/nucleus_client/models/block_type.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/boolean_bucket_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/boolean_bucket_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/boolean_bucket_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/boolean_bucket_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/boolean_cast_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/boolean_cast_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/boolean_constant_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/boolean_constant_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/boolean_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/boolean_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/boolean_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/boolean_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/client.py` & `nucleus_client-0.9.0/nucleus_client/models/client.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/client_features.py` & `nucleus_client-0.9.0/nucleus_client/models/client_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,45 +27,50 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'dataset_upload': 'bool',
         'default_login_policy': 'str',
         'default_user_id': 'str',
         'default_user_token': 'str',
         'glossary': 'bool',
         'page_editor': 'bool',
         'sso': 'bool',
         'user_roles': 'bool'
     }
 
     attribute_map = {
+        'dataset_upload': 'dataset_upload',
         'default_login_policy': 'default_login_policy',
         'default_user_id': 'default_user_id',
         'default_user_token': 'default_user_token',
         'glossary': 'glossary',
         'page_editor': 'page_editor',
         'sso': 'sso',
         'user_roles': 'user_roles'
     }
 
-    def __init__(self, default_login_policy=None, default_user_id=None, default_user_token=None, glossary=None, page_editor=None, sso=None, user_roles=None):  # noqa: E501
+    def __init__(self, dataset_upload=None, default_login_policy=None, default_user_id=None, default_user_token=None, glossary=None, page_editor=None, sso=None, user_roles=None):  # noqa: E501
         """ClientFeatures - a model defined in OpenAPI"""  # noqa: E501
 
+        self._dataset_upload = None
         self._default_login_policy = None
         self._default_user_id = None
         self._default_user_token = None
         self._glossary = None
         self._page_editor = None
         self._sso = None
         self._user_roles = None
         self.discriminator = None
 
+        if dataset_upload is not None:
+            self.dataset_upload = dataset_upload
         if default_login_policy is not None:
             self.default_login_policy = default_login_policy
         if default_user_id is not None:
             self.default_user_id = default_user_id
         if default_user_token is not None:
             self.default_user_token = default_user_token
         if glossary is not None:
@@ -74,14 +79,35 @@
             self.page_editor = page_editor
         if sso is not None:
             self.sso = sso
         if user_roles is not None:
             self.user_roles = user_roles
 
     @property
+    def dataset_upload(self):
+        """Gets the dataset_upload of this ClientFeatures.  # noqa: E501
+
+
+        :return: The dataset_upload of this ClientFeatures.  # noqa: E501
+        :rtype: bool
+        """
+        return self._dataset_upload
+
+    @dataset_upload.setter
+    def dataset_upload(self, dataset_upload):
+        """Sets the dataset_upload of this ClientFeatures.
+
+
+        :param dataset_upload: The dataset_upload of this ClientFeatures.  # noqa: E501
+        :type: bool
+        """
+
+        self._dataset_upload = dataset_upload
+
+    @property
     def default_login_policy(self):
         """Gets the default_login_policy of this ClientFeatures.  # noqa: E501
 
 
         :return: The default_login_policy of this ClientFeatures.  # noqa: E501
         :rtype: str
         """
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/client_package.py` & `nucleus_client-0.9.0/nucleus_client/models/client_package.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/client_settings.py` & `nucleus_client-0.9.0/nucleus_client/models/refresh_schedule.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,143 +12,144 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class ClientSettings(object):
+class RefreshSchedule(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'id': 'str',
-        'colors': 'dict(str, object)',
-        'dataset_metadata': 'dict(str, object)',
-        'field_metadata': 'dict(str, object)'
+        'interval': 'RefreshInterval',
+        'run_time': 'RefreshInterval',
+        'start_date': 'datetime',
+        'state': 'RefreshState'
     }
 
     attribute_map = {
-        'id': '_id',
-        'colors': 'colors',
-        'dataset_metadata': 'dataset_metadata',
-        'field_metadata': 'field_metadata'
+        'interval': 'interval',
+        'run_time': 'run_time',
+        'start_date': 'start_date',
+        'state': 'state'
     }
 
-    def __init__(self, id=None, colors=None, dataset_metadata=None, field_metadata=None):  # noqa: E501
-        """ClientSettings - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, interval=None, run_time=None, start_date=None, state=None):  # noqa: E501
+        """RefreshSchedule - a model defined in OpenAPI"""  # noqa: E501
 
-        self._id = None
-        self._colors = None
-        self._dataset_metadata = None
-        self._field_metadata = None
+        self._interval = None
+        self._run_time = None
+        self._start_date = None
+        self._state = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
-        if colors is not None:
-            self.colors = colors
-        if dataset_metadata is not None:
-            self.dataset_metadata = dataset_metadata
-        if field_metadata is not None:
-            self.field_metadata = field_metadata
+        self.interval = interval
+        if run_time is not None:
+            self.run_time = run_time
+        if start_date is not None:
+            self.start_date = start_date
+        if state is not None:
+            self.state = state
 
     @property
-    def id(self):
-        """Gets the id of this ClientSettings.  # noqa: E501
+    def interval(self):
+        """Gets the interval of this RefreshSchedule.  # noqa: E501
 
 
-        :return: The id of this ClientSettings.  # noqa: E501
-        :rtype: str
+        :return: The interval of this RefreshSchedule.  # noqa: E501
+        :rtype: RefreshInterval
         """
-        return self._id
+        return self._interval
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this ClientSettings.
+    @interval.setter
+    def interval(self, interval):
+        """Sets the interval of this RefreshSchedule.
 
 
-        :param id: The id of this ClientSettings.  # noqa: E501
-        :type: str
+        :param interval: The interval of this RefreshSchedule.  # noqa: E501
+        :type: RefreshInterval
         """
+        if interval is None:
+            raise ValueError("Invalid value for `interval`, must not be `None`")  # noqa: E501
 
-        self._id = id
+        self._interval = interval
 
     @property
-    def colors(self):
-        """Gets the colors of this ClientSettings.  # noqa: E501
+    def run_time(self):
+        """Gets the run_time of this RefreshSchedule.  # noqa: E501
 
 
-        :return: The colors of this ClientSettings.  # noqa: E501
-        :rtype: dict(str, object)
+        :return: The run_time of this RefreshSchedule.  # noqa: E501
+        :rtype: RefreshInterval
         """
-        return self._colors
+        return self._run_time
 
-    @colors.setter
-    def colors(self, colors):
-        """Sets the colors of this ClientSettings.
+    @run_time.setter
+    def run_time(self, run_time):
+        """Sets the run_time of this RefreshSchedule.
 
 
-        :param colors: The colors of this ClientSettings.  # noqa: E501
-        :type: dict(str, object)
+        :param run_time: The run_time of this RefreshSchedule.  # noqa: E501
+        :type: RefreshInterval
         """
 
-        self._colors = colors
+        self._run_time = run_time
 
     @property
-    def dataset_metadata(self):
-        """Gets the dataset_metadata of this ClientSettings.  # noqa: E501
+    def start_date(self):
+        """Gets the start_date of this RefreshSchedule.  # noqa: E501
 
 
-        :return: The dataset_metadata of this ClientSettings.  # noqa: E501
-        :rtype: dict(str, object)
+        :return: The start_date of this RefreshSchedule.  # noqa: E501
+        :rtype: datetime
         """
-        return self._dataset_metadata
+        return self._start_date
 
-    @dataset_metadata.setter
-    def dataset_metadata(self, dataset_metadata):
-        """Sets the dataset_metadata of this ClientSettings.
+    @start_date.setter
+    def start_date(self, start_date):
+        """Sets the start_date of this RefreshSchedule.
 
 
-        :param dataset_metadata: The dataset_metadata of this ClientSettings.  # noqa: E501
-        :type: dict(str, object)
+        :param start_date: The start_date of this RefreshSchedule.  # noqa: E501
+        :type: datetime
         """
 
-        self._dataset_metadata = dataset_metadata
+        self._start_date = start_date
 
     @property
-    def field_metadata(self):
-        """Gets the field_metadata of this ClientSettings.  # noqa: E501
+    def state(self):
+        """Gets the state of this RefreshSchedule.  # noqa: E501
 
 
-        :return: The field_metadata of this ClientSettings.  # noqa: E501
-        :rtype: dict(str, object)
+        :return: The state of this RefreshSchedule.  # noqa: E501
+        :rtype: RefreshState
         """
-        return self._field_metadata
+        return self._state
 
-    @field_metadata.setter
-    def field_metadata(self, field_metadata):
-        """Sets the field_metadata of this ClientSettings.
+    @state.setter
+    def state(self, state):
+        """Sets the state of this RefreshSchedule.
 
 
-        :param field_metadata: The field_metadata of this ClientSettings.  # noqa: E501
-        :type: dict(str, object)
+        :param state: The state of this RefreshSchedule.  # noqa: E501
+        :type: RefreshState
         """
 
-        self._field_metadata = field_metadata
+        self._state = state
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -176,15 +177,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ClientSettings):
+        if not isinstance(other, RefreshSchedule):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/client_settings_update.py` & `nucleus_client-0.9.0/nucleus_client/models/client_settings_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/client_sso.py` & `nucleus_client-0.9.0/nucleus_client/models/client_sso.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/client_update.py` & `nucleus_client-0.9.0/nucleus_client/models/client_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/coalesce_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/coalesce_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/collection_size_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/collection_size_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/column_mapping.py` & `nucleus_client-0.9.0/nucleus_client/models/column_mapping.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/count_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/count_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/create_custom_dataset_task.py` & `nucleus_client-0.9.0/nucleus_client/models/create_custom_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/cumulative_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/cumulative_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/cumulative_metric_order_by.py` & `nucleus_client-0.9.0/nucleus_client/models/cumulative_metric_order_by.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/cumulative_sum_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/cumulative_sum_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_selector.py` & `nucleus_client-0.9.0/nucleus_client/models/data_selector.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,17 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'all_dimensions': 'bool',
+        'all_fields': 'bool',
         'client_id': 'str',
+        'columns': 'list[str]',
         'dataset': 'str',
         'dimensions': 'list[DataViewDimension]',
         'filters': 'list[DataViewFilter]',
         'granularity': 'str',
         'include_goals': 'bool',
         'intervals': 'list[str]',
         'limit': 'int',
@@ -46,15 +48,17 @@
         'query_type': 'str',
         'sort': 'list[DataViewSort]',
         'unique_limit': 'list[DataViewUniqueLimit]'
     }
 
     attribute_map = {
         'all_dimensions': 'all_dimensions',
+        'all_fields': 'all_fields',
         'client_id': 'client_id',
+        'columns': 'columns',
         'dataset': 'dataset',
         'dimensions': 'dimensions',
         'filters': 'filters',
         'granularity': 'granularity',
         'include_goals': 'include_goals',
         'intervals': 'intervals',
         'limit': 'limit',
@@ -62,19 +66,21 @@
         'metrics': 'metrics',
         'mode': 'mode',
         'query_type': 'query_type',
         'sort': 'sort',
         'unique_limit': 'unique_limit'
     }
 
-    def __init__(self, all_dimensions=None, client_id=None, dataset=None, dimensions=None, filters=None, granularity=None, include_goals=None, intervals=None, limit=None, lookups=None, metrics=None, mode=None, query_type=None, sort=None, unique_limit=None):  # noqa: E501
+    def __init__(self, all_dimensions=None, all_fields=None, client_id=None, columns=None, dataset=None, dimensions=None, filters=None, granularity=None, include_goals=None, intervals=None, limit=None, lookups=None, metrics=None, mode=None, query_type=None, sort=None, unique_limit=None):  # noqa: E501
         """DataView - a model defined in OpenAPI"""  # noqa: E501
 
         self._all_dimensions = None
+        self._all_fields = None
         self._client_id = None
+        self._columns = None
         self._dataset = None
         self._dimensions = None
         self._filters = None
         self._granularity = None
         self._include_goals = None
         self._intervals = None
         self._limit = None
@@ -84,30 +90,36 @@
         self._query_type = None
         self._sort = None
         self._unique_limit = None
         self.discriminator = None
 
         if all_dimensions is not None:
             self.all_dimensions = all_dimensions
+        if all_fields is not None:
+            self.all_fields = all_fields
         self.client_id = client_id
+        if columns is not None:
+            self.columns = columns
         self.dataset = dataset
-        self.dimensions = dimensions
+        if dimensions is not None:
+            self.dimensions = dimensions
         if filters is not None:
             self.filters = filters
         if granularity is not None:
             self.granularity = granularity
         if include_goals is not None:
             self.include_goals = include_goals
         if intervals is not None:
             self.intervals = intervals
         if limit is not None:
             self.limit = limit
         if lookups is not None:
             self.lookups = lookups
-        self.metrics = metrics
+        if metrics is not None:
+            self.metrics = metrics
         if mode is not None:
             self.mode = mode
         if query_type is not None:
             self.query_type = query_type
         if sort is not None:
             self.sort = sort
         if unique_limit is not None:
@@ -131,14 +143,35 @@
         :param all_dimensions: The all_dimensions of this DataView.  # noqa: E501
         :type: bool
         """
 
         self._all_dimensions = all_dimensions
 
     @property
+    def all_fields(self):
+        """Gets the all_fields of this DataView.  # noqa: E501
+
+
+        :return: The all_fields of this DataView.  # noqa: E501
+        :rtype: bool
+        """
+        return self._all_fields
+
+    @all_fields.setter
+    def all_fields(self, all_fields):
+        """Sets the all_fields of this DataView.
+
+
+        :param all_fields: The all_fields of this DataView.  # noqa: E501
+        :type: bool
+        """
+
+        self._all_fields = all_fields
+
+    @property
     def client_id(self):
         """Gets the client_id of this DataView.  # noqa: E501
 
 
         :return: The client_id of this DataView.  # noqa: E501
         :rtype: str
         """
@@ -154,14 +187,35 @@
         """
         if client_id is None:
             raise ValueError("Invalid value for `client_id`, must not be `None`")  # noqa: E501
 
         self._client_id = client_id
 
     @property
+    def columns(self):
+        """Gets the columns of this DataView.  # noqa: E501
+
+
+        :return: The columns of this DataView.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._columns
+
+    @columns.setter
+    def columns(self, columns):
+        """Sets the columns of this DataView.
+
+
+        :param columns: The columns of this DataView.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._columns = columns
+
+    @property
     def dataset(self):
         """Gets the dataset of this DataView.  # noqa: E501
 
 
         :return: The dataset of this DataView.  # noqa: E501
         :rtype: str
         """
@@ -194,16 +248,14 @@
     def dimensions(self, dimensions):
         """Sets the dimensions of this DataView.
 
 
         :param dimensions: The dimensions of this DataView.  # noqa: E501
         :type: list[DataViewDimension]
         """
-        if dimensions is None:
-            raise ValueError("Invalid value for `dimensions`, must not be `None`")  # noqa: E501
 
         self._dimensions = dimensions
 
     @property
     def filters(self):
         """Gets the filters of this DataView.  # noqa: E501
 
@@ -343,16 +395,14 @@
     def metrics(self, metrics):
         """Sets the metrics of this DataView.
 
 
         :param metrics: The metrics of this DataView.  # noqa: E501
         :type: list[DataViewMetric]
         """
-        if metrics is None:
-            raise ValueError("Invalid value for `metrics`, must not be `None`")  # noqa: E501
 
         self._metrics = metrics
 
     @property
     def mode(self):
         """Gets the mode of this DataView.  # noqa: E501
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_base.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_base.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_dimension.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_dimension.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_filter_value.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_filter_value.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_interval.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_interval.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_lookup.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_lookup.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/percentile_lookup_metric.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,198 +12,148 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class DataViewMetric(object):
+class PercentileLookupMetric(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'calc': 'DataViewMetricCalc',
         'column': 'str',
         'exclude_column': 'str',
         'output_column': 'str',
-        'selector_columns': 'list[str]',
-        'type': 'str'
+        'selector_columns': 'list[str]'
     }
 
     attribute_map = {
-        'calc': 'calc',
         'column': 'column',
         'exclude_column': 'exclude_column',
         'output_column': 'output_column',
-        'selector_columns': 'selector_columns',
-        'type': 'type'
+        'selector_columns': 'selector_columns'
     }
 
-    def __init__(self, calc=None, column=None, exclude_column=None, output_column=None, selector_columns=None, type=None):  # noqa: E501
-        """DataViewMetric - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, column=None, exclude_column=None, output_column=None, selector_columns=None):  # noqa: E501
+        """PercentileLookupMetric - a model defined in OpenAPI"""  # noqa: E501
 
-        self._calc = None
         self._column = None
         self._exclude_column = None
         self._output_column = None
         self._selector_columns = None
-        self._type = None
         self.discriminator = None
 
-        if calc is not None:
-            self.calc = calc
-        if column is not None:
-            self.column = column
-        if exclude_column is not None:
-            self.exclude_column = exclude_column
+        self.column = column
+        self.exclude_column = exclude_column
         self.output_column = output_column
-        if selector_columns is not None:
-            self.selector_columns = selector_columns
-        self.type = type
-
-    @property
-    def calc(self):
-        """Gets the calc of this DataViewMetric.  # noqa: E501
-
-
-        :return: The calc of this DataViewMetric.  # noqa: E501
-        :rtype: DataViewMetricCalc
-        """
-        return self._calc
-
-    @calc.setter
-    def calc(self, calc):
-        """Sets the calc of this DataViewMetric.
-
-
-        :param calc: The calc of this DataViewMetric.  # noqa: E501
-        :type: DataViewMetricCalc
-        """
-
-        self._calc = calc
+        self.selector_columns = selector_columns
 
     @property
     def column(self):
-        """Gets the column of this DataViewMetric.  # noqa: E501
+        """Gets the column of this PercentileLookupMetric.  # noqa: E501
 
 
-        :return: The column of this DataViewMetric.  # noqa: E501
+        :return: The column of this PercentileLookupMetric.  # noqa: E501
         :rtype: str
         """
         return self._column
 
     @column.setter
     def column(self, column):
-        """Sets the column of this DataViewMetric.
+        """Sets the column of this PercentileLookupMetric.
 
 
-        :param column: The column of this DataViewMetric.  # noqa: E501
+        :param column: The column of this PercentileLookupMetric.  # noqa: E501
         :type: str
         """
+        if column is None:
+            raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
 
         self._column = column
 
     @property
     def exclude_column(self):
-        """Gets the exclude_column of this DataViewMetric.  # noqa: E501
+        """Gets the exclude_column of this PercentileLookupMetric.  # noqa: E501
 
 
-        :return: The exclude_column of this DataViewMetric.  # noqa: E501
+        :return: The exclude_column of this PercentileLookupMetric.  # noqa: E501
         :rtype: str
         """
         return self._exclude_column
 
     @exclude_column.setter
     def exclude_column(self, exclude_column):
-        """Sets the exclude_column of this DataViewMetric.
+        """Sets the exclude_column of this PercentileLookupMetric.
 
 
-        :param exclude_column: The exclude_column of this DataViewMetric.  # noqa: E501
+        :param exclude_column: The exclude_column of this PercentileLookupMetric.  # noqa: E501
         :type: str
         """
+        if exclude_column is None:
+            raise ValueError("Invalid value for `exclude_column`, must not be `None`")  # noqa: E501
 
         self._exclude_column = exclude_column
 
     @property
     def output_column(self):
-        """Gets the output_column of this DataViewMetric.  # noqa: E501
+        """Gets the output_column of this PercentileLookupMetric.  # noqa: E501
 
 
-        :return: The output_column of this DataViewMetric.  # noqa: E501
+        :return: The output_column of this PercentileLookupMetric.  # noqa: E501
         :rtype: str
         """
         return self._output_column
 
     @output_column.setter
     def output_column(self, output_column):
-        """Sets the output_column of this DataViewMetric.
+        """Sets the output_column of this PercentileLookupMetric.
 
 
-        :param output_column: The output_column of this DataViewMetric.  # noqa: E501
+        :param output_column: The output_column of this PercentileLookupMetric.  # noqa: E501
         :type: str
         """
         if output_column is None:
             raise ValueError("Invalid value for `output_column`, must not be `None`")  # noqa: E501
 
         self._output_column = output_column
 
     @property
     def selector_columns(self):
-        """Gets the selector_columns of this DataViewMetric.  # noqa: E501
+        """Gets the selector_columns of this PercentileLookupMetric.  # noqa: E501
 
 
-        :return: The selector_columns of this DataViewMetric.  # noqa: E501
+        :return: The selector_columns of this PercentileLookupMetric.  # noqa: E501
         :rtype: list[str]
         """
         return self._selector_columns
 
     @selector_columns.setter
     def selector_columns(self, selector_columns):
-        """Sets the selector_columns of this DataViewMetric.
+        """Sets the selector_columns of this PercentileLookupMetric.
 
 
-        :param selector_columns: The selector_columns of this DataViewMetric.  # noqa: E501
+        :param selector_columns: The selector_columns of this PercentileLookupMetric.  # noqa: E501
         :type: list[str]
         """
+        if selector_columns is None:
+            raise ValueError("Invalid value for `selector_columns`, must not be `None`")  # noqa: E501
 
         self._selector_columns = selector_columns
 
-    @property
-    def type(self):
-        """Gets the type of this DataViewMetric.  # noqa: E501
-
-
-        :return: The type of this DataViewMetric.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this DataViewMetric.
-
-
-        :param type: The type of this DataViewMetric.  # noqa: E501
-        :type: str
-        """
-        if type is None:
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-
-        self._type = type
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -230,15 +180,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DataViewMetric):
+        if not isinstance(other, PercentileLookupMetric):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_metric_calc.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_metric_calc.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_metric_order_by.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_metric_order_by.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_mode.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_mode.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_period_to_date.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_period_to_date.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_sort.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_sort.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/data_view_unique_limit.py` & `nucleus_client-0.9.0/nucleus_client/models/data_view_unique_limit.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/dataset.py` & `nucleus_client-0.9.0/nucleus_client/models/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,47 +38,50 @@
         'dt_recalculated': 'datetime',
         'dt_u': 'datetime',
         'error': 'DatasetError',
         'hash_key': 'str',
         'name': 'str',
         'schedule': 'RefreshSchedule',
         'settings': 'dict(str, object)',
-        'slug': 'str'
+        'slug': 'str',
+        'upload_id': 'str'
     }
 
     attribute_map = {
         'id': '_id',
         'client_id': 'client_id',
         'dataset_type': 'dataset_type',
         'description': 'description',
         'dt_recalculated': 'dt_recalculated',
         'dt_u': 'dt_u',
         'error': 'error',
         'hash_key': 'hash_key',
         'name': 'name',
         'schedule': 'schedule',
         'settings': 'settings',
-        'slug': 'slug'
+        'slug': 'slug',
+        'upload_id': 'upload_id'
     }
 
-    def __init__(self, id=None, client_id=None, dataset_type=None, description=None, dt_recalculated=None, dt_u=None, error=None, hash_key=None, name=None, schedule=None, settings=None, slug=None):  # noqa: E501
+    def __init__(self, id=None, client_id=None, dataset_type=None, description=None, dt_recalculated=None, dt_u=None, error=None, hash_key=None, name=None, schedule=None, settings=None, slug=None, upload_id=None):  # noqa: E501
         """Dataset - a model defined in OpenAPI"""  # noqa: E501
 
         self._id = None
         self._client_id = None
         self._dataset_type = None
         self._description = None
         self._dt_recalculated = None
         self._dt_u = None
         self._error = None
         self._hash_key = None
         self._name = None
         self._schedule = None
         self._settings = None
         self._slug = None
+        self._upload_id = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         self.client_id = client_id
         self.dataset_type = dataset_type
         if description is not None:
@@ -93,14 +96,16 @@
             self.hash_key = hash_key
         self.name = name
         if schedule is not None:
             self.schedule = schedule
         self.settings = settings
         if slug is not None:
             self.slug = slug
+        if upload_id is not None:
+            self.upload_id = upload_id
 
     @property
     def id(self):
         """Gets the id of this Dataset.  # noqa: E501
 
 
         :return: The id of this Dataset.  # noqa: E501
@@ -354,14 +359,35 @@
 
         :param slug: The slug of this Dataset.  # noqa: E501
         :type: str
         """
 
         self._slug = slug
 
+    @property
+    def upload_id(self):
+        """Gets the upload_id of this Dataset.  # noqa: E501
+
+
+        :return: The upload_id of this Dataset.  # noqa: E501
+        :rtype: str
+        """
+        return self._upload_id
+
+    @upload_id.setter
+    def upload_id(self, upload_id):
+        """Sets the upload_id of this Dataset.
+
+
+        :param upload_id: The upload_id of this Dataset.  # noqa: E501
+        :type: str
+        """
+
+        self._upload_id = upload_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/dataset_error.py` & `nucleus_client-0.9.0/nucleus_client/models/dataset_error.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/dataset_metadata.py` & `nucleus_client-0.9.0/nucleus_client/models/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/dataset_update.py` & `nucleus_client-0.9.0/nucleus_client/models/dataset_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/date_dimension.py` & `nucleus_client-0.9.0/nucleus_client/models/date_dimension.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/date_time_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/date_time_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/date_time_filter_component.py` & `nucleus_client-0.9.0/nucleus_client/models/date_time_filter_component.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_constant_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_constant_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_current_date_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_current_date_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_current_timestamp_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_current_timestamp_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_diff_from_column_date_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_diff_from_column_date_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_diff_from_now_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_diff_from_now_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_diff_from_static_date_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_diff_from_static_date_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_diff_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_diff_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_format_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_format_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_offset_column_value_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_offset_column_value_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_offset_static_value_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_offset_static_value_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_offset_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_offset_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_range_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_range_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_select_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_select_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/datetime_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/datetime_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/dimension.py` & `nucleus_client-0.9.0/nucleus_client/models/dimension.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/divide_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/divide_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/download.py` & `nucleus_client-0.9.0/nucleus_client/models/download.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/download_error.py` & `nucleus_client-0.9.0/nucleus_client/models/download_error.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/download_v1.py` & `nucleus_client-0.9.0/nucleus_client/models/download_v1.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/download_v2.py` & `nucleus_client-0.9.0/nucleus_client/models/download_v2.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/drop_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/drop_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/druid_write_config.py` & `nucleus_client-0.9.0/nucleus_client/models/druid_write_config.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/entity_batch.py` & `nucleus_client-0.9.0/nucleus_client/models/entity_batch.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/entity_batch_health.py` & `nucleus_client-0.9.0/nucleus_client/models/entity_batch_health.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/filter.py` & `nucleus_client-0.9.0/nucleus_client/models/filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/filter_map.py` & `nucleus_client-0.9.0/nucleus_client/models/filter_map.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/filter_preset.py` & `nucleus_client-0.9.0/nucleus_client/models/filter_preset.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/geo_data.py` & `nucleus_client-0.9.0/nucleus_client/models/geo_data.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/goal.py` & `nucleus_client-0.9.0/nucleus_client/models/goal.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/goal_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/goal_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/individual_data_selector.py` & `nucleus_client-0.9.0/nucleus_client/models/individual_data_selector.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/integration.py` & `nucleus_client-0.9.0/nucleus_client/models/integration.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/integration_batch_history_receipt.py` & `nucleus_client-0.9.0/nucleus_client/models/integration_batch_history_receipt.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/integration_dataset.py` & `nucleus_client-0.9.0/nucleus_client/models/integration_dataset.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/integration_sync_history_receipt.py` & `nucleus_client-0.9.0/nucleus_client/models/integration_sync_history_receipt.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/integration_type.py` & `nucleus_client-0.9.0/nucleus_client/models/integration_type.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/integration_type_update.py` & `nucleus_client-0.9.0/nucleus_client/models/integration_type_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/integration_update.py` & `nucleus_client-0.9.0/nucleus_client/models/integration_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/job.py` & `nucleus_client-0.9.0/nucleus_client/models/job.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/job_overview.py` & `nucleus_client-0.9.0/nucleus_client/models/job_overview.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/join.py` & `nucleus_client-0.9.0/nucleus_client/models/join.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/join_relationship.py` & `nucleus_client-0.9.0/nucleus_client/models/join_relationship.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/loader_settings.py` & `nucleus_client-0.9.0/nucleus_client/models/loader_settings.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/map_explode_many_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/map_explode_many_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/map_explode_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/map_explode_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/map_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/map_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/multiply_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/multiply_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/new_user_token.py` & `nucleus_client-0.9.0/nucleus_client/models/new_user_token.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/non_null_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/non_null_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/normal_user.py` & `nucleus_client-0.9.0/nucleus_client/models/normal_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/notify_user.py` & `nucleus_client-0.9.0/nucleus_client/models/notify_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_binary_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/number_binary_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_binary_value_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/number_binary_value_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_bucket_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/number_bucket_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_bucket_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/number_bucket_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_cast_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/number_cast_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_constant_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/number_constant_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_default_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/number_default_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/number_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/number_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/number_unary_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/number_unary_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/or_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/or_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/page.py` & `nucleus_client-0.9.0/nucleus_client/models/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,23 +29,25 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'id': 'str',
         'block_order': 'list[str]',
+        'block_order_by_width': 'dict(str, object)',
         'blocks': 'dict(str, object)',
         'client_id': 'str',
         'colors': 'dict(str, object)',
         'data_table_mode': 'str',
         'dt_u': 'datetime',
         'editor_properties': 'dict(str, object)',
         'filter_excludes': 'list[str]',
         'filter_mode': 'str',
         'filters': 'list[Filter]',
+        'options': 'Options',
         'page_template_id': 'str',
         'page_template_slug': 'str',
         'publication_properties': 'PagePublications',
         'section_title': 'str',
         'section_title_template': 'list[dict(str, object)]',
         'slug': 'str',
         'sub_nav': 'SubNav',
@@ -56,23 +58,25 @@
         'views': 'dict(str, object)',
         'widgets': 'dict(str, object)'
     }
 
     attribute_map = {
         'id': '_id',
         'block_order': 'block_order',
+        'block_order_by_width': 'block_order_by_width',
         'blocks': 'blocks',
         'client_id': 'client_id',
         'colors': 'colors',
         'data_table_mode': 'data_table_mode',
         'dt_u': 'dt_u',
         'editor_properties': 'editor_properties',
         'filter_excludes': 'filter_excludes',
         'filter_mode': 'filter_mode',
         'filters': 'filters',
+        'options': 'options',
         'page_template_id': 'page_template_id',
         'page_template_slug': 'page_template_slug',
         'publication_properties': 'publication_properties',
         'section_title': 'section_title',
         'section_title_template': 'section_title_template',
         'slug': 'slug',
         'sub_nav': 'sub_nav',
@@ -80,28 +84,30 @@
         'title_template': 'title_template',
         'use_druid': 'use_druid',
         'user_id': 'user_id',
         'views': 'views',
         'widgets': 'widgets'
     }
 
-    def __init__(self, id=None, block_order=None, blocks=None, client_id=None, colors=None, data_table_mode=None, dt_u=None, editor_properties=None, filter_excludes=None, filter_mode=None, filters=None, page_template_id=None, page_template_slug=None, publication_properties=None, section_title=None, section_title_template=None, slug=None, sub_nav=None, title=None, title_template=None, use_druid=None, user_id=None, views=None, widgets=None):  # noqa: E501
+    def __init__(self, id=None, block_order=None, block_order_by_width=None, blocks=None, client_id=None, colors=None, data_table_mode=None, dt_u=None, editor_properties=None, filter_excludes=None, filter_mode=None, filters=None, options=None, page_template_id=None, page_template_slug=None, publication_properties=None, section_title=None, section_title_template=None, slug=None, sub_nav=None, title=None, title_template=None, use_druid=None, user_id=None, views=None, widgets=None):  # noqa: E501
         """Page - a model defined in OpenAPI"""  # noqa: E501
 
         self._id = None
         self._block_order = None
+        self._block_order_by_width = None
         self._blocks = None
         self._client_id = None
         self._colors = None
         self._data_table_mode = None
         self._dt_u = None
         self._editor_properties = None
         self._filter_excludes = None
         self._filter_mode = None
         self._filters = None
+        self._options = None
         self._page_template_id = None
         self._page_template_slug = None
         self._publication_properties = None
         self._section_title = None
         self._section_title_template = None
         self._slug = None
         self._sub_nav = None
@@ -113,14 +119,16 @@
         self._widgets = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if block_order is not None:
             self.block_order = block_order
+        if block_order_by_width is not None:
+            self.block_order_by_width = block_order_by_width
         if blocks is not None:
             self.blocks = blocks
         self.client_id = client_id
         if colors is not None:
             self.colors = colors
         if data_table_mode is not None:
             self.data_table_mode = data_table_mode
@@ -130,14 +138,16 @@
             self.editor_properties = editor_properties
         if filter_excludes is not None:
             self.filter_excludes = filter_excludes
         if filter_mode is not None:
             self.filter_mode = filter_mode
         if filters is not None:
             self.filters = filters
+        if options is not None:
+            self.options = options
         if page_template_id is not None:
             self.page_template_id = page_template_id
         if page_template_slug is not None:
             self.page_template_slug = page_template_slug
         if publication_properties is not None:
             self.publication_properties = publication_properties
         if section_title is not None:
@@ -198,14 +208,35 @@
         :param block_order: The block_order of this Page.  # noqa: E501
         :type: list[str]
         """
 
         self._block_order = block_order
 
     @property
+    def block_order_by_width(self):
+        """Gets the block_order_by_width of this Page.  # noqa: E501
+
+
+        :return: The block_order_by_width of this Page.  # noqa: E501
+        :rtype: dict(str, object)
+        """
+        return self._block_order_by_width
+
+    @block_order_by_width.setter
+    def block_order_by_width(self, block_order_by_width):
+        """Sets the block_order_by_width of this Page.
+
+
+        :param block_order_by_width: The block_order_by_width of this Page.  # noqa: E501
+        :type: dict(str, object)
+        """
+
+        self._block_order_by_width = block_order_by_width
+
+    @property
     def blocks(self):
         """Gets the blocks of this Page.  # noqa: E501
 
 
         :return: The blocks of this Page.  # noqa: E501
         :rtype: dict(str, object)
         """
@@ -389,14 +420,35 @@
         :param filters: The filters of this Page.  # noqa: E501
         :type: list[Filter]
         """
 
         self._filters = filters
 
     @property
+    def options(self):
+        """Gets the options of this Page.  # noqa: E501
+
+
+        :return: The options of this Page.  # noqa: E501
+        :rtype: Options
+        """
+        return self._options
+
+    @options.setter
+    def options(self, options):
+        """Sets the options of this Page.
+
+
+        :param options: The options of this Page.  # noqa: E501
+        :type: Options
+        """
+
+        self._options = options
+
+    @property
     def page_template_id(self):
         """Gets the page_template_id of this Page.  # noqa: E501
 
 
         :return: The page_template_id of this Page.  # noqa: E501
         :rtype: str
         """
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/page_filter_preferences.py` & `nucleus_client-0.9.0/nucleus_client/models/page_filter_preferences.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/page_full.py` & `nucleus_client-0.9.0/nucleus_client/models/page_full.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,25 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'id': 'str',
         'block_order': 'list[str]',
+        'block_order_by_width': 'dict(str, object)',
         'blocks': 'dict(str, object)',
         'client_id': 'str',
         'colors': 'dict(str, object)',
         'data_table_mode': 'str',
         'dt_u': 'datetime',
         'editor_properties': 'dict(str, object)',
         'filter_excludes': 'list[str]',
         'filter_mode': 'str',
         'filters': 'list[Filter]',
+        'options': 'Options',
         'page_template_id': 'str',
         'page_template_slug': 'str',
         'publication_properties': 'PagePublications',
         'section_title': 'str',
         'section_title_template': 'list[dict(str, object)]',
         'slug': 'str',
         'sub_nav': 'SubNav',
@@ -56,23 +58,25 @@
         'views': 'dict(str, object)',
         'widgets': 'dict(str, object)'
     }
 
     attribute_map = {
         'id': '_id',
         'block_order': 'block_order',
+        'block_order_by_width': 'block_order_by_width',
         'blocks': 'blocks',
         'client_id': 'client_id',
         'colors': 'colors',
         'data_table_mode': 'data_table_mode',
         'dt_u': 'dt_u',
         'editor_properties': 'editor_properties',
         'filter_excludes': 'filter_excludes',
         'filter_mode': 'filter_mode',
         'filters': 'filters',
+        'options': 'options',
         'page_template_id': 'page_template_id',
         'page_template_slug': 'page_template_slug',
         'publication_properties': 'publication_properties',
         'section_title': 'section_title',
         'section_title_template': 'section_title_template',
         'slug': 'slug',
         'sub_nav': 'sub_nav',
@@ -80,28 +84,30 @@
         'title_template': 'title_template',
         'use_druid': 'use_druid',
         'user_id': 'user_id',
         'views': 'views',
         'widgets': 'widgets'
     }
 
-    def __init__(self, id=None, block_order=None, blocks=None, client_id=None, colors=None, data_table_mode=None, dt_u=None, editor_properties=None, filter_excludes=None, filter_mode=None, filters=None, page_template_id=None, page_template_slug=None, publication_properties=None, section_title=None, section_title_template=None, slug=None, sub_nav=None, title=None, title_template=None, use_druid=None, user_id=None, views=None, widgets=None):  # noqa: E501
+    def __init__(self, id=None, block_order=None, block_order_by_width=None, blocks=None, client_id=None, colors=None, data_table_mode=None, dt_u=None, editor_properties=None, filter_excludes=None, filter_mode=None, filters=None, options=None, page_template_id=None, page_template_slug=None, publication_properties=None, section_title=None, section_title_template=None, slug=None, sub_nav=None, title=None, title_template=None, use_druid=None, user_id=None, views=None, widgets=None):  # noqa: E501
         """PageFull - a model defined in OpenAPI"""  # noqa: E501
 
         self._id = None
         self._block_order = None
+        self._block_order_by_width = None
         self._blocks = None
         self._client_id = None
         self._colors = None
         self._data_table_mode = None
         self._dt_u = None
         self._editor_properties = None
         self._filter_excludes = None
         self._filter_mode = None
         self._filters = None
+        self._options = None
         self._page_template_id = None
         self._page_template_slug = None
         self._publication_properties = None
         self._section_title = None
         self._section_title_template = None
         self._slug = None
         self._sub_nav = None
@@ -113,14 +119,16 @@
         self._widgets = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if block_order is not None:
             self.block_order = block_order
+        if block_order_by_width is not None:
+            self.block_order_by_width = block_order_by_width
         if blocks is not None:
             self.blocks = blocks
         self.client_id = client_id
         if colors is not None:
             self.colors = colors
         if data_table_mode is not None:
             self.data_table_mode = data_table_mode
@@ -130,14 +138,16 @@
             self.editor_properties = editor_properties
         if filter_excludes is not None:
             self.filter_excludes = filter_excludes
         if filter_mode is not None:
             self.filter_mode = filter_mode
         if filters is not None:
             self.filters = filters
+        if options is not None:
+            self.options = options
         if page_template_id is not None:
             self.page_template_id = page_template_id
         if page_template_slug is not None:
             self.page_template_slug = page_template_slug
         if publication_properties is not None:
             self.publication_properties = publication_properties
         if section_title is not None:
@@ -198,14 +208,35 @@
         :param block_order: The block_order of this PageFull.  # noqa: E501
         :type: list[str]
         """
 
         self._block_order = block_order
 
     @property
+    def block_order_by_width(self):
+        """Gets the block_order_by_width of this PageFull.  # noqa: E501
+
+
+        :return: The block_order_by_width of this PageFull.  # noqa: E501
+        :rtype: dict(str, object)
+        """
+        return self._block_order_by_width
+
+    @block_order_by_width.setter
+    def block_order_by_width(self, block_order_by_width):
+        """Sets the block_order_by_width of this PageFull.
+
+
+        :param block_order_by_width: The block_order_by_width of this PageFull.  # noqa: E501
+        :type: dict(str, object)
+        """
+
+        self._block_order_by_width = block_order_by_width
+
+    @property
     def blocks(self):
         """Gets the blocks of this PageFull.  # noqa: E501
 
 
         :return: The blocks of this PageFull.  # noqa: E501
         :rtype: dict(str, object)
         """
@@ -389,14 +420,35 @@
         :param filters: The filters of this PageFull.  # noqa: E501
         :type: list[Filter]
         """
 
         self._filters = filters
 
     @property
+    def options(self):
+        """Gets the options of this PageFull.  # noqa: E501
+
+
+        :return: The options of this PageFull.  # noqa: E501
+        :rtype: Options
+        """
+        return self._options
+
+    @options.setter
+    def options(self, options):
+        """Sets the options of this PageFull.
+
+
+        :param options: The options of this PageFull.  # noqa: E501
+        :type: Options
+        """
+
+        self._options = options
+
+    @property
     def page_template_id(self):
         """Gets the page_template_id of this PageFull.  # noqa: E501
 
 
         :return: The page_template_id of this PageFull.  # noqa: E501
         :rtype: str
         """
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/page_preferences.py` & `nucleus_client-0.9.0/nucleus_client/models/page_preferences.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/page_preferences_update.py` & `nucleus_client-0.9.0/nucleus_client/models/page_preferences_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/page_publications.py` & `nucleus_client-0.9.0/nucleus_client/models/page_publications.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/page_template.py` & `nucleus_client-0.9.0/nucleus_client/models/page_template.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/page_template_update.py` & `nucleus_client-0.9.0/nucleus_client/models/page_template_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/page_view.py` & `nucleus_client-0.9.0/nucleus_client/models/page_view.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/partner_batch.py` & `nucleus_client-0.9.0/nucleus_client/models/partner_batch.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/partner_post_data.py` & `nucleus_client-0.9.0/nucleus_client/models/partner_post_data.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/password_change_request.py` & `nucleus_client-0.9.0/nucleus_client/models/password_change_request.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/password_reset_change.py` & `nucleus_client-0.9.0/nucleus_client/models/password_reset_change.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/password_reset_request.py` & `nucleus_client-0.9.0/nucleus_client/models/password_reset_request.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/percentile_lookup_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/percentage_metric.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class PercentileLookupMetric(object):
+class PercentageMetric(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,129 +30,128 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'column': 'str',
         'exclude_column': 'str',
         'output_column': 'str',
-        'selector_columns': 'list[str]'
+        'population_dataset': 'str'
     }
 
     attribute_map = {
         'column': 'column',
         'exclude_column': 'exclude_column',
         'output_column': 'output_column',
-        'selector_columns': 'selector_columns'
+        'population_dataset': 'population_dataset'
     }
 
-    def __init__(self, column=None, exclude_column=None, output_column=None, selector_columns=None):  # noqa: E501
-        """PercentileLookupMetric - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, column=None, exclude_column=None, output_column=None, population_dataset=None):  # noqa: E501
+        """PercentageMetric - a model defined in OpenAPI"""  # noqa: E501
 
         self._column = None
         self._exclude_column = None
         self._output_column = None
-        self._selector_columns = None
+        self._population_dataset = None
         self.discriminator = None
 
         self.column = column
-        self.exclude_column = exclude_column
+        if exclude_column is not None:
+            self.exclude_column = exclude_column
         self.output_column = output_column
-        self.selector_columns = selector_columns
+        self.population_dataset = population_dataset
 
     @property
     def column(self):
-        """Gets the column of this PercentileLookupMetric.  # noqa: E501
+        """Gets the column of this PercentageMetric.  # noqa: E501
 
 
-        :return: The column of this PercentileLookupMetric.  # noqa: E501
+        :return: The column of this PercentageMetric.  # noqa: E501
         :rtype: str
         """
         return self._column
 
     @column.setter
     def column(self, column):
-        """Sets the column of this PercentileLookupMetric.
+        """Sets the column of this PercentageMetric.
 
 
-        :param column: The column of this PercentileLookupMetric.  # noqa: E501
+        :param column: The column of this PercentageMetric.  # noqa: E501
         :type: str
         """
         if column is None:
             raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
 
         self._column = column
 
     @property
     def exclude_column(self):
-        """Gets the exclude_column of this PercentileLookupMetric.  # noqa: E501
+        """Gets the exclude_column of this PercentageMetric.  # noqa: E501
 
 
-        :return: The exclude_column of this PercentileLookupMetric.  # noqa: E501
+        :return: The exclude_column of this PercentageMetric.  # noqa: E501
         :rtype: str
         """
         return self._exclude_column
 
     @exclude_column.setter
     def exclude_column(self, exclude_column):
-        """Sets the exclude_column of this PercentileLookupMetric.
+        """Sets the exclude_column of this PercentageMetric.
 
 
-        :param exclude_column: The exclude_column of this PercentileLookupMetric.  # noqa: E501
+        :param exclude_column: The exclude_column of this PercentageMetric.  # noqa: E501
         :type: str
         """
-        if exclude_column is None:
-            raise ValueError("Invalid value for `exclude_column`, must not be `None`")  # noqa: E501
 
         self._exclude_column = exclude_column
 
     @property
     def output_column(self):
-        """Gets the output_column of this PercentileLookupMetric.  # noqa: E501
+        """Gets the output_column of this PercentageMetric.  # noqa: E501
 
 
-        :return: The output_column of this PercentileLookupMetric.  # noqa: E501
+        :return: The output_column of this PercentageMetric.  # noqa: E501
         :rtype: str
         """
         return self._output_column
 
     @output_column.setter
     def output_column(self, output_column):
-        """Sets the output_column of this PercentileLookupMetric.
+        """Sets the output_column of this PercentageMetric.
 
 
-        :param output_column: The output_column of this PercentileLookupMetric.  # noqa: E501
+        :param output_column: The output_column of this PercentageMetric.  # noqa: E501
         :type: str
         """
         if output_column is None:
             raise ValueError("Invalid value for `output_column`, must not be `None`")  # noqa: E501
 
         self._output_column = output_column
 
     @property
-    def selector_columns(self):
-        """Gets the selector_columns of this PercentileLookupMetric.  # noqa: E501
+    def population_dataset(self):
+        """Gets the population_dataset of this PercentageMetric.  # noqa: E501
 
 
-        :return: The selector_columns of this PercentileLookupMetric.  # noqa: E501
-        :rtype: list[str]
+        :return: The population_dataset of this PercentageMetric.  # noqa: E501
+        :rtype: str
         """
-        return self._selector_columns
+        return self._population_dataset
 
-    @selector_columns.setter
-    def selector_columns(self, selector_columns):
-        """Sets the selector_columns of this PercentileLookupMetric.
+    @population_dataset.setter
+    def population_dataset(self, population_dataset):
+        """Sets the population_dataset of this PercentageMetric.
 
 
-        :param selector_columns: The selector_columns of this PercentileLookupMetric.  # noqa: E501
-        :type: list[str]
+        :param population_dataset: The population_dataset of this PercentageMetric.  # noqa: E501
+        :type: str
         """
-        if selector_columns is None:
-            raise ValueError("Invalid value for `selector_columns`, must not be `None`")  # noqa: E501
+        if population_dataset is None:
+            raise ValueError("Invalid value for `population_dataset`, must not be `None`")  # noqa: E501
 
-        self._selector_columns = selector_columns
+        self._population_dataset = population_dataset
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -180,15 +179,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PercentileLookupMetric):
+        if not isinstance(other, PercentageMetric):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/post_data.py` & `nucleus_client-0.9.0/nucleus_client/models/post_data.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/refresh_interval.py` & `nucleus_client-0.9.0/nucleus_client/models/refresh_interval.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/refresh_schedule.py` & `nucleus_client-0.9.0/nucleus_client/models/schema_field.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,118 +12,144 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class RefreshSchedule(object):
+class SchemaField(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'interval': 'RefreshInterval',
-        'start_date': 'datetime',
-        'state': 'RefreshState'
+        'metadata': 'SchemaFieldMetadata',
+        'name': 'str',
+        'nullable': 'bool',
+        'type': 'str'
     }
 
     attribute_map = {
-        'interval': 'interval',
-        'start_date': 'start_date',
-        'state': 'state'
+        'metadata': 'metadata',
+        'name': 'name',
+        'nullable': 'nullable',
+        'type': 'type'
     }
 
-    def __init__(self, interval=None, start_date=None, state=None):  # noqa: E501
-        """RefreshSchedule - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, metadata=None, name=None, nullable=None, type=None):  # noqa: E501
+        """SchemaField - a model defined in OpenAPI"""  # noqa: E501
 
-        self._interval = None
-        self._start_date = None
-        self._state = None
+        self._metadata = None
+        self._name = None
+        self._nullable = None
+        self._type = None
         self.discriminator = None
 
-        self.interval = interval
-        if start_date is not None:
-            self.start_date = start_date
-        if state is not None:
-            self.state = state
+        if metadata is not None:
+            self.metadata = metadata
+        if name is not None:
+            self.name = name
+        self.nullable = nullable
+        if type is not None:
+            self.type = type
 
     @property
-    def interval(self):
-        """Gets the interval of this RefreshSchedule.  # noqa: E501
+    def metadata(self):
+        """Gets the metadata of this SchemaField.  # noqa: E501
 
 
-        :return: The interval of this RefreshSchedule.  # noqa: E501
-        :rtype: RefreshInterval
+        :return: The metadata of this SchemaField.  # noqa: E501
+        :rtype: SchemaFieldMetadata
         """
-        return self._interval
+        return self._metadata
 
-    @interval.setter
-    def interval(self, interval):
-        """Sets the interval of this RefreshSchedule.
+    @metadata.setter
+    def metadata(self, metadata):
+        """Sets the metadata of this SchemaField.
 
 
-        :param interval: The interval of this RefreshSchedule.  # noqa: E501
-        :type: RefreshInterval
+        :param metadata: The metadata of this SchemaField.  # noqa: E501
+        :type: SchemaFieldMetadata
         """
-        if interval is None:
-            raise ValueError("Invalid value for `interval`, must not be `None`")  # noqa: E501
 
-        self._interval = interval
+        self._metadata = metadata
 
     @property
-    def start_date(self):
-        """Gets the start_date of this RefreshSchedule.  # noqa: E501
+    def name(self):
+        """Gets the name of this SchemaField.  # noqa: E501
 
 
-        :return: The start_date of this RefreshSchedule.  # noqa: E501
-        :rtype: datetime
+        :return: The name of this SchemaField.  # noqa: E501
+        :rtype: str
         """
-        return self._start_date
+        return self._name
 
-    @start_date.setter
-    def start_date(self, start_date):
-        """Sets the start_date of this RefreshSchedule.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this SchemaField.
 
 
-        :param start_date: The start_date of this RefreshSchedule.  # noqa: E501
-        :type: datetime
+        :param name: The name of this SchemaField.  # noqa: E501
+        :type: str
         """
 
-        self._start_date = start_date
+        self._name = name
 
     @property
-    def state(self):
-        """Gets the state of this RefreshSchedule.  # noqa: E501
+    def nullable(self):
+        """Gets the nullable of this SchemaField.  # noqa: E501
 
 
-        :return: The state of this RefreshSchedule.  # noqa: E501
-        :rtype: RefreshState
+        :return: The nullable of this SchemaField.  # noqa: E501
+        :rtype: bool
         """
-        return self._state
+        return self._nullable
 
-    @state.setter
-    def state(self, state):
-        """Sets the state of this RefreshSchedule.
+    @nullable.setter
+    def nullable(self, nullable):
+        """Sets the nullable of this SchemaField.
 
 
-        :param state: The state of this RefreshSchedule.  # noqa: E501
-        :type: RefreshState
+        :param nullable: The nullable of this SchemaField.  # noqa: E501
+        :type: bool
         """
+        if nullable is None:
+            raise ValueError("Invalid value for `nullable`, must not be `None`")  # noqa: E501
 
-        self._state = state
+        self._nullable = nullable
+
+    @property
+    def type(self):
+        """Gets the type of this SchemaField.  # noqa: E501
+
+
+        :return: The type of this SchemaField.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this SchemaField.
+
+
+        :param type: The type of this SchemaField.  # noqa: E501
+        :type: str
+        """
+
+        self._type = type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -151,15 +177,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RefreshSchedule):
+        if not isinstance(other, SchemaField):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/refresh_state.py` & `nucleus_client-0.9.0/nucleus_client/models/refresh_state.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/rename_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/rename_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/role.py` & `nucleus_client-0.9.0/nucleus_client/models/role.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/role_permission.py` & `nucleus_client-0.9.0/nucleus_client/models/role_permission.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/role_update.py` & `nucleus_client-0.9.0/nucleus_client/models/role_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/sarimax_dataset_task.py` & `nucleus_client-0.9.0/nucleus_client/models/sarimax_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/sarimax_task.py` & `nucleus_client-0.9.0/nucleus_client/models/sarimax_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/sarimax_task_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/sarimax_task_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/schema.py` & `nucleus_client-0.9.0/nucleus_client/models/schema.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/schema_field.py` & `nucleus_client-0.9.0/nucleus_client/models/string_casing_transform.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,142 +12,118 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class SchemaField(object):
+class StringCasingTransform(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'metadata': 'SchemaFieldMetadata',
-        'name': 'str',
-        'nullable': 'bool',
+        'column': 'str',
+        'output_column': 'str',
         'type': 'str'
     }
 
     attribute_map = {
-        'metadata': 'metadata',
-        'name': 'name',
-        'nullable': 'nullable',
+        'column': 'column',
+        'output_column': 'output_column',
         'type': 'type'
     }
 
-    def __init__(self, metadata=None, name=None, nullable=None, type=None):  # noqa: E501
-        """SchemaField - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, column=None, output_column=None, type=None):  # noqa: E501
+        """StringCasingTransform - a model defined in OpenAPI"""  # noqa: E501
 
-        self._metadata = None
-        self._name = None
-        self._nullable = None
+        self._column = None
+        self._output_column = None
         self._type = None
         self.discriminator = None
 
-        if metadata is not None:
-            self.metadata = metadata
-        if name is not None:
-            self.name = name
-        self.nullable = nullable
-        if type is not None:
-            self.type = type
+        self.column = column
+        self.output_column = output_column
+        self.type = type
 
     @property
-    def metadata(self):
-        """Gets the metadata of this SchemaField.  # noqa: E501
+    def column(self):
+        """Gets the column of this StringCasingTransform.  # noqa: E501
 
 
-        :return: The metadata of this SchemaField.  # noqa: E501
-        :rtype: SchemaFieldMetadata
-        """
-        return self._metadata
-
-    @metadata.setter
-    def metadata(self, metadata):
-        """Sets the metadata of this SchemaField.
-
-
-        :param metadata: The metadata of this SchemaField.  # noqa: E501
-        :type: SchemaFieldMetadata
-        """
-
-        self._metadata = metadata
-
-    @property
-    def name(self):
-        """Gets the name of this SchemaField.  # noqa: E501
-
-
-        :return: The name of this SchemaField.  # noqa: E501
+        :return: The column of this StringCasingTransform.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._column
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this SchemaField.
+    @column.setter
+    def column(self, column):
+        """Sets the column of this StringCasingTransform.
 
 
-        :param name: The name of this SchemaField.  # noqa: E501
+        :param column: The column of this StringCasingTransform.  # noqa: E501
         :type: str
         """
+        if column is None:
+            raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._column = column
 
     @property
-    def nullable(self):
-        """Gets the nullable of this SchemaField.  # noqa: E501
+    def output_column(self):
+        """Gets the output_column of this StringCasingTransform.  # noqa: E501
 
 
-        :return: The nullable of this SchemaField.  # noqa: E501
-        :rtype: bool
+        :return: The output_column of this StringCasingTransform.  # noqa: E501
+        :rtype: str
         """
-        return self._nullable
+        return self._output_column
 
-    @nullable.setter
-    def nullable(self, nullable):
-        """Sets the nullable of this SchemaField.
+    @output_column.setter
+    def output_column(self, output_column):
+        """Sets the output_column of this StringCasingTransform.
 
 
-        :param nullable: The nullable of this SchemaField.  # noqa: E501
-        :type: bool
+        :param output_column: The output_column of this StringCasingTransform.  # noqa: E501
+        :type: str
         """
-        if nullable is None:
-            raise ValueError("Invalid value for `nullable`, must not be `None`")  # noqa: E501
+        if output_column is None:
+            raise ValueError("Invalid value for `output_column`, must not be `None`")  # noqa: E501
 
-        self._nullable = nullable
+        self._output_column = output_column
 
     @property
     def type(self):
-        """Gets the type of this SchemaField.  # noqa: E501
+        """Gets the type of this StringCasingTransform.  # noqa: E501
 
 
-        :return: The type of this SchemaField.  # noqa: E501
+        :return: The type of this StringCasingTransform.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this SchemaField.
+        """Sets the type of this StringCasingTransform.
 
 
-        :param type: The type of this SchemaField.  # noqa: E501
+        :param type: The type of this StringCasingTransform.  # noqa: E501
         :type: str
         """
+        if type is None:
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
         self._type = type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -177,15 +153,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SchemaField):
+        if not isinstance(other, StringCasingTransform):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/schema_field_metadata.py` & `nucleus_client-0.9.0/nucleus_client/models/schema_field_metadata.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/schema_schema.py` & `nucleus_client-0.9.0/nucleus_client/models/schema_schema.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/settings_spec.py` & `nucleus_client-0.9.0/nucleus_client/models/settings_spec.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/snapshot_dataset_task.py` & `nucleus_client-0.9.0/nucleus_client/models/snapshot_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/sort.py` & `nucleus_client-0.9.0/nucleus_client/models/sort.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_bucket_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/string_bucket_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_bucket_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_bucket_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_casing_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_to_datetime_transform.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class StringCasingTransform(object):
+class StringToDatetimeTransform(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -28,104 +28,104 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'column': 'str',
-        'output_column': 'str',
-        'type': 'str'
+        'format': 'str',
+        'output_column': 'str'
     }
 
     attribute_map = {
         'column': 'column',
-        'output_column': 'output_column',
-        'type': 'type'
+        'format': 'format',
+        'output_column': 'output_column'
     }
 
-    def __init__(self, column=None, output_column=None, type=None):  # noqa: E501
-        """StringCasingTransform - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, column=None, format=None, output_column=None):  # noqa: E501
+        """StringToDatetimeTransform - a model defined in OpenAPI"""  # noqa: E501
 
         self._column = None
+        self._format = None
         self._output_column = None
-        self._type = None
         self.discriminator = None
 
         self.column = column
+        self.format = format
         self.output_column = output_column
-        self.type = type
 
     @property
     def column(self):
-        """Gets the column of this StringCasingTransform.  # noqa: E501
+        """Gets the column of this StringToDatetimeTransform.  # noqa: E501
 
 
-        :return: The column of this StringCasingTransform.  # noqa: E501
+        :return: The column of this StringToDatetimeTransform.  # noqa: E501
         :rtype: str
         """
         return self._column
 
     @column.setter
     def column(self, column):
-        """Sets the column of this StringCasingTransform.
+        """Sets the column of this StringToDatetimeTransform.
 
 
-        :param column: The column of this StringCasingTransform.  # noqa: E501
+        :param column: The column of this StringToDatetimeTransform.  # noqa: E501
         :type: str
         """
         if column is None:
             raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
 
         self._column = column
 
     @property
-    def output_column(self):
-        """Gets the output_column of this StringCasingTransform.  # noqa: E501
+    def format(self):
+        """Gets the format of this StringToDatetimeTransform.  # noqa: E501
 
 
-        :return: The output_column of this StringCasingTransform.  # noqa: E501
+        :return: The format of this StringToDatetimeTransform.  # noqa: E501
         :rtype: str
         """
-        return self._output_column
+        return self._format
 
-    @output_column.setter
-    def output_column(self, output_column):
-        """Sets the output_column of this StringCasingTransform.
+    @format.setter
+    def format(self, format):
+        """Sets the format of this StringToDatetimeTransform.
 
 
-        :param output_column: The output_column of this StringCasingTransform.  # noqa: E501
+        :param format: The format of this StringToDatetimeTransform.  # noqa: E501
         :type: str
         """
-        if output_column is None:
-            raise ValueError("Invalid value for `output_column`, must not be `None`")  # noqa: E501
+        if format is None:
+            raise ValueError("Invalid value for `format`, must not be `None`")  # noqa: E501
 
-        self._output_column = output_column
+        self._format = format
 
     @property
-    def type(self):
-        """Gets the type of this StringCasingTransform.  # noqa: E501
+    def output_column(self):
+        """Gets the output_column of this StringToDatetimeTransform.  # noqa: E501
 
 
-        :return: The type of this StringCasingTransform.  # noqa: E501
+        :return: The output_column of this StringToDatetimeTransform.  # noqa: E501
         :rtype: str
         """
-        return self._type
+        return self._output_column
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this StringCasingTransform.
+    @output_column.setter
+    def output_column(self, output_column):
+        """Sets the output_column of this StringToDatetimeTransform.
 
 
-        :param type: The type of this StringCasingTransform.  # noqa: E501
+        :param output_column: The output_column of this StringToDatetimeTransform.  # noqa: E501
         :type: str
         """
-        if type is None:
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if output_column is None:
+            raise ValueError("Invalid value for `output_column`, must not be `None`")  # noqa: E501
 
-        self._type = type
+        self._output_column = output_column
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -153,15 +153,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StringCasingTransform):
+        if not isinstance(other, StringToDatetimeTransform):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_constant_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_constant_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_default_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_default_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_distance_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_distance_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_extract_url_component_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_extract_url_component_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_filter.py` & `nucleus_client-0.9.0/nucleus_client/models/string_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_format_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_format_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_lookup_state_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_lookup_state_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_regexp_extract_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_regexp_extract_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_regexp_replace_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_regexp_replace_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_soundex_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_soundex_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_split_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_split_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_substring_index_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_substring_index_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_substring_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_substring_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_to_datetime_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_growth_rate_metric.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class StringToDatetimeTransform(object):
+class TimeStepGrowthRateMetric(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -28,98 +28,98 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'column': 'str',
-        'format': 'str',
+        'operation': 'str',
         'output_column': 'str'
     }
 
     attribute_map = {
         'column': 'column',
-        'format': 'format',
+        'operation': 'operation',
         'output_column': 'output_column'
     }
 
-    def __init__(self, column=None, format=None, output_column=None):  # noqa: E501
-        """StringToDatetimeTransform - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, column=None, operation=None, output_column=None):  # noqa: E501
+        """TimeStepGrowthRateMetric - a model defined in OpenAPI"""  # noqa: E501
 
         self._column = None
-        self._format = None
+        self._operation = None
         self._output_column = None
         self.discriminator = None
 
         self.column = column
-        self.format = format
+        self.operation = operation
         self.output_column = output_column
 
     @property
     def column(self):
-        """Gets the column of this StringToDatetimeTransform.  # noqa: E501
+        """Gets the column of this TimeStepGrowthRateMetric.  # noqa: E501
 
 
-        :return: The column of this StringToDatetimeTransform.  # noqa: E501
+        :return: The column of this TimeStepGrowthRateMetric.  # noqa: E501
         :rtype: str
         """
         return self._column
 
     @column.setter
     def column(self, column):
-        """Sets the column of this StringToDatetimeTransform.
+        """Sets the column of this TimeStepGrowthRateMetric.
 
 
-        :param column: The column of this StringToDatetimeTransform.  # noqa: E501
+        :param column: The column of this TimeStepGrowthRateMetric.  # noqa: E501
         :type: str
         """
         if column is None:
             raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
 
         self._column = column
 
     @property
-    def format(self):
-        """Gets the format of this StringToDatetimeTransform.  # noqa: E501
+    def operation(self):
+        """Gets the operation of this TimeStepGrowthRateMetric.  # noqa: E501
 
 
-        :return: The format of this StringToDatetimeTransform.  # noqa: E501
+        :return: The operation of this TimeStepGrowthRateMetric.  # noqa: E501
         :rtype: str
         """
-        return self._format
+        return self._operation
 
-    @format.setter
-    def format(self, format):
-        """Sets the format of this StringToDatetimeTransform.
+    @operation.setter
+    def operation(self, operation):
+        """Sets the operation of this TimeStepGrowthRateMetric.
 
 
-        :param format: The format of this StringToDatetimeTransform.  # noqa: E501
+        :param operation: The operation of this TimeStepGrowthRateMetric.  # noqa: E501
         :type: str
         """
-        if format is None:
-            raise ValueError("Invalid value for `format`, must not be `None`")  # noqa: E501
+        if operation is None:
+            raise ValueError("Invalid value for `operation`, must not be `None`")  # noqa: E501
 
-        self._format = format
+        self._operation = operation
 
     @property
     def output_column(self):
-        """Gets the output_column of this StringToDatetimeTransform.  # noqa: E501
+        """Gets the output_column of this TimeStepGrowthRateMetric.  # noqa: E501
 
 
-        :return: The output_column of this StringToDatetimeTransform.  # noqa: E501
+        :return: The output_column of this TimeStepGrowthRateMetric.  # noqa: E501
         :rtype: str
         """
         return self._output_column
 
     @output_column.setter
     def output_column(self, output_column):
-        """Sets the output_column of this StringToDatetimeTransform.
+        """Sets the output_column of this TimeStepGrowthRateMetric.
 
 
-        :param output_column: The output_column of this StringToDatetimeTransform.  # noqa: E501
+        :param output_column: The output_column of this TimeStepGrowthRateMetric.  # noqa: E501
         :type: str
         """
         if output_column is None:
             raise ValueError("Invalid value for `output_column`, must not be `None`")  # noqa: E501
 
         self._output_column = output_column
 
@@ -153,15 +153,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StringToDatetimeTransform):
+        if not isinstance(other, TimeStepGrowthRateMetric):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_to_num_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_to_num_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/string_trim_transform.py` & `nucleus_client-0.9.0/nucleus_client/models/string_trim_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/sub_nav.py` & `nucleus_client-0.9.0/nucleus_client/models/sub_nav.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/subtract_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/subtract_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/templated_page.py` & `nucleus_client-0.9.0/nucleus_client/models/templated_page.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/term.py` & `nucleus_client-0.9.0/nucleus_client/models/term.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_aggregation_dataset_task.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_aggregation_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_aggregation_task.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_aggregation_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_difference_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_difference_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_growth_rate_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/rename_transform2.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class TimeStepGrowthRateMetric(object):
+class RenameTransform2(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -28,98 +28,71 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'column': 'str',
-        'operation': 'str',
         'output_column': 'str'
     }
 
     attribute_map = {
         'column': 'column',
-        'operation': 'operation',
         'output_column': 'output_column'
     }
 
-    def __init__(self, column=None, operation=None, output_column=None):  # noqa: E501
-        """TimeStepGrowthRateMetric - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, column=None, output_column=None):  # noqa: E501
+        """RenameTransform2 - a model defined in OpenAPI"""  # noqa: E501
 
         self._column = None
-        self._operation = None
         self._output_column = None
         self.discriminator = None
 
         self.column = column
-        self.operation = operation
         self.output_column = output_column
 
     @property
     def column(self):
-        """Gets the column of this TimeStepGrowthRateMetric.  # noqa: E501
+        """Gets the column of this RenameTransform2.  # noqa: E501
 
 
-        :return: The column of this TimeStepGrowthRateMetric.  # noqa: E501
+        :return: The column of this RenameTransform2.  # noqa: E501
         :rtype: str
         """
         return self._column
 
     @column.setter
     def column(self, column):
-        """Sets the column of this TimeStepGrowthRateMetric.
+        """Sets the column of this RenameTransform2.
 
 
-        :param column: The column of this TimeStepGrowthRateMetric.  # noqa: E501
+        :param column: The column of this RenameTransform2.  # noqa: E501
         :type: str
         """
         if column is None:
             raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
 
         self._column = column
 
     @property
-    def operation(self):
-        """Gets the operation of this TimeStepGrowthRateMetric.  # noqa: E501
-
-
-        :return: The operation of this TimeStepGrowthRateMetric.  # noqa: E501
-        :rtype: str
-        """
-        return self._operation
-
-    @operation.setter
-    def operation(self, operation):
-        """Sets the operation of this TimeStepGrowthRateMetric.
-
-
-        :param operation: The operation of this TimeStepGrowthRateMetric.  # noqa: E501
-        :type: str
-        """
-        if operation is None:
-            raise ValueError("Invalid value for `operation`, must not be `None`")  # noqa: E501
-
-        self._operation = operation
-
-    @property
     def output_column(self):
-        """Gets the output_column of this TimeStepGrowthRateMetric.  # noqa: E501
+        """Gets the output_column of this RenameTransform2.  # noqa: E501
 
 
-        :return: The output_column of this TimeStepGrowthRateMetric.  # noqa: E501
+        :return: The output_column of this RenameTransform2.  # noqa: E501
         :rtype: str
         """
         return self._output_column
 
     @output_column.setter
     def output_column(self, output_column):
-        """Sets the output_column of this TimeStepGrowthRateMetric.
+        """Sets the output_column of this RenameTransform2.
 
 
-        :param output_column: The output_column of this TimeStepGrowthRateMetric.  # noqa: E501
+        :param output_column: The output_column of this RenameTransform2.  # noqa: E501
         :type: str
         """
         if output_column is None:
             raise ValueError("Invalid value for `output_column`, must not be `None`")  # noqa: E501
 
         self._output_column = output_column
 
@@ -153,15 +126,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TimeStepGrowthRateMetric):
+        if not isinstance(other, RenameTransform2):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_metric_dataset_task.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_metric_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_metric_task.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_metric_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_mode.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_mode.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_netforum_stats_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_netforum_stats_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/time_step_renewal_rate_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/time_step_renewal_rate_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/top_n_dataset_task.py` & `nucleus_client-0.9.0/nucleus_client/models/top_n_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/top_n_task.py` & `nucleus_client-0.9.0/nucleus_client/models/top_n_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/top_n_task_partition.py` & `nucleus_client-0.9.0/nucleus_client/models/top_n_task_partition.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/top_n_task_sort.py` & `nucleus_client-0.9.0/nucleus_client/models/top_n_task_sort.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/transform.py` & `nucleus_client-0.9.0/nucleus_client/models/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         'datetime': 'DatetimeTransform',
         'drop': 'DropTransform',
         'dt': 'DatetimeTransform',
         'map': 'MapTransform',
         'num': 'NumberTransform',
         'number': 'NumberTransform',
         'rename': 'RenameTransform',
+        'rename2': 'RenameTransform2',
         'str': 'StringTransform',
         'string': 'StringTransform'
     }
 
     attribute_map = {
         'array': 'array',
         'bool': 'bool',
@@ -54,32 +55,34 @@
         'datetime': 'datetime',
         'drop': 'drop',
         'dt': 'dt',
         'map': 'map',
         'num': 'num',
         'number': 'number',
         'rename': 'rename',
+        'rename2': 'rename2',
         'str': 'str',
         'string': 'string'
     }
 
-    def __init__(self, array=None, bool=None, boolean=None, coalesce=None, datetime=None, drop=None, dt=None, map=None, num=None, number=None, rename=None, str=None, string=None):  # noqa: E501
+    def __init__(self, array=None, bool=None, boolean=None, coalesce=None, datetime=None, drop=None, dt=None, map=None, num=None, number=None, rename=None, rename2=None, str=None, string=None):  # noqa: E501
         """Transform - a model defined in OpenAPI"""  # noqa: E501
 
         self._array = None
         self._bool = None
         self._boolean = None
         self._coalesce = None
         self._datetime = None
         self._drop = None
         self._dt = None
         self._map = None
         self._num = None
         self._number = None
         self._rename = None
+        self._rename2 = None
         self._str = None
         self._string = None
         self.discriminator = None
 
         if array is not None:
             self.array = array
         if bool is not None:
@@ -98,14 +101,16 @@
             self.map = map
         if num is not None:
             self.num = num
         if number is not None:
             self.number = number
         if rename is not None:
             self.rename = rename
+        if rename2 is not None:
+            self.rename2 = rename2
         if str is not None:
             self.str = str
         if string is not None:
             self.string = string
 
     @property
     def array(self):
@@ -335,14 +340,35 @@
         :param rename: The rename of this Transform.  # noqa: E501
         :type: RenameTransform
         """
 
         self._rename = rename
 
     @property
+    def rename2(self):
+        """Gets the rename2 of this Transform.  # noqa: E501
+
+
+        :return: The rename2 of this Transform.  # noqa: E501
+        :rtype: RenameTransform2
+        """
+        return self._rename2
+
+    @rename2.setter
+    def rename2(self, rename2):
+        """Sets the rename2 of this Transform.
+
+
+        :param rename2: The rename2 of this Transform.  # noqa: E501
+        :type: RenameTransform2
+        """
+
+        self._rename2 = rename2
+
+    @property
     def str(self):
         """Gets the str of this Transform.  # noqa: E501
 
 
         :return: The str of this Transform.  # noqa: E501
         :rtype: StringTransform
         """
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/unary_metric.py` & `nucleus_client-0.9.0/nucleus_client/models/unary_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/unique_limit.py` & `nucleus_client-0.9.0/nucleus_client/models/unique_limit.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/update_api_user.py` & `nucleus_client-0.9.0/nucleus_client/models/update_api_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/update_user.py` & `nucleus_client-0.9.0/nucleus_client/models/update_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/user_activation.py` & `nucleus_client-0.9.0/nucleus_client/models/user_activation.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/user_role.py` & `nucleus_client-0.9.0/nucleus_client/models/user_role.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/user_token.py` & `nucleus_client-0.9.0/nucleus_client/models/user_token.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/view.py` & `nucleus_client-0.9.0/nucleus_client/models/view.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/view_error.py` & `nucleus_client-0.9.0/nucleus_client/models/view_error.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/virtual_user.py` & `nucleus_client-0.9.0/nucleus_client/models/virtual_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/widget.py` & `nucleus_client-0.9.0/nucleus_client/models/widget_full.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class Widget(object):
+class WidgetFull(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -33,14 +33,15 @@
     openapi_types = {
         'id': 'str',
         'data_selectors': 'DataSelector',
         'dt_u': 'datetime',
         'filter_excludes': 'list[str]',
         'filter_map': 'list[FilterMap]',
         'label_map': 'dict(str, object)',
+        'links': 'Link',
         'settings': 'dict(str, object)',
         'sub_title': 'str',
         'sub_title_template': 'list[dict(str, object)]',
         'title': 'str',
         'title_template': 'list[dict(str, object)]',
         'view_hash_key': 'str',
         'view_transforms': 'list[dict(str, object)]',
@@ -50,55 +51,58 @@
     attribute_map = {
         'id': '_id',
         'data_selectors': 'data_selectors',
         'dt_u': 'dt_u',
         'filter_excludes': 'filter_excludes',
         'filter_map': 'filter_map',
         'label_map': 'label_map',
+        'links': 'links',
         'settings': 'settings',
         'sub_title': 'sub_title',
         'sub_title_template': 'sub_title_template',
         'title': 'title',
         'title_template': 'title_template',
         'view_hash_key': 'view_hash_key',
         'view_transforms': 'view_transforms',
         'widget_type_name': 'widget_type_name'
     }
 
-    def __init__(self, id=None, data_selectors=None, dt_u=None, filter_excludes=None, filter_map=None, label_map=None, settings=None, sub_title=None, sub_title_template=None, title=None, title_template=None, view_hash_key=None, view_transforms=None, widget_type_name=None):  # noqa: E501
-        """Widget - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, id=None, data_selectors=None, dt_u=None, filter_excludes=None, filter_map=None, label_map=None, links=None, settings=None, sub_title=None, sub_title_template=None, title=None, title_template=None, view_hash_key=None, view_transforms=None, widget_type_name=None):  # noqa: E501
+        """WidgetFull - a model defined in OpenAPI"""  # noqa: E501
 
         self._id = None
         self._data_selectors = None
         self._dt_u = None
         self._filter_excludes = None
         self._filter_map = None
         self._label_map = None
+        self._links = None
         self._settings = None
         self._sub_title = None
         self._sub_title_template = None
         self._title = None
         self._title_template = None
         self._view_hash_key = None
         self._view_transforms = None
         self._widget_type_name = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
+        self.id = id
         if data_selectors is not None:
             self.data_selectors = data_selectors
         if dt_u is not None:
             self.dt_u = dt_u
         if filter_excludes is not None:
             self.filter_excludes = filter_excludes
         if filter_map is not None:
             self.filter_map = filter_map
         if label_map is not None:
             self.label_map = label_map
+        if links is not None:
+            self.links = links
         if settings is not None:
             self.settings = settings
         if sub_title is not None:
             self.sub_title = sub_title
         if sub_title_template is not None:
             self.sub_title_template = sub_title_template
         self.title = title
@@ -107,305 +111,328 @@
         self.view_hash_key = view_hash_key
         if view_transforms is not None:
             self.view_transforms = view_transforms
         self.widget_type_name = widget_type_name
 
     @property
     def id(self):
-        """Gets the id of this Widget.  # noqa: E501
+        """Gets the id of this WidgetFull.  # noqa: E501
 
 
-        :return: The id of this Widget.  # noqa: E501
+        :return: The id of this WidgetFull.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this Widget.
+        """Sets the id of this WidgetFull.
 
 
-        :param id: The id of this Widget.  # noqa: E501
+        :param id: The id of this WidgetFull.  # noqa: E501
         :type: str
         """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def data_selectors(self):
-        """Gets the data_selectors of this Widget.  # noqa: E501
+        """Gets the data_selectors of this WidgetFull.  # noqa: E501
 
 
-        :return: The data_selectors of this Widget.  # noqa: E501
+        :return: The data_selectors of this WidgetFull.  # noqa: E501
         :rtype: DataSelector
         """
         return self._data_selectors
 
     @data_selectors.setter
     def data_selectors(self, data_selectors):
-        """Sets the data_selectors of this Widget.
+        """Sets the data_selectors of this WidgetFull.
 
 
-        :param data_selectors: The data_selectors of this Widget.  # noqa: E501
+        :param data_selectors: The data_selectors of this WidgetFull.  # noqa: E501
         :type: DataSelector
         """
 
         self._data_selectors = data_selectors
 
     @property
     def dt_u(self):
-        """Gets the dt_u of this Widget.  # noqa: E501
+        """Gets the dt_u of this WidgetFull.  # noqa: E501
 
 
-        :return: The dt_u of this Widget.  # noqa: E501
+        :return: The dt_u of this WidgetFull.  # noqa: E501
         :rtype: datetime
         """
         return self._dt_u
 
     @dt_u.setter
     def dt_u(self, dt_u):
-        """Sets the dt_u of this Widget.
+        """Sets the dt_u of this WidgetFull.
 
 
-        :param dt_u: The dt_u of this Widget.  # noqa: E501
+        :param dt_u: The dt_u of this WidgetFull.  # noqa: E501
         :type: datetime
         """
 
         self._dt_u = dt_u
 
     @property
     def filter_excludes(self):
-        """Gets the filter_excludes of this Widget.  # noqa: E501
+        """Gets the filter_excludes of this WidgetFull.  # noqa: E501
 
 
-        :return: The filter_excludes of this Widget.  # noqa: E501
+        :return: The filter_excludes of this WidgetFull.  # noqa: E501
         :rtype: list[str]
         """
         return self._filter_excludes
 
     @filter_excludes.setter
     def filter_excludes(self, filter_excludes):
-        """Sets the filter_excludes of this Widget.
+        """Sets the filter_excludes of this WidgetFull.
 
 
-        :param filter_excludes: The filter_excludes of this Widget.  # noqa: E501
+        :param filter_excludes: The filter_excludes of this WidgetFull.  # noqa: E501
         :type: list[str]
         """
 
         self._filter_excludes = filter_excludes
 
     @property
     def filter_map(self):
-        """Gets the filter_map of this Widget.  # noqa: E501
+        """Gets the filter_map of this WidgetFull.  # noqa: E501
 
 
-        :return: The filter_map of this Widget.  # noqa: E501
+        :return: The filter_map of this WidgetFull.  # noqa: E501
         :rtype: list[FilterMap]
         """
         return self._filter_map
 
     @filter_map.setter
     def filter_map(self, filter_map):
-        """Sets the filter_map of this Widget.
+        """Sets the filter_map of this WidgetFull.
 
 
-        :param filter_map: The filter_map of this Widget.  # noqa: E501
+        :param filter_map: The filter_map of this WidgetFull.  # noqa: E501
         :type: list[FilterMap]
         """
 
         self._filter_map = filter_map
 
     @property
     def label_map(self):
-        """Gets the label_map of this Widget.  # noqa: E501
+        """Gets the label_map of this WidgetFull.  # noqa: E501
 
 
-        :return: The label_map of this Widget.  # noqa: E501
+        :return: The label_map of this WidgetFull.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._label_map
 
     @label_map.setter
     def label_map(self, label_map):
-        """Sets the label_map of this Widget.
+        """Sets the label_map of this WidgetFull.
 
 
-        :param label_map: The label_map of this Widget.  # noqa: E501
+        :param label_map: The label_map of this WidgetFull.  # noqa: E501
         :type: dict(str, object)
         """
 
         self._label_map = label_map
 
     @property
+    def links(self):
+        """Gets the links of this WidgetFull.  # noqa: E501
+
+
+        :return: The links of this WidgetFull.  # noqa: E501
+        :rtype: Link
+        """
+        return self._links
+
+    @links.setter
+    def links(self, links):
+        """Sets the links of this WidgetFull.
+
+
+        :param links: The links of this WidgetFull.  # noqa: E501
+        :type: Link
+        """
+
+        self._links = links
+
+    @property
     def settings(self):
-        """Gets the settings of this Widget.  # noqa: E501
+        """Gets the settings of this WidgetFull.  # noqa: E501
 
 
-        :return: The settings of this Widget.  # noqa: E501
+        :return: The settings of this WidgetFull.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._settings
 
     @settings.setter
     def settings(self, settings):
-        """Sets the settings of this Widget.
+        """Sets the settings of this WidgetFull.
 
 
-        :param settings: The settings of this Widget.  # noqa: E501
+        :param settings: The settings of this WidgetFull.  # noqa: E501
         :type: dict(str, object)
         """
 
         self._settings = settings
 
     @property
     def sub_title(self):
-        """Gets the sub_title of this Widget.  # noqa: E501
+        """Gets the sub_title of this WidgetFull.  # noqa: E501
 
 
-        :return: The sub_title of this Widget.  # noqa: E501
+        :return: The sub_title of this WidgetFull.  # noqa: E501
         :rtype: str
         """
         return self._sub_title
 
     @sub_title.setter
     def sub_title(self, sub_title):
-        """Sets the sub_title of this Widget.
+        """Sets the sub_title of this WidgetFull.
 
 
-        :param sub_title: The sub_title of this Widget.  # noqa: E501
+        :param sub_title: The sub_title of this WidgetFull.  # noqa: E501
         :type: str
         """
 
         self._sub_title = sub_title
 
     @property
     def sub_title_template(self):
-        """Gets the sub_title_template of this Widget.  # noqa: E501
+        """Gets the sub_title_template of this WidgetFull.  # noqa: E501
 
 
-        :return: The sub_title_template of this Widget.  # noqa: E501
+        :return: The sub_title_template of this WidgetFull.  # noqa: E501
         :rtype: list[dict(str, object)]
         """
         return self._sub_title_template
 
     @sub_title_template.setter
     def sub_title_template(self, sub_title_template):
-        """Sets the sub_title_template of this Widget.
+        """Sets the sub_title_template of this WidgetFull.
 
 
-        :param sub_title_template: The sub_title_template of this Widget.  # noqa: E501
+        :param sub_title_template: The sub_title_template of this WidgetFull.  # noqa: E501
         :type: list[dict(str, object)]
         """
 
         self._sub_title_template = sub_title_template
 
     @property
     def title(self):
-        """Gets the title of this Widget.  # noqa: E501
+        """Gets the title of this WidgetFull.  # noqa: E501
 
 
-        :return: The title of this Widget.  # noqa: E501
+        :return: The title of this WidgetFull.  # noqa: E501
         :rtype: str
         """
         return self._title
 
     @title.setter
     def title(self, title):
-        """Sets the title of this Widget.
+        """Sets the title of this WidgetFull.
 
 
-        :param title: The title of this Widget.  # noqa: E501
+        :param title: The title of this WidgetFull.  # noqa: E501
         :type: str
         """
         if title is None:
             raise ValueError("Invalid value for `title`, must not be `None`")  # noqa: E501
 
         self._title = title
 
     @property
     def title_template(self):
-        """Gets the title_template of this Widget.  # noqa: E501
+        """Gets the title_template of this WidgetFull.  # noqa: E501
 
 
-        :return: The title_template of this Widget.  # noqa: E501
+        :return: The title_template of this WidgetFull.  # noqa: E501
         :rtype: list[dict(str, object)]
         """
         return self._title_template
 
     @title_template.setter
     def title_template(self, title_template):
-        """Sets the title_template of this Widget.
+        """Sets the title_template of this WidgetFull.
 
 
-        :param title_template: The title_template of this Widget.  # noqa: E501
+        :param title_template: The title_template of this WidgetFull.  # noqa: E501
         :type: list[dict(str, object)]
         """
 
         self._title_template = title_template
 
     @property
     def view_hash_key(self):
-        """Gets the view_hash_key of this Widget.  # noqa: E501
+        """Gets the view_hash_key of this WidgetFull.  # noqa: E501
 
 
-        :return: The view_hash_key of this Widget.  # noqa: E501
+        :return: The view_hash_key of this WidgetFull.  # noqa: E501
         :rtype: str
         """
         return self._view_hash_key
 
     @view_hash_key.setter
     def view_hash_key(self, view_hash_key):
-        """Sets the view_hash_key of this Widget.
+        """Sets the view_hash_key of this WidgetFull.
 
 
-        :param view_hash_key: The view_hash_key of this Widget.  # noqa: E501
+        :param view_hash_key: The view_hash_key of this WidgetFull.  # noqa: E501
         :type: str
         """
         if view_hash_key is None:
             raise ValueError("Invalid value for `view_hash_key`, must not be `None`")  # noqa: E501
 
         self._view_hash_key = view_hash_key
 
     @property
     def view_transforms(self):
-        """Gets the view_transforms of this Widget.  # noqa: E501
+        """Gets the view_transforms of this WidgetFull.  # noqa: E501
 
 
-        :return: The view_transforms of this Widget.  # noqa: E501
+        :return: The view_transforms of this WidgetFull.  # noqa: E501
         :rtype: list[dict(str, object)]
         """
         return self._view_transforms
 
     @view_transforms.setter
     def view_transforms(self, view_transforms):
-        """Sets the view_transforms of this Widget.
+        """Sets the view_transforms of this WidgetFull.
 
 
-        :param view_transforms: The view_transforms of this Widget.  # noqa: E501
+        :param view_transforms: The view_transforms of this WidgetFull.  # noqa: E501
         :type: list[dict(str, object)]
         """
 
         self._view_transforms = view_transforms
 
     @property
     def widget_type_name(self):
-        """Gets the widget_type_name of this Widget.  # noqa: E501
+        """Gets the widget_type_name of this WidgetFull.  # noqa: E501
 
 
-        :return: The widget_type_name of this Widget.  # noqa: E501
+        :return: The widget_type_name of this WidgetFull.  # noqa: E501
         :rtype: str
         """
         return self._widget_type_name
 
     @widget_type_name.setter
     def widget_type_name(self, widget_type_name):
-        """Sets the widget_type_name of this Widget.
+        """Sets the widget_type_name of this WidgetFull.
 
 
-        :param widget_type_name: The widget_type_name of this Widget.  # noqa: E501
+        :param widget_type_name: The widget_type_name of this WidgetFull.  # noqa: E501
         :type: str
         """
         if widget_type_name is None:
             raise ValueError("Invalid value for `widget_type_name`, must not be `None`")  # noqa: E501
 
         self._widget_type_name = widget_type_name
 
@@ -439,15 +466,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Widget):
+        if not isinstance(other, WidgetFull):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/widget_full.py` & `nucleus_client-0.9.0/nucleus_client/models/widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class WidgetFull(object):
+class Widget(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -33,14 +33,15 @@
     openapi_types = {
         'id': 'str',
         'data_selectors': 'DataSelector',
         'dt_u': 'datetime',
         'filter_excludes': 'list[str]',
         'filter_map': 'list[FilterMap]',
         'label_map': 'dict(str, object)',
+        'links': 'Link',
         'settings': 'dict(str, object)',
         'sub_title': 'str',
         'sub_title_template': 'list[dict(str, object)]',
         'title': 'str',
         'title_template': 'list[dict(str, object)]',
         'view_hash_key': 'str',
         'view_transforms': 'list[dict(str, object)]',
@@ -50,54 +51,59 @@
     attribute_map = {
         'id': '_id',
         'data_selectors': 'data_selectors',
         'dt_u': 'dt_u',
         'filter_excludes': 'filter_excludes',
         'filter_map': 'filter_map',
         'label_map': 'label_map',
+        'links': 'links',
         'settings': 'settings',
         'sub_title': 'sub_title',
         'sub_title_template': 'sub_title_template',
         'title': 'title',
         'title_template': 'title_template',
         'view_hash_key': 'view_hash_key',
         'view_transforms': 'view_transforms',
         'widget_type_name': 'widget_type_name'
     }
 
-    def __init__(self, id=None, data_selectors=None, dt_u=None, filter_excludes=None, filter_map=None, label_map=None, settings=None, sub_title=None, sub_title_template=None, title=None, title_template=None, view_hash_key=None, view_transforms=None, widget_type_name=None):  # noqa: E501
-        """WidgetFull - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, id=None, data_selectors=None, dt_u=None, filter_excludes=None, filter_map=None, label_map=None, links=None, settings=None, sub_title=None, sub_title_template=None, title=None, title_template=None, view_hash_key=None, view_transforms=None, widget_type_name=None):  # noqa: E501
+        """Widget - a model defined in OpenAPI"""  # noqa: E501
 
         self._id = None
         self._data_selectors = None
         self._dt_u = None
         self._filter_excludes = None
         self._filter_map = None
         self._label_map = None
+        self._links = None
         self._settings = None
         self._sub_title = None
         self._sub_title_template = None
         self._title = None
         self._title_template = None
         self._view_hash_key = None
         self._view_transforms = None
         self._widget_type_name = None
         self.discriminator = None
 
-        self.id = id
+        if id is not None:
+            self.id = id
         if data_selectors is not None:
             self.data_selectors = data_selectors
         if dt_u is not None:
             self.dt_u = dt_u
         if filter_excludes is not None:
             self.filter_excludes = filter_excludes
         if filter_map is not None:
             self.filter_map = filter_map
         if label_map is not None:
             self.label_map = label_map
+        if links is not None:
+            self.links = links
         if settings is not None:
             self.settings = settings
         if sub_title is not None:
             self.sub_title = sub_title
         if sub_title_template is not None:
             self.sub_title_template = sub_title_template
         self.title = title
@@ -106,307 +112,326 @@
         self.view_hash_key = view_hash_key
         if view_transforms is not None:
             self.view_transforms = view_transforms
         self.widget_type_name = widget_type_name
 
     @property
     def id(self):
-        """Gets the id of this WidgetFull.  # noqa: E501
+        """Gets the id of this Widget.  # noqa: E501
 
 
-        :return: The id of this WidgetFull.  # noqa: E501
+        :return: The id of this Widget.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this WidgetFull.
+        """Sets the id of this Widget.
 
 
-        :param id: The id of this WidgetFull.  # noqa: E501
+        :param id: The id of this Widget.  # noqa: E501
         :type: str
         """
-        if id is None:
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def data_selectors(self):
-        """Gets the data_selectors of this WidgetFull.  # noqa: E501
+        """Gets the data_selectors of this Widget.  # noqa: E501
 
 
-        :return: The data_selectors of this WidgetFull.  # noqa: E501
+        :return: The data_selectors of this Widget.  # noqa: E501
         :rtype: DataSelector
         """
         return self._data_selectors
 
     @data_selectors.setter
     def data_selectors(self, data_selectors):
-        """Sets the data_selectors of this WidgetFull.
+        """Sets the data_selectors of this Widget.
 
 
-        :param data_selectors: The data_selectors of this WidgetFull.  # noqa: E501
+        :param data_selectors: The data_selectors of this Widget.  # noqa: E501
         :type: DataSelector
         """
 
         self._data_selectors = data_selectors
 
     @property
     def dt_u(self):
-        """Gets the dt_u of this WidgetFull.  # noqa: E501
+        """Gets the dt_u of this Widget.  # noqa: E501
 
 
-        :return: The dt_u of this WidgetFull.  # noqa: E501
+        :return: The dt_u of this Widget.  # noqa: E501
         :rtype: datetime
         """
         return self._dt_u
 
     @dt_u.setter
     def dt_u(self, dt_u):
-        """Sets the dt_u of this WidgetFull.
+        """Sets the dt_u of this Widget.
 
 
-        :param dt_u: The dt_u of this WidgetFull.  # noqa: E501
+        :param dt_u: The dt_u of this Widget.  # noqa: E501
         :type: datetime
         """
 
         self._dt_u = dt_u
 
     @property
     def filter_excludes(self):
-        """Gets the filter_excludes of this WidgetFull.  # noqa: E501
+        """Gets the filter_excludes of this Widget.  # noqa: E501
 
 
-        :return: The filter_excludes of this WidgetFull.  # noqa: E501
+        :return: The filter_excludes of this Widget.  # noqa: E501
         :rtype: list[str]
         """
         return self._filter_excludes
 
     @filter_excludes.setter
     def filter_excludes(self, filter_excludes):
-        """Sets the filter_excludes of this WidgetFull.
+        """Sets the filter_excludes of this Widget.
 
 
-        :param filter_excludes: The filter_excludes of this WidgetFull.  # noqa: E501
+        :param filter_excludes: The filter_excludes of this Widget.  # noqa: E501
         :type: list[str]
         """
 
         self._filter_excludes = filter_excludes
 
     @property
     def filter_map(self):
-        """Gets the filter_map of this WidgetFull.  # noqa: E501
+        """Gets the filter_map of this Widget.  # noqa: E501
 
 
-        :return: The filter_map of this WidgetFull.  # noqa: E501
+        :return: The filter_map of this Widget.  # noqa: E501
         :rtype: list[FilterMap]
         """
         return self._filter_map
 
     @filter_map.setter
     def filter_map(self, filter_map):
-        """Sets the filter_map of this WidgetFull.
+        """Sets the filter_map of this Widget.
 
 
-        :param filter_map: The filter_map of this WidgetFull.  # noqa: E501
+        :param filter_map: The filter_map of this Widget.  # noqa: E501
         :type: list[FilterMap]
         """
 
         self._filter_map = filter_map
 
     @property
     def label_map(self):
-        """Gets the label_map of this WidgetFull.  # noqa: E501
+        """Gets the label_map of this Widget.  # noqa: E501
 
 
-        :return: The label_map of this WidgetFull.  # noqa: E501
+        :return: The label_map of this Widget.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._label_map
 
     @label_map.setter
     def label_map(self, label_map):
-        """Sets the label_map of this WidgetFull.
+        """Sets the label_map of this Widget.
 
 
-        :param label_map: The label_map of this WidgetFull.  # noqa: E501
+        :param label_map: The label_map of this Widget.  # noqa: E501
         :type: dict(str, object)
         """
 
         self._label_map = label_map
 
     @property
+    def links(self):
+        """Gets the links of this Widget.  # noqa: E501
+
+
+        :return: The links of this Widget.  # noqa: E501
+        :rtype: Link
+        """
+        return self._links
+
+    @links.setter
+    def links(self, links):
+        """Sets the links of this Widget.
+
+
+        :param links: The links of this Widget.  # noqa: E501
+        :type: Link
+        """
+
+        self._links = links
+
+    @property
     def settings(self):
-        """Gets the settings of this WidgetFull.  # noqa: E501
+        """Gets the settings of this Widget.  # noqa: E501
 
 
-        :return: The settings of this WidgetFull.  # noqa: E501
+        :return: The settings of this Widget.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._settings
 
     @settings.setter
     def settings(self, settings):
-        """Sets the settings of this WidgetFull.
+        """Sets the settings of this Widget.
 
 
-        :param settings: The settings of this WidgetFull.  # noqa: E501
+        :param settings: The settings of this Widget.  # noqa: E501
         :type: dict(str, object)
         """
 
         self._settings = settings
 
     @property
     def sub_title(self):
-        """Gets the sub_title of this WidgetFull.  # noqa: E501
+        """Gets the sub_title of this Widget.  # noqa: E501
 
 
-        :return: The sub_title of this WidgetFull.  # noqa: E501
+        :return: The sub_title of this Widget.  # noqa: E501
         :rtype: str
         """
         return self._sub_title
 
     @sub_title.setter
     def sub_title(self, sub_title):
-        """Sets the sub_title of this WidgetFull.
+        """Sets the sub_title of this Widget.
 
 
-        :param sub_title: The sub_title of this WidgetFull.  # noqa: E501
+        :param sub_title: The sub_title of this Widget.  # noqa: E501
         :type: str
         """
 
         self._sub_title = sub_title
 
     @property
     def sub_title_template(self):
-        """Gets the sub_title_template of this WidgetFull.  # noqa: E501
+        """Gets the sub_title_template of this Widget.  # noqa: E501
 
 
-        :return: The sub_title_template of this WidgetFull.  # noqa: E501
+        :return: The sub_title_template of this Widget.  # noqa: E501
         :rtype: list[dict(str, object)]
         """
         return self._sub_title_template
 
     @sub_title_template.setter
     def sub_title_template(self, sub_title_template):
-        """Sets the sub_title_template of this WidgetFull.
+        """Sets the sub_title_template of this Widget.
 
 
-        :param sub_title_template: The sub_title_template of this WidgetFull.  # noqa: E501
+        :param sub_title_template: The sub_title_template of this Widget.  # noqa: E501
         :type: list[dict(str, object)]
         """
 
         self._sub_title_template = sub_title_template
 
     @property
     def title(self):
-        """Gets the title of this WidgetFull.  # noqa: E501
+        """Gets the title of this Widget.  # noqa: E501
 
 
-        :return: The title of this WidgetFull.  # noqa: E501
+        :return: The title of this Widget.  # noqa: E501
         :rtype: str
         """
         return self._title
 
     @title.setter
     def title(self, title):
-        """Sets the title of this WidgetFull.
+        """Sets the title of this Widget.
 
 
-        :param title: The title of this WidgetFull.  # noqa: E501
+        :param title: The title of this Widget.  # noqa: E501
         :type: str
         """
         if title is None:
             raise ValueError("Invalid value for `title`, must not be `None`")  # noqa: E501
 
         self._title = title
 
     @property
     def title_template(self):
-        """Gets the title_template of this WidgetFull.  # noqa: E501
+        """Gets the title_template of this Widget.  # noqa: E501
 
 
-        :return: The title_template of this WidgetFull.  # noqa: E501
+        :return: The title_template of this Widget.  # noqa: E501
         :rtype: list[dict(str, object)]
         """
         return self._title_template
 
     @title_template.setter
     def title_template(self, title_template):
-        """Sets the title_template of this WidgetFull.
+        """Sets the title_template of this Widget.
 
 
-        :param title_template: The title_template of this WidgetFull.  # noqa: E501
+        :param title_template: The title_template of this Widget.  # noqa: E501
         :type: list[dict(str, object)]
         """
 
         self._title_template = title_template
 
     @property
     def view_hash_key(self):
-        """Gets the view_hash_key of this WidgetFull.  # noqa: E501
+        """Gets the view_hash_key of this Widget.  # noqa: E501
 
 
-        :return: The view_hash_key of this WidgetFull.  # noqa: E501
+        :return: The view_hash_key of this Widget.  # noqa: E501
         :rtype: str
         """
         return self._view_hash_key
 
     @view_hash_key.setter
     def view_hash_key(self, view_hash_key):
-        """Sets the view_hash_key of this WidgetFull.
+        """Sets the view_hash_key of this Widget.
 
 
-        :param view_hash_key: The view_hash_key of this WidgetFull.  # noqa: E501
+        :param view_hash_key: The view_hash_key of this Widget.  # noqa: E501
         :type: str
         """
         if view_hash_key is None:
             raise ValueError("Invalid value for `view_hash_key`, must not be `None`")  # noqa: E501
 
         self._view_hash_key = view_hash_key
 
     @property
     def view_transforms(self):
-        """Gets the view_transforms of this WidgetFull.  # noqa: E501
+        """Gets the view_transforms of this Widget.  # noqa: E501
 
 
-        :return: The view_transforms of this WidgetFull.  # noqa: E501
+        :return: The view_transforms of this Widget.  # noqa: E501
         :rtype: list[dict(str, object)]
         """
         return self._view_transforms
 
     @view_transforms.setter
     def view_transforms(self, view_transforms):
-        """Sets the view_transforms of this WidgetFull.
+        """Sets the view_transforms of this Widget.
 
 
-        :param view_transforms: The view_transforms of this WidgetFull.  # noqa: E501
+        :param view_transforms: The view_transforms of this Widget.  # noqa: E501
         :type: list[dict(str, object)]
         """
 
         self._view_transforms = view_transforms
 
     @property
     def widget_type_name(self):
-        """Gets the widget_type_name of this WidgetFull.  # noqa: E501
+        """Gets the widget_type_name of this Widget.  # noqa: E501
 
 
-        :return: The widget_type_name of this WidgetFull.  # noqa: E501
+        :return: The widget_type_name of this Widget.  # noqa: E501
         :rtype: str
         """
         return self._widget_type_name
 
     @widget_type_name.setter
     def widget_type_name(self, widget_type_name):
-        """Sets the widget_type_name of this WidgetFull.
+        """Sets the widget_type_name of this Widget.
 
 
-        :param widget_type_name: The widget_type_name of this WidgetFull.  # noqa: E501
+        :param widget_type_name: The widget_type_name of this Widget.  # noqa: E501
         :type: str
         """
         if widget_type_name is None:
             raise ValueError("Invalid value for `widget_type_name`, must not be `None`")  # noqa: E501
 
         self._widget_type_name = widget_type_name
 
@@ -440,15 +465,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WidgetFull):
+        if not isinstance(other, Widget):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/widget_type.py` & `nucleus_client-0.9.0/nucleus_client/models/widget_type.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/write_config.py` & `nucleus_client-0.9.0/nucleus_client/models/write_config_override.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,118 +12,118 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class WriteConfig(object):
+class WriteConfigOverride(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'druid': 'DruidWriteConfig',
-        'overrides': 'WriteConfigOverride',
-        'write_output': 'bool'
+        'column': 'str',
+        'druid': 'WriteConfigDruidOverride',
+        'output_column': 'str'
     }
 
     attribute_map = {
+        'column': 'column',
         'druid': 'druid',
-        'overrides': 'overrides',
-        'write_output': 'write_output'
+        'output_column': 'output_column'
     }
 
-    def __init__(self, druid=None, overrides=None, write_output=None):  # noqa: E501
-        """WriteConfig - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, column=None, druid=None, output_column=None):  # noqa: E501
+        """WriteConfigOverride - a model defined in OpenAPI"""  # noqa: E501
 
+        self._column = None
         self._druid = None
-        self._overrides = None
-        self._write_output = None
+        self._output_column = None
         self.discriminator = None
 
+        self.column = column
         if druid is not None:
             self.druid = druid
-        if overrides is not None:
-            self.overrides = overrides
-        self.write_output = write_output
+        if output_column is not None:
+            self.output_column = output_column
 
     @property
-    def druid(self):
-        """Gets the druid of this WriteConfig.  # noqa: E501
+    def column(self):
+        """Gets the column of this WriteConfigOverride.  # noqa: E501
 
 
-        :return: The druid of this WriteConfig.  # noqa: E501
-        :rtype: DruidWriteConfig
+        :return: The column of this WriteConfigOverride.  # noqa: E501
+        :rtype: str
         """
-        return self._druid
+        return self._column
 
-    @druid.setter
-    def druid(self, druid):
-        """Sets the druid of this WriteConfig.
+    @column.setter
+    def column(self, column):
+        """Sets the column of this WriteConfigOverride.
 
 
-        :param druid: The druid of this WriteConfig.  # noqa: E501
-        :type: DruidWriteConfig
+        :param column: The column of this WriteConfigOverride.  # noqa: E501
+        :type: str
         """
+        if column is None:
+            raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
 
-        self._druid = druid
+        self._column = column
 
     @property
-    def overrides(self):
-        """Gets the overrides of this WriteConfig.  # noqa: E501
+    def druid(self):
+        """Gets the druid of this WriteConfigOverride.  # noqa: E501
 
 
-        :return: The overrides of this WriteConfig.  # noqa: E501
-        :rtype: WriteConfigOverride
+        :return: The druid of this WriteConfigOverride.  # noqa: E501
+        :rtype: WriteConfigDruidOverride
         """
-        return self._overrides
+        return self._druid
 
-    @overrides.setter
-    def overrides(self, overrides):
-        """Sets the overrides of this WriteConfig.
+    @druid.setter
+    def druid(self, druid):
+        """Sets the druid of this WriteConfigOverride.
 
 
-        :param overrides: The overrides of this WriteConfig.  # noqa: E501
-        :type: WriteConfigOverride
+        :param druid: The druid of this WriteConfigOverride.  # noqa: E501
+        :type: WriteConfigDruidOverride
         """
 
-        self._overrides = overrides
+        self._druid = druid
 
     @property
-    def write_output(self):
-        """Gets the write_output of this WriteConfig.  # noqa: E501
+    def output_column(self):
+        """Gets the output_column of this WriteConfigOverride.  # noqa: E501
 
 
-        :return: The write_output of this WriteConfig.  # noqa: E501
-        :rtype: bool
+        :return: The output_column of this WriteConfigOverride.  # noqa: E501
+        :rtype: str
         """
-        return self._write_output
+        return self._output_column
 
-    @write_output.setter
-    def write_output(self, write_output):
-        """Sets the write_output of this WriteConfig.
+    @output_column.setter
+    def output_column(self, output_column):
+        """Sets the output_column of this WriteConfigOverride.
 
 
-        :param write_output: The write_output of this WriteConfig.  # noqa: E501
-        :type: bool
+        :param output_column: The output_column of this WriteConfigOverride.  # noqa: E501
+        :type: str
         """
-        if write_output is None:
-            raise ValueError("Invalid value for `write_output`, must not be `None`")  # noqa: E501
 
-        self._write_output = write_output
+        self._output_column = output_column
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -151,15 +151,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WriteConfig):
+        if not isinstance(other, WriteConfigOverride):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/models/write_config_druid_override.py` & `nucleus_client-0.9.0/nucleus_client/models/write_config_druid_override.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client/models/write_config_override.py` & `nucleus_client-0.9.0/nucleus_client/models/email_address.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,118 +12,119 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class WriteConfigOverride(object):
+class EmailAddress(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'column': 'str',
-        'druid': 'WriteConfigDruidOverride',
-        'output_column': 'str'
+        'email_address': 'str',
+        'name': 'str',
+        'to_type': 'str'
     }
 
     attribute_map = {
-        'column': 'column',
-        'druid': 'druid',
-        'output_column': 'output_column'
+        'email_address': 'email_address',
+        'name': 'name',
+        'to_type': 'to_type'
     }
 
-    def __init__(self, column=None, druid=None, output_column=None):  # noqa: E501
-        """WriteConfigOverride - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, email_address=None, name=None, to_type=None):  # noqa: E501
+        """EmailAddress - a model defined in OpenAPI"""  # noqa: E501
 
-        self._column = None
-        self._druid = None
-        self._output_column = None
+        self._email_address = None
+        self._name = None
+        self._to_type = None
         self.discriminator = None
 
-        self.column = column
-        if druid is not None:
-            self.druid = druid
-        if output_column is not None:
-            self.output_column = output_column
+        self.email_address = email_address
+        self.name = name
+        if to_type is not None:
+            self.to_type = to_type
 
     @property
-    def column(self):
-        """Gets the column of this WriteConfigOverride.  # noqa: E501
+    def email_address(self):
+        """Gets the email_address of this EmailAddress.  # noqa: E501
 
 
-        :return: The column of this WriteConfigOverride.  # noqa: E501
+        :return: The email_address of this EmailAddress.  # noqa: E501
         :rtype: str
         """
-        return self._column
+        return self._email_address
 
-    @column.setter
-    def column(self, column):
-        """Sets the column of this WriteConfigOverride.
+    @email_address.setter
+    def email_address(self, email_address):
+        """Sets the email_address of this EmailAddress.
 
 
-        :param column: The column of this WriteConfigOverride.  # noqa: E501
+        :param email_address: The email_address of this EmailAddress.  # noqa: E501
         :type: str
         """
-        if column is None:
-            raise ValueError("Invalid value for `column`, must not be `None`")  # noqa: E501
+        if email_address is None:
+            raise ValueError("Invalid value for `email_address`, must not be `None`")  # noqa: E501
 
-        self._column = column
+        self._email_address = email_address
 
     @property
-    def druid(self):
-        """Gets the druid of this WriteConfigOverride.  # noqa: E501
+    def name(self):
+        """Gets the name of this EmailAddress.  # noqa: E501
 
 
-        :return: The druid of this WriteConfigOverride.  # noqa: E501
-        :rtype: WriteConfigDruidOverride
+        :return: The name of this EmailAddress.  # noqa: E501
+        :rtype: str
         """
-        return self._druid
+        return self._name
 
-    @druid.setter
-    def druid(self, druid):
-        """Sets the druid of this WriteConfigOverride.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this EmailAddress.
 
 
-        :param druid: The druid of this WriteConfigOverride.  # noqa: E501
-        :type: WriteConfigDruidOverride
+        :param name: The name of this EmailAddress.  # noqa: E501
+        :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._druid = druid
+        self._name = name
 
     @property
-    def output_column(self):
-        """Gets the output_column of this WriteConfigOverride.  # noqa: E501
+    def to_type(self):
+        """Gets the to_type of this EmailAddress.  # noqa: E501
 
 
-        :return: The output_column of this WriteConfigOverride.  # noqa: E501
+        :return: The to_type of this EmailAddress.  # noqa: E501
         :rtype: str
         """
-        return self._output_column
+        return self._to_type
 
-    @output_column.setter
-    def output_column(self, output_column):
-        """Sets the output_column of this WriteConfigOverride.
+    @to_type.setter
+    def to_type(self, to_type):
+        """Sets the to_type of this EmailAddress.
 
 
-        :param output_column: The output_column of this WriteConfigOverride.  # noqa: E501
+        :param to_type: The to_type of this EmailAddress.  # noqa: E501
         :type: str
         """
 
-        self._output_column = output_column
+        self._to_type = to_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -151,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WriteConfigOverride):
+        if not isinstance(other, EmailAddress):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `nucleus_client-0.8.0/nucleus_client/rest.py` & `nucleus_client-0.9.0/nucleus_client/rest.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/nucleus_client.egg-info/SOURCES.txt` & `nucleus_client-0.9.0/nucleus_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 nucleus_client/models/divide_metric.py
 nucleus_client/models/download.py
 nucleus_client/models/download_error.py
 nucleus_client/models/download_v1.py
 nucleus_client/models/download_v2.py
 nucleus_client/models/drop_transform.py
 nucleus_client/models/druid_write_config.py
+nucleus_client/models/email_address.py
+nucleus_client/models/email_report_config.py
 nucleus_client/models/entity_batch.py
 nucleus_client/models/entity_batch_health.py
 nucleus_client/models/filter.py
 nucleus_client/models/filter_map.py
 nucleus_client/models/filter_preset.py
 nucleus_client/models/geo_data.py
 nucleus_client/models/goal.py
@@ -111,14 +113,15 @@
 nucleus_client/models/integration_type.py
 nucleus_client/models/integration_type_update.py
 nucleus_client/models/integration_update.py
 nucleus_client/models/job.py
 nucleus_client/models/job_overview.py
 nucleus_client/models/join.py
 nucleus_client/models/join_relationship.py
+nucleus_client/models/link.py
 nucleus_client/models/loader_settings.py
 nucleus_client/models/map_explode_many_transform.py
 nucleus_client/models/map_explode_transform.py
 nucleus_client/models/map_transform.py
 nucleus_client/models/multiply_metric.py
 nucleus_client/models/new_user_token.py
 nucleus_client/models/non_null_filter.py
@@ -130,14 +133,15 @@
 nucleus_client/models/number_bucket_transform.py
 nucleus_client/models/number_cast_transform.py
 nucleus_client/models/number_constant_transform.py
 nucleus_client/models/number_default_transform.py
 nucleus_client/models/number_filter.py
 nucleus_client/models/number_transform.py
 nucleus_client/models/number_unary_transform.py
+nucleus_client/models/options.py
 nucleus_client/models/or_filter.py
 nucleus_client/models/page.py
 nucleus_client/models/page_filter_preferences.py
 nucleus_client/models/page_full.py
 nucleus_client/models/page_preferences.py
 nucleus_client/models/page_preferences_update.py
 nucleus_client/models/page_publications.py
@@ -145,20 +149,35 @@
 nucleus_client/models/page_template_update.py
 nucleus_client/models/page_view.py
 nucleus_client/models/partner_batch.py
 nucleus_client/models/partner_post_data.py
 nucleus_client/models/password_change_request.py
 nucleus_client/models/password_reset_change.py
 nucleus_client/models/password_reset_request.py
+nucleus_client/models/percentage_metric.py
 nucleus_client/models/percentile_lookup_metric.py
 nucleus_client/models/post_data.py
+nucleus_client/models/prolearn_base_object.py
+nucleus_client/models/prolearn_callback.py
+nucleus_client/models/prolearn_course.py
+nucleus_client/models/prolearn_credit.py
+nucleus_client/models/prolearn_credit_type.py
+nucleus_client/models/prolearn_registration.py
+nucleus_client/models/prolearn_user.py
 nucleus_client/models/refresh_interval.py
 nucleus_client/models/refresh_schedule.py
 nucleus_client/models/refresh_state.py
 nucleus_client/models/rename_transform.py
+nucleus_client/models/rename_transform2.py
+nucleus_client/models/report.py
+nucleus_client/models/report_add.py
+nucleus_client/models/report_config.py
+nucleus_client/models/report_config_update.py
+nucleus_client/models/report_error.py
+nucleus_client/models/report_update.py
 nucleus_client/models/role.py
 nucleus_client/models/role_permission.py
 nucleus_client/models/role_update.py
 nucleus_client/models/sarimax_dataset_task.py
 nucleus_client/models/sarimax_task.py
 nucleus_client/models/sarimax_task_metric.py
 nucleus_client/models/schema.py
@@ -207,23 +226,26 @@
 nucleus_client/models/top_n_task_partition.py
 nucleus_client/models/top_n_task_sort.py
 nucleus_client/models/transform.py
 nucleus_client/models/unary_metric.py
 nucleus_client/models/unique_limit.py
 nucleus_client/models/update_api_user.py
 nucleus_client/models/update_user.py
+nucleus_client/models/upload.py
+nucleus_client/models/upload_field.py
 nucleus_client/models/user_activation.py
 nucleus_client/models/user_role.py
 nucleus_client/models/user_token.py
 nucleus_client/models/view.py
 nucleus_client/models/view_error.py
 nucleus_client/models/virtual_user.py
 nucleus_client/models/widget.py
 nucleus_client/models/widget_full.py
 nucleus_client/models/widget_type.py
+nucleus_client/models/write_backup.py
 nucleus_client/models/write_config.py
 nucleus_client/models/write_config_druid_override.py
 nucleus_client/models/write_config_override.py
 test/__init__.py
 test/test_activity.py
 test/test_add_metric.py
 test/test_aggregation_dataset_task.py
@@ -304,14 +326,16 @@
 test/test_divide_metric.py
 test/test_download.py
 test/test_download_error.py
 test/test_download_v1.py
 test/test_download_v2.py
 test/test_drop_transform.py
 test/test_druid_write_config.py
+test/test_email_address.py
+test/test_email_report_config.py
 test/test_entity_batch.py
 test/test_entity_batch_health.py
 test/test_filter.py
 test/test_filter_map.py
 test/test_filter_preset.py
 test/test_geo_data.py
 test/test_goal.py
@@ -324,14 +348,15 @@
 test/test_integration_type.py
 test/test_integration_type_update.py
 test/test_integration_update.py
 test/test_job.py
 test/test_job_overview.py
 test/test_join.py
 test/test_join_relationship.py
+test/test_link.py
 test/test_loader_settings.py
 test/test_map_explode_many_transform.py
 test/test_map_explode_transform.py
 test/test_map_transform.py
 test/test_multiply_metric.py
 test/test_new_user_token.py
 test/test_non_null_filter.py
@@ -343,14 +368,15 @@
 test/test_number_bucket_transform.py
 test/test_number_cast_transform.py
 test/test_number_constant_transform.py
 test/test_number_default_transform.py
 test/test_number_filter.py
 test/test_number_transform.py
 test/test_number_unary_transform.py
+test/test_options.py
 test/test_or_filter.py
 test/test_page.py
 test/test_page_filter_preferences.py
 test/test_page_full.py
 test/test_page_preferences.py
 test/test_page_preferences_update.py
 test/test_page_publications.py
@@ -358,20 +384,35 @@
 test/test_page_template_update.py
 test/test_page_view.py
 test/test_partner_batch.py
 test/test_partner_post_data.py
 test/test_password_change_request.py
 test/test_password_reset_change.py
 test/test_password_reset_request.py
+test/test_percentage_metric.py
 test/test_percentile_lookup_metric.py
 test/test_post_data.py
+test/test_prolearn_base_object.py
+test/test_prolearn_callback.py
+test/test_prolearn_course.py
+test/test_prolearn_credit.py
+test/test_prolearn_credit_type.py
+test/test_prolearn_registration.py
+test/test_prolearn_user.py
 test/test_refresh_interval.py
 test/test_refresh_schedule.py
 test/test_refresh_state.py
 test/test_rename_transform.py
+test/test_rename_transform2.py
+test/test_report.py
+test/test_report_add.py
+test/test_report_config.py
+test/test_report_config_update.py
+test/test_report_error.py
+test/test_report_update.py
 test/test_role.py
 test/test_role_permission.py
 test/test_role_update.py
 test/test_sarimax_dataset_task.py
 test/test_sarimax_task.py
 test/test_sarimax_task_metric.py
 test/test_schema.py
@@ -420,19 +461,22 @@
 test/test_top_n_task_partition.py
 test/test_top_n_task_sort.py
 test/test_transform.py
 test/test_unary_metric.py
 test/test_unique_limit.py
 test/test_update_api_user.py
 test/test_update_user.py
+test/test_upload.py
+test/test_upload_field.py
 test/test_user_activation.py
 test/test_user_role.py
 test/test_user_token.py
 test/test_view.py
 test/test_view_error.py
 test/test_virtual_user.py
 test/test_widget.py
 test/test_widget_full.py
 test/test_widget_type.py
+test/test_write_backup.py
 test/test_write_config.py
 test/test_write_config_druid_override.py
 test/test_write_config_override.py
```

### Comparing `nucleus_client-0.8.0/setup.py` & `nucleus_client-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "nucleus_client"
-VERSION = "0.8.0"
+VERSION = "0.9.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `nucleus_client-0.8.0/test/test_activity.py` & `nucleus_client-0.9.0/test/test_activity.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_add_metric.py` & `nucleus_client-0.9.0/test/test_add_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_aggregation_dataset_task.py` & `nucleus_client-0.9.0/test/test_aggregation_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_aggregation_parameterized_task.py` & `nucleus_client-0.9.0/test/test_aggregation_parameterized_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_aggregation_task.py` & `nucleus_client-0.9.0/test/test_aggregation_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_aggregation_task_metric.py` & `nucleus_client-0.9.0/test/test_aggregation_task_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_api_user.py` & `nucleus_client-0.9.0/test/test_api_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_array_explode_many_transform.py` & `nucleus_client-0.9.0/test/test_array_explode_many_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_array_explode_transform.py` & `nucleus_client-0.9.0/test/test_array_explode_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_array_transform.py` & `nucleus_client-0.9.0/test/test_array_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_base_page.py` & `nucleus_client-0.9.0/test/test_base_page.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_base_templated_page.py` & `nucleus_client-0.9.0/test/test_base_templated_page.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_base_user.py` & `nucleus_client-0.9.0/test/test_base_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_batch_receipt.py` & `nucleus_client-0.9.0/test/test_batch_receipt.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_binomial_logistic_regression_task.py` & `nucleus_client-0.9.0/test/test_binomial_logistic_regression_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_block.py` & `nucleus_client-0.9.0/test/test_block.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_block_full.py` & `nucleus_client-0.9.0/test/test_block_full.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_block_type.py` & `nucleus_client-0.9.0/test/test_block_type.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_boolean_bucket_filter.py` & `nucleus_client-0.9.0/test/test_boolean_bucket_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_boolean_bucket_transform.py` & `nucleus_client-0.9.0/test/test_boolean_bucket_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_boolean_cast_transform.py` & `nucleus_client-0.9.0/test/test_boolean_cast_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_boolean_constant_transform.py` & `nucleus_client-0.9.0/test/test_boolean_constant_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_boolean_filter.py` & `nucleus_client-0.9.0/test/test_boolean_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_boolean_transform.py` & `nucleus_client-0.9.0/test/test_boolean_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_client.py` & `nucleus_client-0.9.0/test/test_client.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_client_features.py` & `nucleus_client-0.9.0/test/test_client_features.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_client_package.py` & `nucleus_client-0.9.0/test/test_client_package.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_client_settings.py` & `nucleus_client-0.9.0/test/test_client_settings.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_client_settings_update.py` & `nucleus_client-0.9.0/test/test_client_settings_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_client_sso.py` & `nucleus_client-0.9.0/test/test_client_sso.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_client_update.py` & `nucleus_client-0.9.0/test/test_client_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_coalesce_transform.py` & `nucleus_client-0.9.0/test/test_coalesce_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_collection_size_transform.py` & `nucleus_client-0.9.0/test/test_collection_size_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_column_mapping.py` & `nucleus_client-0.9.0/test/test_column_mapping.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_count_metric.py` & `nucleus_client-0.9.0/test/test_count_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_create_custom_dataset_task.py` & `nucleus_client-0.9.0/test/test_create_custom_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_cumulative_metric.py` & `nucleus_client-0.9.0/test/test_cumulative_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_cumulative_metric_order_by.py` & `nucleus_client-0.9.0/test/test_cumulative_metric_order_by.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_cumulative_sum_metric.py` & `nucleus_client-0.9.0/test/test_cumulative_sum_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_selector.py` & `nucleus_client-0.9.0/test/test_data_selector.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view.py` & `nucleus_client-0.9.0/test/test_data_view.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_base.py` & `nucleus_client-0.9.0/test/test_data_view_base.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_dimension.py` & `nucleus_client-0.9.0/test/test_data_view_dimension.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_filter.py` & `nucleus_client-0.9.0/test/test_data_view_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_filter_value.py` & `nucleus_client-0.9.0/test/test_data_view_filter_value.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_interval.py` & `nucleus_client-0.9.0/test/test_data_view_interval.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_lookup.py` & `nucleus_client-0.9.0/test/test_data_view_lookup.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_metric.py` & `nucleus_client-0.9.0/test/test_data_view_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_metric_calc.py` & `nucleus_client-0.9.0/test/test_data_view_metric_calc.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_metric_order_by.py` & `nucleus_client-0.9.0/test/test_data_view_metric_order_by.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_mode.py` & `nucleus_client-0.9.0/test/test_data_view_mode.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_period_to_date.py` & `nucleus_client-0.9.0/test/test_data_view_period_to_date.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_sort.py` & `nucleus_client-0.9.0/test/test_data_view_sort.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_data_view_unique_limit.py` & `nucleus_client-0.9.0/test/test_data_view_unique_limit.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_dataset.py` & `nucleus_client-0.9.0/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_dataset_error.py` & `nucleus_client-0.9.0/test/test_dataset_error.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_dataset_metadata.py` & `nucleus_client-0.9.0/test/test_dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_dataset_update.py` & `nucleus_client-0.9.0/test/test_dataset_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_date_dimension.py` & `nucleus_client-0.9.0/test/test_date_dimension.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_date_time_filter.py` & `nucleus_client-0.9.0/test/test_date_time_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_date_time_filter_component.py` & `nucleus_client-0.9.0/test/test_date_time_filter_component.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_constant_transform.py` & `nucleus_client-0.9.0/test/test_datetime_constant_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_current_date_transform.py` & `nucleus_client-0.9.0/test/test_datetime_current_date_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_current_timestamp_transform.py` & `nucleus_client-0.9.0/test/test_datetime_current_timestamp_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_diff_from_column_date_transform.py` & `nucleus_client-0.9.0/test/test_datetime_diff_from_column_date_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_diff_from_now_transform.py` & `nucleus_client-0.9.0/test/test_datetime_diff_from_now_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_diff_from_static_date_transform.py` & `nucleus_client-0.9.0/test/test_datetime_diff_from_static_date_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_diff_transform.py` & `nucleus_client-0.9.0/test/test_datetime_diff_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_format_transform.py` & `nucleus_client-0.9.0/test/test_datetime_format_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_offset_column_value_transform.py` & `nucleus_client-0.9.0/test/test_datetime_offset_column_value_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_offset_static_value_transform.py` & `nucleus_client-0.9.0/test/test_datetime_offset_static_value_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_offset_transform.py` & `nucleus_client-0.9.0/test/test_datetime_offset_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_range_transform.py` & `nucleus_client-0.9.0/test/test_datetime_range_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_select_transform.py` & `nucleus_client-0.9.0/test/test_datetime_select_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_datetime_transform.py` & `nucleus_client-0.9.0/test/test_datetime_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_default_api.py` & `nucleus_client-0.9.0/test/test_default_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -129,14 +129,21 @@
     def test_add_integration(self):
         """Test case for add_integration
 
         Adds a new integration  # noqa: E501
         """
         pass
 
+    def test_add_integration_sync_request(self):
+        """Test case for add_integration_sync_request
+
+        Run a sync integration      Responses:          204: The sync request was successfully queued  # noqa: E501
+        """
+        pass
+
     def test_add_integration_type(self):
         """Test case for add_integration_type
 
         Add a new integration type  # noqa: E501
         """
         pass
 
@@ -171,14 +178,35 @@
     def test_add_password_reset_request(self):
         """Test case for add_password_reset_request
 
         Creates a new request to reset a user's password  # noqa: E501
         """
         pass
 
+    def test_add_prolearn_activity(self):
+        """Test case for add_prolearn_activity
+
+        Prolearn callback  # noqa: E501
+        """
+        pass
+
+    def test_add_report(self):
+        """Test case for add_report
+
+        Add a new report  # noqa: E501
+        """
+        pass
+
+    def test_add_report_config(self):
+        """Test case for add_report_config
+
+        Add a new report_config  # noqa: E501
+        """
+        pass
+
     def test_add_role(self):
         """Test case for add_role
 
         Adds a new role  # noqa: E501
         """
         pass
 
@@ -192,14 +220,21 @@
     def test_add_term(self):
         """Test case for add_term
 
         Adds a new term  # noqa: E501
         """
         pass
 
+    def test_add_upload_request(self):
+        """Test case for add_upload_request
+
+        Adds a new (pending) upload request  # noqa: E501
+        """
+        pass
+
     def test_add_user(self):
         """Test case for add_user
 
         Adds a new user  # noqa: E501
         """
         pass
 
@@ -339,14 +374,28 @@
     def test_delete_page_template_by_slug(self):
         """Test case for delete_page_template_by_slug
 
         Deletes all page templates with the specified slug  # noqa: E501
         """
         pass
 
+    def test_delete_report(self):
+        """Test case for delete_report
+
+        Deletes a report by ID  # noqa: E501
+        """
+        pass
+
+    def test_delete_report_config(self):
+        """Test case for delete_report_config
+
+        Deletes a report_config by ID  # noqa: E501
+        """
+        pass
+
     def test_delete_role(self):
         """Test case for delete_role
 
         Deletes a role by ID  # noqa: E501
         """
         pass
 
@@ -563,14 +612,35 @@
     def test_get_password_reset_by_key(self):
         """Test case for get_password_reset_by_key
 
         Gets a user by the reset key associated with them  # noqa: E501
         """
         pass
 
+    def test_get_report(self):
+        """Test case for get_report
+
+        Get a report by ID  # noqa: E501
+        """
+        pass
+
+    def test_get_report_config(self):
+        """Test case for get_report_config
+
+        Get a report_config by ID  # noqa: E501
+        """
+        pass
+
+    def test_get_report_config_by_name(self):
+        """Test case for get_report_config_by_name
+
+        Get a report_config by name  # noqa: E501
+        """
+        pass
+
     def test_get_role(self):
         """Test case for get_role
 
         Gets a role by ID  # noqa: E501
         """
         pass
 
@@ -605,14 +675,21 @@
     def test_get_term_by_term(self):
         """Test case for get_term_by_term
 
         Gets a term by term  # noqa: E501
         """
         pass
 
+    def test_get_upload_request(self):
+        """Test case for get_upload_request
+
+        Gets an upload request by id  # noqa: E501
+        """
+        pass
+
     def test_get_user(self):
         """Test case for get_user
 
         Gets a user by ID  # noqa: E501
         """
         pass
 
@@ -801,14 +878,28 @@
     def test_list_pages_by_page_template(self):
         """Test case for list_pages_by_page_template
 
         List all pages associated with a particular page template and optionally client  # noqa: E501
         """
         pass
 
+    def test_list_report_configs(self):
+        """Test case for list_report_configs
+
+        List all report_configs associated with a client  # noqa: E501
+        """
+        pass
+
+    def test_list_reports(self):
+        """Test case for list_reports
+
+        List all reports associated with a client  # noqa: E501
+        """
+        pass
+
     def test_list_role_permissions(self):
         """Test case for list_role_permissions
 
         List all permissions for a specific role  # noqa: E501
         """
         pass
 
@@ -829,14 +920,21 @@
     def test_list_terms(self):
         """Test case for list_terms
 
         List all terms associated with a client  # noqa: E501
         """
         pass
 
+    def test_list_upload_requests(self):
+        """Test case for list_upload_requests
+
+        Gets all unexpired upload requests for the authenticated user  # noqa: E501
+        """
+        pass
+
     def test_list_user_roles(self):
         """Test case for list_user_roles
 
         List all roles for a specific user  # noqa: E501
         """
         pass
 
@@ -976,14 +1074,28 @@
     def test_update_page_preference(self):
         """Test case for update_page_preference
 
         Add or update a page preference  # noqa: E501
         """
         pass
 
+    def test_update_report(self):
+        """Test case for update_report
+
+        Updates an existing report  # noqa: E501
+        """
+        pass
+
+    def test_update_report_config(self):
+        """Test case for update_report_config
+
+        Updates an existing report_config  # noqa: E501
+        """
+        pass
+
     def test_update_role(self):
         """Test case for update_role
 
         Updates an existing role  # noqa: E501
         """
         pass
```

### Comparing `nucleus_client-0.8.0/test/test_dimension.py` & `nucleus_client-0.9.0/test/test_dimension.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_divide_metric.py` & `nucleus_client-0.9.0/test/test_divide_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_download.py` & `nucleus_client-0.9.0/test/test_download.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_download_error.py` & `nucleus_client-0.9.0/test/test_download_error.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_download_v1.py` & `nucleus_client-0.9.0/test/test_download_v1.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_download_v2.py` & `nucleus_client-0.9.0/test/test_download_v2.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_drop_transform.py` & `nucleus_client-0.9.0/test/test_drop_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_druid_write_config.py` & `nucleus_client-0.9.0/test/test_druid_write_config.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_entity_batch.py` & `nucleus_client-0.9.0/test/test_entity_batch.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_entity_batch_health.py` & `nucleus_client-0.9.0/test/test_entity_batch_health.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_filter.py` & `nucleus_client-0.9.0/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_filter_map.py` & `nucleus_client-0.9.0/test/test_filter_map.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_filter_preset.py` & `nucleus_client-0.9.0/test/test_filter_preset.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_geo_data.py` & `nucleus_client-0.9.0/test/test_geo_data.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_goal.py` & `nucleus_client-0.9.0/test/test_goal.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_goal_filter.py` & `nucleus_client-0.9.0/test/test_goal_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_individual_data_selector.py` & `nucleus_client-0.9.0/test/test_individual_data_selector.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_integration.py` & `nucleus_client-0.9.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_integration_batch_history_receipt.py` & `nucleus_client-0.9.0/test/test_integration_batch_history_receipt.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_integration_dataset.py` & `nucleus_client-0.9.0/test/test_integration_dataset.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_integration_sync_history_receipt.py` & `nucleus_client-0.9.0/test/test_integration_sync_history_receipt.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_integration_type.py` & `nucleus_client-0.9.0/test/test_integration_type.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_integration_type_update.py` & `nucleus_client-0.9.0/test/test_integration_type_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_integration_update.py` & `nucleus_client-0.9.0/test/test_integration_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_job.py` & `nucleus_client-0.9.0/test/test_job.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_job_overview.py` & `nucleus_client-0.9.0/test/test_job_overview.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_join.py` & `nucleus_client-0.9.0/test/test_join.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_join_relationship.py` & `nucleus_client-0.9.0/test/test_join_relationship.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_loader_settings.py` & `nucleus_client-0.9.0/test/test_loader_settings.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_map_explode_many_transform.py` & `nucleus_client-0.9.0/test/test_map_explode_many_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_map_explode_transform.py` & `nucleus_client-0.9.0/test/test_map_explode_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_map_transform.py` & `nucleus_client-0.9.0/test/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_multiply_metric.py` & `nucleus_client-0.9.0/test/test_multiply_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_new_user_token.py` & `nucleus_client-0.9.0/test/test_new_user_token.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_non_null_filter.py` & `nucleus_client-0.9.0/test/test_non_null_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_normal_user.py` & `nucleus_client-0.9.0/test/test_normal_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_notify_user.py` & `nucleus_client-0.9.0/test/test_notify_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_binary_transform.py` & `nucleus_client-0.9.0/test/test_number_binary_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_binary_value_transform.py` & `nucleus_client-0.9.0/test/test_number_binary_value_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_bucket_filter.py` & `nucleus_client-0.9.0/test/test_number_bucket_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_bucket_transform.py` & `nucleus_client-0.9.0/test/test_number_bucket_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_cast_transform.py` & `nucleus_client-0.9.0/test/test_number_cast_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_constant_transform.py` & `nucleus_client-0.9.0/test/test_number_constant_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_default_transform.py` & `nucleus_client-0.9.0/test/test_number_default_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_filter.py` & `nucleus_client-0.9.0/test/test_number_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_transform.py` & `nucleus_client-0.9.0/test/test_number_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_number_unary_transform.py` & `nucleus_client-0.9.0/test/test_number_unary_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_or_filter.py` & `nucleus_client-0.9.0/test/test_or_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_page.py` & `nucleus_client-0.9.0/test/test_page.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_page_filter_preferences.py` & `nucleus_client-0.9.0/test/test_page_filter_preferences.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_page_full.py` & `nucleus_client-0.9.0/test/test_page_full.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_page_preferences.py` & `nucleus_client-0.9.0/test/test_page_preferences.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_page_preferences_update.py` & `nucleus_client-0.9.0/test/test_page_preferences_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_page_publications.py` & `nucleus_client-0.9.0/test/test_page_publications.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_page_template.py` & `nucleus_client-0.9.0/test/test_page_template.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_page_template_update.py` & `nucleus_client-0.9.0/test/test_page_template_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_page_view.py` & `nucleus_client-0.9.0/test/test_page_view.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_partner_batch.py` & `nucleus_client-0.9.0/test/test_partner_batch.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_partner_post_data.py` & `nucleus_client-0.9.0/test/test_partner_post_data.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_password_change_request.py` & `nucleus_client-0.9.0/test/test_password_change_request.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_password_reset_change.py` & `nucleus_client-0.9.0/test/test_password_reset_change.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_password_reset_request.py` & `nucleus_client-0.9.0/test/test_password_reset_request.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_percentile_lookup_metric.py` & `nucleus_client-0.9.0/test/test_percentile_lookup_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_post_data.py` & `nucleus_client-0.9.0/test/test_post_data.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_refresh_interval.py` & `nucleus_client-0.9.0/test/test_refresh_interval.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_refresh_schedule.py` & `nucleus_client-0.9.0/test/test_refresh_schedule.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_refresh_state.py` & `nucleus_client-0.9.0/test/test_refresh_state.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_rename_transform.py` & `nucleus_client-0.9.0/test/test_rename_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_role.py` & `nucleus_client-0.9.0/test/test_role.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_role_permission.py` & `nucleus_client-0.9.0/test/test_role_permission.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_role_update.py` & `nucleus_client-0.9.0/test/test_role_update.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_sarimax_dataset_task.py` & `nucleus_client-0.9.0/test/test_sarimax_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_sarimax_task.py` & `nucleus_client-0.9.0/test/test_sarimax_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_sarimax_task_metric.py` & `nucleus_client-0.9.0/test/test_sarimax_task_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_schema.py` & `nucleus_client-0.9.0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_schema_field.py` & `nucleus_client-0.9.0/test/test_schema_field.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_schema_field_metadata.py` & `nucleus_client-0.9.0/test/test_schema_field_metadata.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_schema_schema.py` & `nucleus_client-0.9.0/test/test_schema_schema.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_settings_spec.py` & `nucleus_client-0.9.0/test/test_settings_spec.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_snapshot_dataset_task.py` & `nucleus_client-0.9.0/test/test_snapshot_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_sort.py` & `nucleus_client-0.9.0/test/test_sort.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_bucket_filter.py` & `nucleus_client-0.9.0/test/test_string_bucket_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_bucket_transform.py` & `nucleus_client-0.9.0/test/test_string_bucket_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_casing_transform.py` & `nucleus_client-0.9.0/test/test_string_casing_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_constant_transform.py` & `nucleus_client-0.9.0/test/test_string_constant_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_default_transform.py` & `nucleus_client-0.9.0/test/test_string_default_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_distance_transform.py` & `nucleus_client-0.9.0/test/test_string_distance_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_extract_url_component_transform.py` & `nucleus_client-0.9.0/test/test_string_extract_url_component_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_filter.py` & `nucleus_client-0.9.0/test/test_string_filter.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_format_transform.py` & `nucleus_client-0.9.0/test/test_string_format_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_lookup_state_transform.py` & `nucleus_client-0.9.0/test/test_string_lookup_state_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_regexp_extract_transform.py` & `nucleus_client-0.9.0/test/test_string_regexp_extract_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_regexp_replace_transform.py` & `nucleus_client-0.9.0/test/test_string_regexp_replace_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_soundex_transform.py` & `nucleus_client-0.9.0/test/test_string_soundex_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_split_transform.py` & `nucleus_client-0.9.0/test/test_string_split_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_substring_index_transform.py` & `nucleus_client-0.9.0/test/test_string_substring_index_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_substring_transform.py` & `nucleus_client-0.9.0/test/test_string_substring_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_to_datetime_transform.py` & `nucleus_client-0.9.0/test/test_string_to_datetime_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_to_num_transform.py` & `nucleus_client-0.9.0/test/test_string_to_num_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_transform.py` & `nucleus_client-0.9.0/test/test_string_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_string_trim_transform.py` & `nucleus_client-0.9.0/test/test_string_trim_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_sub_nav.py` & `nucleus_client-0.9.0/test/test_sub_nav.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_subtract_metric.py` & `nucleus_client-0.9.0/test/test_subtract_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_templated_page.py` & `nucleus_client-0.9.0/test/test_templated_page.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_term.py` & `nucleus_client-0.9.0/test/test_term.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_aggregation_dataset_task.py` & `nucleus_client-0.9.0/test/test_time_step_aggregation_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_aggregation_task.py` & `nucleus_client-0.9.0/test/test_time_step_aggregation_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_difference_metric.py` & `nucleus_client-0.9.0/test/test_time_step_difference_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_growth_rate_metric.py` & `nucleus_client-0.9.0/test/test_time_step_growth_rate_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_metric.py` & `nucleus_client-0.9.0/test/test_time_step_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_metric_dataset_task.py` & `nucleus_client-0.9.0/test/test_time_step_metric_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_metric_task.py` & `nucleus_client-0.9.0/test/test_time_step_metric_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_mode.py` & `nucleus_client-0.9.0/test/test_time_step_mode.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_netforum_stats_metric.py` & `nucleus_client-0.9.0/test/test_time_step_netforum_stats_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_time_step_renewal_rate_metric.py` & `nucleus_client-0.9.0/test/test_time_step_renewal_rate_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_top_n_dataset_task.py` & `nucleus_client-0.9.0/test/test_top_n_dataset_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_top_n_task.py` & `nucleus_client-0.9.0/test/test_top_n_task.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_top_n_task_partition.py` & `nucleus_client-0.9.0/test/test_top_n_task_partition.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_top_n_task_sort.py` & `nucleus_client-0.9.0/test/test_top_n_task_sort.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_transform.py` & `nucleus_client-0.9.0/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_unary_metric.py` & `nucleus_client-0.9.0/test/test_unary_metric.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_unique_limit.py` & `nucleus_client-0.9.0/test/test_unique_limit.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_update_api_user.py` & `nucleus_client-0.9.0/test/test_update_api_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_update_user.py` & `nucleus_client-0.9.0/test/test_update_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_user_activation.py` & `nucleus_client-0.9.0/test/test_user_activation.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_user_role.py` & `nucleus_client-0.9.0/test/test_user_role.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_user_token.py` & `nucleus_client-0.9.0/test/test_user_token.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_view.py` & `nucleus_client-0.9.0/test/test_view.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_view_error.py` & `nucleus_client-0.9.0/test/test_view_error.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_virtual_user.py` & `nucleus_client-0.9.0/test/test_virtual_user.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_widget.py` & `nucleus_client-0.9.0/test/test_widget.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_widget_full.py` & `nucleus_client-0.9.0/test/test_widget_full.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_widget_type.py` & `nucleus_client-0.9.0/test/test_widget_type.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_write_config.py` & `nucleus_client-0.9.0/test/test_write_config.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_write_config_druid_override.py` & `nucleus_client-0.9.0/test/test_write_config_druid_override.py`

 * *Files identical despite different names*

### Comparing `nucleus_client-0.8.0/test/test_write_config_override.py` & `nucleus_client-0.9.0/test/test_write_config_override.py`

 * *Files identical despite different names*

