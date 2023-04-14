# Comparing `tmp/sample_metadata-5.6.1.tar.gz` & `tmp/sample_metadata-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample_metadata-5.6.1.tar", last modified: Tue Apr 11 23:58:43 2023, max compression
+gzip compressed data, was "sample_metadata-5.7.0.tar", last modified: Thu Apr 13 10:18:03 2023, max compression
```

## Comparing `sample_metadata-5.6.1.tar` & `sample_metadata-5.7.0.tar`

### file list

```diff
@@ -1,107 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.115352 sample_metadata-5.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-04-11 23:58:43.115352 sample_metadata-5.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.099352 sample_metadata-5.6.1/sample_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.099352 sample_metadata-5.6.1/sample_metadata/api/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61864 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42202 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27906 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53539 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47013 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38773 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/sequence_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37587 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.099352 sample_metadata-5.6.1/sample_metadata/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.103351 sample_metadata-5.6.1/sample_metadata/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/body_get_sequences_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/nested_family.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/nested_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/new_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/new_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/participant_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/participant_upsert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/project_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_batch_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_batch_upsert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_technology.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    82237 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.103351 sample_metadata-5.6.1/sample_metadata/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.107352 sample_metadata-5.6.1/sample_metadata/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    32263 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    49430 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.099352 sample_metadata-5.6.1/sample_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 23:58:43.115352 sample_metadata-5.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.115352 sample_metadata-5.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_add_samples_for_joint_calling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_joint_calling_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    26731 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16296 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/testbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.275948 sample_metadata-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-13 10:18:03.275948 sample_metadata-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.255948 sample_metadata-5.7.0/sample_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.259948 sample_metadata-5.7.0/sample_metadata/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61864 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42202 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27906 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53539 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47013 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38773 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/sequence_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37587 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.259948 sample_metadata-5.7.0/sample_metadata/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.259948 sample_metadata-5.7.0/sample_metadata/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/sample_metadata/graphql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.267948 sample_metadata-5.7.0/sample_metadata/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/analysis_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/analysis_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/body_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/body_get_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/body_get_sequences_by_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/nested_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/nested_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/new_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/new_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/participant_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/participant_upsert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/project_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sample_batch_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sample_batch_upsert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sample_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sequence_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sequence_technology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sequence_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/sequence_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82237 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.267948 sample_metadata-5.7.0/sample_metadata/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.267948 sample_metadata-5.7.0/sample_metadata/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/sample_metadata/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/sample_metadata/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32263 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/sample_metadata/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49608 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/sample_metadata/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/sample_metadata/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-04-13 10:16:01.000000 sample_metadata-5.7.0/sample_metadata/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.255948 sample_metadata-5.7.0/sample_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-13 10:18:03.000000 sample_metadata-5.7.0/sample_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-13 10:18:03.000000 sample_metadata-5.7.0/sample_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:18:03.000000 sample_metadata-5.7.0/sample_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:18:03.000000 sample_metadata-5.7.0/sample_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 10:18:03.000000 sample_metadata-5.7.0/sample_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 10:18:03.000000 sample_metadata-5.7.0/sample_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:18:03.275948 sample_metadata-5.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:18:03.271948 sample_metadata-5.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_add_samples_for_joint_calling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_joint_calling_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27410 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16296 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-13 10:13:44.000000 sample_metadata-5.7.0/test/testbase.py
```

### Comparing `sample_metadata-5.6.1/LICENSE` & `sample_metadata-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/PKG-INFO` & `sample_metadata-5.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample_metadata
-Version: 5.6.1
+Version: 5.7.0
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,38 @@
 - An installable python library that wraps the Python web API (using OpenAPI generator)
 
 Every resource in sample-metadata belongs to a project. All resources are access
 controlled through membership of the google groups:
 `$dataset-sample-metadata-main-{read,write}`. Note that members of google-groups
 are cached in a secret as group-membership identity checks are slow.
 
+## API
+
+There are two ways to query metamist in Python:
+
+1. Use the REST interface with the predefined requests
+2. Use the GraphQL interface.
+
+To use the GraphQL interface in Python with the `sample_metadata` library, you can do the following:
+
+```python
+from sample_metadata.graphql import query
+
+_query = """
+query YourQueryNameHere($sampleId: String!) {
+  sample(id: $sampleId) {
+    id
+    externalId
+  }
+}
+"""
+
+print(query(_query, {"sampleId": "CPG18"}))
+```
+
 ## Structure
 
 ![Database structure](resources/2021-10-27_db-diagram.png)
 
 ### Sample IDs
 
 In an effort to reduce our dependency on potentially mutable external sample IDs with inconsistent format,
```

### Comparing `sample_metadata-5.6.1/README.md` & `sample_metadata-5.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,38 @@
 - An installable python library that wraps the Python web API (using OpenAPI generator)
 
 Every resource in sample-metadata belongs to a project. All resources are access
 controlled through membership of the google groups:
 `$dataset-sample-metadata-main-{read,write}`. Note that members of google-groups
 are cached in a secret as group-membership identity checks are slow.
 
+## API
+
+There are two ways to query metamist in Python:
+
+1. Use the REST interface with the predefined requests
+2. Use the GraphQL interface.
+
+To use the GraphQL interface in Python with the `sample_metadata` library, you can do the following:
+
+```python
+from sample_metadata.graphql import query
+
+_query = """
+query YourQueryNameHere($sampleId: String!) {
+  sample(id: $sampleId) {
+    id
+    externalId
+  }
+}
+"""
+
+print(query(_query, {"sampleId": "CPG18"}))
+```
+
 ## Structure
 
 ![Database structure](resources/2021-10-27_db-diagram.png)
 
 ### Sample IDs
 
 In an effort to reduce our dependency on potentially mutable external sample IDs with inconsistent format,
```

### Comparing `sample_metadata-5.6.1/sample_metadata/__init__.py` & `sample_metadata-5.7.0/sample_metadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/analysis_api.py` & `sample_metadata-5.7.0/sample_metadata/api/analysis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/default_api.py` & `sample_metadata-5.7.0/sample_metadata/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/family_api.py` & `sample_metadata-5.7.0/sample_metadata/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/import_api.py` & `sample_metadata-5.7.0/sample_metadata/api/import_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/participant_api.py` & `sample_metadata-5.7.0/sample_metadata/api/participant_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/project_api.py` & `sample_metadata-5.7.0/sample_metadata/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/sample_api.py` & `sample_metadata-5.7.0/sample_metadata/api/sample_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/seqr_api.py` & `sample_metadata-5.7.0/sample_metadata/api/seqr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/sequence_api.py` & `sample_metadata-5.7.0/sample_metadata/api/sequence_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api/web_api.py` & `sample_metadata-5.7.0/sample_metadata/api/web_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/api_client.py` & `sample_metadata-5.7.0/sample_metadata/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `sample_metadata-5.6.1/sample_metadata/apis/__init__.py` & `sample_metadata-5.7.0/sample_metadata/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/sample_metadata/configuration.py` & `sample_metadata-5.7.0/sample_metadata/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -25,14 +25,23 @@
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
 TOKEN_AUDIENCE = 'https://sample-metadata-api-mnrpw3mdza-ts.a.run.app/'
+sm_url = getenv('SM_URL')
+if not sm_url:
+    env = getenv('SM_ENVIRONMENT', 'PRODUCTION')
+    if 'local' in env.lower():
+        sm_url = "http://localhost:8000"
+    elif 'dev' in env.lower():
+        sm_url = 'https://sample-metadata-api-dev-mnrpw3mdza-ts.a.run.app'
+    else:
+        sm_url = 'https://sample-metadata-api-mnrpw3mdza-ts.a.run.app'
 
 class Configuration(object):
     """NOTE: This class is auto generated by OpenAPI Generator
 
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
 
@@ -96,22 +105,15 @@
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ):
         """Constructor
         """
         env = getenv('SM_ENVIRONMENT', 'PRODUCTION')
-        if host is not None:
-            self._base_path = host
-        elif 'local' in env.lower():
-            self._base_path = "http://localhost:8000"
-        elif 'dev' in env.lower():
-            self._base_path = 'https://sample-metadata-api-dev-mnrpw3mdza-ts.a.run.app'
-        else:
-            self._base_path = 'https://sample-metadata-api-mnrpw3mdza-ts.a.run.app'
+        self._base_path = host or sm_url
 
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
@@ -399,15 +401,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 5.6.1\n"\
+               "Version of the API: 5.7.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `sample_metadata-5.6.1/sample_metadata/exceptions.py` & `sample_metadata-5.7.0/sample_metadata/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/analysis_model.py` & `sample_metadata-5.7.0/sample_metadata/model/analysis_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/analysis_query_model.py` & `sample_metadata-5.7.0/sample_metadata/model/analysis_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/analysis_status.py` & `sample_metadata-5.7.0/sample_metadata/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/analysis_type.py` & `sample_metadata-5.7.0/sample_metadata/model/analysis_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/analysis_update_model.py` & `sample_metadata-5.7.0/sample_metadata/model/analysis_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py` & `sample_metadata-5.7.0/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/body_get_participants.py` & `sample_metadata-5.7.0/sample_metadata/model/body_get_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/body_get_samples.py` & `sample_metadata-5.7.0/sample_metadata/model/body_get_samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/body_get_sequences_by_criteria.py` & `sample_metadata-5.7.0/sample_metadata/model/body_get_sequences_by_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/error_response.py` & `sample_metadata-5.7.0/sample_metadata/model/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/export_type.py` & `sample_metadata-5.7.0/sample_metadata/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/extra_participant_importer_handler.py` & `sample_metadata-5.7.0/sample_metadata/model/extra_participant_importer_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/family_search_response_data.py` & `sample_metadata-5.7.0/sample_metadata/model/family_search_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/family_update_model.py` & `sample_metadata-5.7.0/sample_metadata/model/family_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/http_validation_error.py` & `sample_metadata-5.7.0/sample_metadata/model/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/meta_search_entity_prefix.py` & `sample_metadata-5.7.0/sample_metadata/model/meta_search_entity_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/nested_family.py` & `sample_metadata-5.7.0/sample_metadata/model/nested_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/nested_participant.py` & `sample_metadata-5.7.0/sample_metadata/model/nested_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/nested_sample.py` & `sample_metadata-5.7.0/sample_metadata/model/nested_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/nested_sequence.py` & `sample_metadata-5.7.0/sample_metadata/model/nested_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/new_sample.py` & `sample_metadata-5.7.0/sample_metadata/model/new_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/new_sequence.py` & `sample_metadata-5.7.0/sample_metadata/model/new_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/paging_links.py` & `sample_metadata-5.7.0/sample_metadata/model/paging_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/participant_search_response_data.py` & `sample_metadata-5.7.0/sample_metadata/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/participant_update_model.py` & `sample_metadata-5.7.0/sample_metadata/model/participant_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/participant_upsert.py` & `sample_metadata-5.7.0/sample_metadata/model/participant_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/participant_upsert_body.py` & `sample_metadata-5.7.0/sample_metadata/model/participant_upsert_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/project.py` & `sample_metadata-5.7.0/sample_metadata/model/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/project_summary_response.py` & `sample_metadata-5.7.0/sample_metadata/model/project_summary_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sample_batch_upsert.py` & `sample_metadata-5.7.0/sample_metadata/model/sample_batch_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sample_batch_upsert_body.py` & `sample_metadata-5.7.0/sample_metadata/model/sample_batch_upsert_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sample_search_response_data.py` & `sample_metadata-5.7.0/sample_metadata/model/sample_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sample_type.py` & `sample_metadata-5.7.0/sample_metadata/model/sample_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sample_update_model.py` & `sample_metadata-5.7.0/sample_metadata/model/sample_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/search_item.py` & `sample_metadata-5.7.0/sample_metadata/model/search_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/search_response.py` & `sample_metadata-5.7.0/sample_metadata/model/search_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/search_response_model.py` & `sample_metadata-5.7.0/sample_metadata/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/search_response_type.py` & `sample_metadata-5.7.0/sample_metadata/model/search_response_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sequence_status.py` & `sample_metadata-5.7.0/sample_metadata/model/sequence_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sequence_technology.py` & `sample_metadata-5.7.0/sample_metadata/model/sequence_technology.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sequence_type.py` & `sample_metadata-5.7.0/sample_metadata/model/sequence_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sequence_update_model.py` & `sample_metadata-5.7.0/sample_metadata/model/sequence_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/sequence_upsert.py` & `sample_metadata-5.7.0/sample_metadata/model/sequence_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/validation_error.py` & `sample_metadata-5.7.0/sample_metadata/model/validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model/web_project.py` & `sample_metadata-5.7.0/sample_metadata/model/web_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.1/sample_metadata/model_utils.py` & `sample_metadata-5.7.0/sample_metadata/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `sample_metadata-5.6.1/sample_metadata/models/__init__.py` & `sample_metadata-5.7.0/sample_metadata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/sample_metadata/parser/cloudhelper.py` & `sample_metadata-5.7.0/sample_metadata/parser/cloudhelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=no-member
 import os
 import logging
 from typing import Iterable, Callable, TypeVar
 from collections import defaultdict
+from datetime import datetime
 
 from cloudpathlib import AnyPath, GSPath
 from google.cloud import storage
 
 
 # type declarations for GroupBy
 T = TypeVar('T')
@@ -122,14 +123,29 @@
 
         return AnyPath(path).exists()
 
     async def file_size(self, filename) -> int:
         """Get size of file in bytes"""
         return AnyPath(self.file_path(filename)).stat().st_size
 
+    async def datetime_added(self, filename) -> datetime | None:
+        """Get the date and time the file was created"""
+        path = self.file_path(filename)
+        if path.startswith('gs://'):
+            # add a specific case for GCS as the AnyPath implementation calls
+            # bucket.get_blob which triggers a read (which humans are not permitted)
+            blob = await self.get_gcs_blob(path)
+            return blob.time_created
+
+        ctime = AnyPath(path).stat().st_ctime
+        if not ctime:
+            return None
+
+        return datetime.utcfromtimestamp(ctime)
+
     def populate_filename_map(self, search_locations: list[str]) -> dict[str, str]:
         """
         FileMapParser uses search locations based on the filename,
         so let's prepopulate that filename_map from the search_locations!
         """
 
         fn_map: dict[str, str] = {}
```

### Comparing `sample_metadata-5.6.1/sample_metadata/parser/generic_metadata_parser.py` & `sample_metadata-5.7.0/sample_metadata/parser/generic_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/sample_metadata/parser/generic_parser.py` & `sample_metadata-5.7.0/sample_metadata/parser/generic_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1217,31 +1217,33 @@
         filename: str,
         secondary_files: List[SingleRow] = None,
         checksum: Optional[str] = None,
     ) -> SingleRow:
         """Takes filename, returns formed CWL dictionary"""
         _checksum = checksum
         file_size = None
+        datetime_added = None
 
         if not self.skip_checking_gcs_objects:
             if not _checksum:
                 md5_filename = self.file_path(filename + '.md5')
                 if await self.file_exists(md5_filename):
                     contents = await self.file_contents(md5_filename)
                     if contents:
                         _checksum = f'md5:{contents.strip()}'
 
-            file_size = await self.file_size(filename)
+            file_size, datetime_added = await asyncio.gather(self.file_size(filename), self.datetime_added(filename))
 
         d = {
             'location': self.file_path(filename),
             'basename': os.path.basename(filename),
             'class': 'File',
             'checksum': _checksum,
             'size': file_size,
+            'datetime_added': datetime_added.isoformat() if datetime_added else None
         }
 
         if secondary_files:
             d['secondaryFiles'] = secondary_files
 
         return d
```

### Comparing `sample_metadata-5.6.1/sample_metadata/parser/sample_file_map_parser.py` & `sample_metadata-5.7.0/sample_metadata/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/sample_metadata/rest.py` & `sample_metadata-5.7.0/sample_metadata/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.1
+    The version of the OpenAPI document: 5.7.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `sample_metadata-5.6.1/sample_metadata.egg-info/PKG-INFO` & `sample_metadata-5.7.0/sample_metadata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-metadata
-Version: 5.6.1
+Version: 5.7.0
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,38 @@
 - An installable python library that wraps the Python web API (using OpenAPI generator)
 
 Every resource in sample-metadata belongs to a project. All resources are access
 controlled through membership of the google groups:
 `$dataset-sample-metadata-main-{read,write}`. Note that members of google-groups
 are cached in a secret as group-membership identity checks are slow.
 
+## API
+
+There are two ways to query metamist in Python:
+
+1. Use the REST interface with the predefined requests
+2. Use the GraphQL interface.
+
+To use the GraphQL interface in Python with the `sample_metadata` library, you can do the following:
+
+```python
+from sample_metadata.graphql import query
+
+_query = """
+query YourQueryNameHere($sampleId: String!) {
+  sample(id: $sampleId) {
+    id
+    externalId
+  }
+}
+"""
+
+print(query(_query, {"sampleId": "CPG18"}))
+```
+
 ## Structure
 
 ![Database structure](resources/2021-10-27_db-diagram.png)
 
 ### Sample IDs
 
 In an effort to reduce our dependency on potentially mutable external sample IDs with inconsistent format,
```

### Comparing `sample_metadata-5.6.1/sample_metadata.egg-info/SOURCES.txt` & `sample_metadata-5.7.0/sample_metadata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 sample_metadata/api/participant_api.py
 sample_metadata/api/project_api.py
 sample_metadata/api/sample_api.py
 sample_metadata/api/seqr_api.py
 sample_metadata/api/sequence_api.py
 sample_metadata/api/web_api.py
 sample_metadata/apis/__init__.py
+sample_metadata/graphql/__init__.py
 sample_metadata/model/__init__.py
 sample_metadata/model/analysis_model.py
 sample_metadata/model/analysis_query_model.py
 sample_metadata/model/analysis_status.py
 sample_metadata/model/analysis_type.py
 sample_metadata/model/analysis_update_model.py
 sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py
```

### Comparing `sample_metadata-5.6.1/setup.py` & `sample_metadata-5.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='5.6.1',
+    version='5.7.0',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/sample-metadata',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `sample_metadata-5.6.1/test/test_add_samples_for_joint_calling.py` & `sample_metadata-5.7.0/test/test_add_samples_for_joint_calling.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_analysis.py` & `sample_metadata-5.7.0/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_get_participants.py` & `sample_metadata-5.7.0/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_import_individual_metadata.py` & `sample_metadata-5.7.0/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_joint_calling_workflow.py` & `sample_metadata-5.7.0/test/test_joint_calling_workflow.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_parse_file_map.py` & `sample_metadata-5.7.0/test/test_parse_file_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,21 +64,23 @@
                 [
                     {
                         'location': 'gs://BUCKET/FAKE/<sample-id>.filename-R1.fastq.gz',
                         'basename': '<sample-id>.filename-R1.fastq.gz',
                         'class': 'File',
                         'checksum': None,
                         'size': None,
+                        'datetime_added': None,
                     },
                     {
                         'location': 'gs://BUCKET/FAKE/<sample-id>.filename-R2.fastq.gz',
                         'basename': '<sample-id>.filename-R2.fastq.gz',
                         'class': 'File',
                         'checksum': None,
                         'size': None,
+                        'datetime_added': None,
                     },
                 ]
             ],
             'reads_type': 'fastq',
         }
         self.assertEqual('short-read', str(sequencing_to_add[0].technology))
         self.assertDictEqual(expected_sequence_dict, sequencing_to_add[0].meta)
@@ -141,40 +143,44 @@
         expected_sequence1_reads = [
             {
                 'location': 'gs://BUCKET/FAKE/<sample-id>.filename-R1.fastq.gz',
                 'basename': '<sample-id>.filename-R1.fastq.gz',
                 'class': 'File',
                 'checksum': '<checksum>',
                 'size': None,
+                'datetime_added': None,
             },
             {
                 'location': 'gs://BUCKET/FAKE/<sample-id>.filename-R2.fastq.gz',
                 'basename': '<sample-id>.filename-R2.fastq.gz',
                 'class': 'File',
                 'checksum': '<checksum2>',
                 'size': None,
+                'datetime_added': None,
             },
         ]
 
         self.assertListEqual(
             expected_sequence1_reads, sequencing_to_add[0].meta['reads'][0]
         )
 
         expected_sequence2_reads = [
             {
                 'location': 'gs://BUCKET/FAKE/<sample-id2>.filename-R1.fastq.gz',
                 'basename': '<sample-id2>.filename-R1.fastq.gz',
                 'class': 'File',
                 'checksum': '<checksum3>',
                 'size': None,
+                'datetime_added': None,
             },
             {
                 'location': 'gs://BUCKET/FAKE/<sample-id2>.filename-R2.fastq.gz',
                 'basename': '<sample-id2>.filename-R2.fastq.gz',
                 'class': 'File',
                 'checksum': '<checksum4>',
                 'size': None,
+                'datetime_added': None,
             },
         ]
         self.assertListEqual(
             expected_sequence2_reads, sequencing_to_add[1].meta['reads'][0]
         )
```

### Comparing `sample_metadata-5.6.1/test/test_parse_generic_metadata.py` & `sample_metadata-5.7.0/test/test_parse_generic_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+from datetime import datetime
 from io import StringIO
 from unittest.mock import patch
 from test.testbase import run_as_sync
 
 from sample_metadata.parser.generic_metadata_parser import GenericMetadataParser
 
 
@@ -75,28 +76,35 @@
             self.assertEqual(
                 "Key 'extra' not found in provided key map: fn, sample", str(e)
             )
 
     @run_as_sync
     @patch('sample_metadata.apis.SampleApi.get_sample_id_map_by_external')
     @patch('sample_metadata.apis.SequenceApi.get_sequence_ids_for_sample_ids_by_type')
+    @patch('sample_metadata.parser.cloudhelper.CloudHelper.datetime_added')
     @patch('sample_metadata.parser.cloudhelper.CloudHelper.file_exists')
     @patch('sample_metadata.parser.cloudhelper.CloudHelper.file_size')
     async def test_single_row(
-        self, mock_filesize, mock_fileexists, mock_get_sequence_ids, mock_get_sample_id
+        self,
+        mock_filesize,
+        mock_fileexists,
+        mock_datetime_added,
+        mock_get_sequence_ids,
+        mock_get_sample_id,
     ):
         """
         Test importing a single row, forms objects and checks response
         - MOCKS: get_sample_id_map_by_external, get_sequence_ids_for_sample_ids_by_type
         """
         mock_get_sample_id.return_value = {}
         mock_get_sequence_ids.return_value = {}
 
         mock_filesize.return_value = 111
         mock_fileexists.return_value = False
+        mock_datetime_added.return_value = datetime.fromisoformat('2022-02-02T22:22:22')
 
         rows = [
             'GVCF\tCRAM\tSampleId\tsample.flowcell_lane\tsample.platform\tsample.centre\tsample.reference_genome\traw_data.FREEMIX\traw_data.PCT_CHIMERAS\traw_data.MEDIAN_INSERT_SIZE\traw_data.MEDIAN_COVERAGE',
             '<sample-id>.g.vcf.gz\t<sample-id>.bam\t<sample-id>\tHK7NFCCXX.1\tILLUMINA\tKCCG\thg38\t0.01\t0.01\t400\t30',
         ]
         parser = GenericMetadataParser(
             search_locations=[],
@@ -152,24 +160,26 @@
             'reads': [
                 {
                     'location': '/path/to/<sample-id>.bam',
                     'basename': '<sample-id>.bam',
                     'class': 'File',
                     'checksum': None,
                     'size': 111,
+                    'datetime_added': '2022-02-02T22:22:22',
                 }
             ],
             'reads_type': 'bam',
             'gvcfs': [
                 {
                     'location': '/path/to/<sample-id>.g.vcf.gz',
                     'basename': '<sample-id>.g.vcf.gz',
                     'class': 'File',
                     'checksum': None,
                     'size': 111,
+                    'datetime_added': '2022-02-02T22:22:22',
                 }
             ],
             'gvcf_types': 'gvcf',
         }
         self.assertDictEqual(expected_sequence_dict, sequences_to_add[0].meta)
         analysis = analyses_to_add['<sample-id>'][0]
         self.assertDictEqual(
@@ -262,21 +272,23 @@
                 [
                     {
                         'basename': 'sample_id001.filename-R1.fastq.gz',
                         'checksum': None,
                         'class': 'File',
                         'location': '/path/to/sample_id001.filename-R1.fastq.gz',
                         'size': None,
+                        'datetime_added': None,
                     },
                     {
                         'basename': 'sample_id001.filename-R2.fastq.gz',
                         'checksum': None,
                         'class': 'File',
                         'location': '/path/to/sample_id001.filename-R2.fastq.gz',
                         'size': None,
+                        'datetime_added': None,
                     },
                 ]
             ],
             'reads_type': 'fastq',
         }
         self.assertDictEqual(expected_sequence_dict, sequences_to_add[0].meta)
 
@@ -437,14 +449,15 @@
             reads_column='Filename',
             participant_meta_map={},
             sample_meta_map={},
             sequence_meta_map={},
             qc_meta_map={},
             # doesn't matter, we're going to mock the call anyway
             project='devdev',
+            skip_checking_gcs_objects=True,
         )
 
         parser.filename_map = {'file.cram': 'gs://path/file.cram'}
 
         # Call generic parser
         file_contents = '\n'.join(rows)
         with self.assertRaises(ValueError) as ctx:
@@ -511,21 +524,23 @@
 
         expected = {
             'location': 'gs://path/file.fasta',
             'basename': 'file.fasta',
             'class': 'File',
             'checksum': None,
             'size': None,
+            'datetime_added': None,
             'secondaryFiles': [
                 {
                     'location': 'gs://path/file.fasta.fai',
                     'basename': 'file.fasta.fai',
                     'class': 'File',
                     'checksum': None,
                     'size': None,
+                    'datetime_added': None,
                 }
             ],
         }
 
         self.assertDictEqual(
             expected,
             resp['sequences']['insert'][0]['meta']['reference_assembly'],
@@ -585,21 +600,23 @@
 
         expected = {
             'location': 'gs://path/ref.fa',
             'basename': 'ref.fa',
             'class': 'File',
             'checksum': None,
             'size': None,
+            'datetime_added': None,
             'secondaryFiles': [
                 {
                     'location': 'gs://path/ref.fa.fai',
                     'basename': 'ref.fa.fai',
                     'class': 'File',
                     'checksum': None,
                     'size': None,
+                    'datetime_added': None,
                 }
             ],
         }
 
         self.assertDictEqual(
             expected,
             resp['sequences']['insert'][0]['meta']['reference_assembly'],
```

### Comparing `sample_metadata-5.6.1/test/test_parse_ont_processor.py` & `sample_metadata-5.7.0/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_parse_ont_sheet.py` & `sample_metadata-5.7.0/test/test_parse_ont_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
                 [
                     {
                         'location': 'gs://BUCKET/FAKE/Sample01_fail.fastq.gz',
                         'basename': 'Sample01_fail.fastq.gz',
                         'class': 'File',
                         'checksum': None,
                         'size': None,
+                        'datetime_added': None,
                     }
                 ]
             ],
             'flow_cell': 'PRO002',
             'flowcell_id': 'XYZ1',
             'mux_total': '7107',
             'protocol': 'LSK1',
@@ -92,14 +93,15 @@
                 [
                     {
                         'basename': 'Sample01_pass.fastq.gz',
                         'checksum': None,
                         'class': 'File',
                         'location': 'gs://BUCKET/FAKE/Sample01_pass.fastq.gz',
                         'size': None,
+                        'datetime_added': None,
                     }
                 ]
             ],
             'reads_type': 'fastq',
             'sequencing_date': '10/12/2034',
         }
```

### Comparing `sample_metadata-5.6.1/test/test_pedigree.py` & `sample_metadata-5.7.0/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_sample.py` & `sample_metadata-5.7.0/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_search.py` & `sample_metadata-5.7.0/test/test_search.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_sequence.py` & `sample_metadata-5.7.0/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_upsert.py` & `sample_metadata-5.7.0/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/test_web.py` & `sample_metadata-5.7.0/test/test_web.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.1/test/testbase.py` & `sample_metadata-5.7.0/test/testbase.py`

 * *Files identical despite different names*

