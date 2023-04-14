# Comparing `tmp/credsweeper-1.4.8.tar.gz` & `tmp/credsweeper-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credsweeper-1.4.8.tar", last modified: Fri Feb  3 09:03:52 2023, max compression
+gzip compressed data, was "credsweeper-1.4.9.tar", last modified: Fri Mar  3 10:05:50 2023, max compression
```

## Comparing `credsweeper-1.4.8.tar` & `credsweeper-1.4.9.tar`

### file list

```diff
@@ -1,119 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.304062 credsweeper-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-03 09:03:42.000000 credsweeper-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-02-03 09:03:52.304062 credsweeper-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-02-03 09:03:42.000000 credsweeper-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.296062 credsweeper-1.4.8/credsweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29835 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.296062 credsweeper-1.4.8/credsweeper/common/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/common/keyword_checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/common/keyword_checklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.296062 credsweeper-1.4.8/credsweeper/config/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.296062 credsweeper-1.4.8/credsweeper/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/credentials/candidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/credentials/candidate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/credentials/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/credentials/line_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.296062 credsweeper-1.4.8/credsweeper/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/files_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/patch_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/text_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/file_handler/text_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.300063 credsweeper-1.4.8/credsweeper/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.300063 credsweeper-1.4.8/credsweeper/filters/group/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/group/pem_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_entropy_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_method_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/filters/variable_not_allowed_pattern_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.300063 credsweeper-1.4.8/credsweeper/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.300063 credsweeper-1.4.8/credsweeper/ml_model/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/ml_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/ml_model/features.py
--rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/ml_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.300063 credsweeper-1.4.8/credsweeper/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/rules/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.300063 credsweeper-1.4.8/credsweeper/scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.304062 credsweeper-1.4.8/credsweeper/scanner/scan_type/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.304062 credsweeper-1.4.8/credsweeper/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/secret/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/secret/log.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.304062 credsweeper-1.4.8/credsweeper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.304062 credsweeper-1.4.8/credsweeper/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/apply_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/github_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-03 09:03:42.000000 credsweeper-1.4.8/credsweeper/validations/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 09:03:52.296062 credsweeper-1.4.8/credsweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-02-03 09:03:52.000000 credsweeper-1.4.8/credsweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-02-03 09:03:52.000000 credsweeper-1.4.8/credsweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 09:03:52.000000 credsweeper-1.4.8/credsweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-03 09:03:52.000000 credsweeper-1.4.8/credsweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-03 09:03:52.000000 credsweeper-1.4.8/credsweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-03 09:03:52.000000 credsweeper-1.4.8/credsweeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-03 09:03:52.304062 credsweeper-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-02-03 09:03:42.000000 credsweeper-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.888596 credsweeper-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-03 10:05:41.000000 credsweeper-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-03-03 10:05:50.888596 credsweeper-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-03-03 10:05:41.000000 credsweeper-1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/common/keyword_checklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/line_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.876596 credsweeper-1.4.9/credsweeper/deep_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/deep_scaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/zip_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.876596 credsweeper-1.4.9/credsweeper/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/patch_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/text_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/text_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.880596 credsweeper-1.4.9/credsweeper/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/cred_card_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.880596 credsweeper-1.4.9/credsweeper/filters/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/credit_card_number_sequense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/pem_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_entropy_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_method_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/variable_not_allowed_pattern_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.880596 credsweeper-1.4.9/credsweeper/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/ml_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/rules/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/scanner/scan_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/secret/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/secret/log.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.888596 credsweeper-1.4.9/credsweeper/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/apply_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-03 10:05:50.888596 credsweeper-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-03 10:05:41.000000 credsweeper-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.888596 credsweeper-1.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27535 2023-03-03 10:05:41.000000 credsweeper-1.4.9/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34004 2023-03-03 10:05:41.000000 credsweeper-1.4.9/tests/test_main.py
```

### Comparing `credsweeper-1.4.8/LICENSE` & `credsweeper-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/PKG-INFO` & `credsweeper-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.4.8
+Version: 1.4.9
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.4.8/README.md` & `credsweeper-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/__init__.py` & `credsweeper-1.4.9/credsweeper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     'ThresholdPreset',  #
     'CREDSWEEPER_DIR',  #
     '__version__'
 ]
 
 CREDSWEEPER_DIR = Path(__file__).resolve().parent
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
```

### Comparing `credsweeper-1.4.8/credsweeper/__main__.py` & `credsweeper-1.4.9/credsweeper/__main__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/common/constants.py` & `credsweeper-1.4.9/credsweeper/common/constants.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/common/keyword_checklist.py` & `credsweeper-1.4.9/credsweeper/common/keyword_checklist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
-from typing import List
+from typing import List, Set
 
-from credsweeper.common.constants import DEFAULT_ENCODING
+from credsweeper.utils import Util
 
 
 class KeywordChecklist:
     __keyword_list: List[str] = []
 
     def __init__(self) -> None:
         dir_path = os.path.dirname(os.path.realpath(__file__))
-        with open(os.path.join(dir_path, "keyword_checklist.txt"), "r", encoding=DEFAULT_ENCODING) as f:
-            self.set_list(f.read().splitlines())
+        file_path = os.path.join(dir_path, "keyword_checklist.txt")
+        self.set_list(Util.read_file(file_path))
 
     def get_list(self) -> List[str]:
         """Get list with keywords.
 
         Return:
             List of strings
 
@@ -24,8 +24,12 @@
     def set_list(self, keyword_list: List[str]) -> None:
         """Remove old keywords and setup new one.
 
         Args:
             keyword_list: list of keywords to be added
 
         """
-        self.__keyword_list = keyword_list
+        keyword_set: Set[str] = set()
+        for i in keyword_list:
+            if 3 <= len(i):
+                keyword_set.add(i)
+        self.__keyword_list = list(keyword_set)
```

### Comparing `credsweeper-1.4.8/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.4.9/credsweeper/common/keyword_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/config/config.py` & `credsweeper-1.4.9/credsweeper/config/config.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/credentials/candidate.py` & `credsweeper-1.4.9/credsweeper/credentials/candidate.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.4.9/credsweeper/credentials/candidate_group_generator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/credentials/candidate_key.py` & `credsweeper-1.4.9/credsweeper/credentials/candidate_key.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/credentials/credential_manager.py` & `credsweeper-1.4.9/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/credentials/line_data.py` & `credsweeper-1.4.9/credsweeper/credentials/line_data.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/file_handler/__init__.py` & `credsweeper-1.4.9/credsweeper/file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.4.9/credsweeper/file_handler/byte_content_provider.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,15 +16,38 @@
             info: Optional[str] = None) -> None:
         """
         Parameters:
             content: The bytes are transformed to an array of lines with split by new line character.
 
         """
         super().__init__(file_path=file_path, file_type=file_type, info=info)
-        self.lines = Util.decode_bytes(content)
+        self.data = content
+        self.__lines: Optional[List[str]] = None
+
+    @property
+    def data(self) -> Optional[bytes]:
+        """data getter for ByteContentProvider"""
+        return self.__data
+
+    @data.setter
+    def data(self, data: Optional[bytes]) -> None:
+        """data setter for ByteContentProvider"""
+        self.__data = data
+
+    @property
+    def lines(self) -> List[str]:
+        """lines getter for ByteContentProvider"""
+        if self.__lines is None:
+            self.__lines = Util.decode_bytes(self.__data)
+        return self.__lines if self.__lines is not None else []
+
+    @lines.setter
+    def lines(self, lines: List[str]) -> None:
+        """lines setter for ByteContentProvider"""
+        self.__lines = lines
 
     def get_analysis_target(self) -> List[AnalysisTarget]:
         """Return lines to scan.
 
         Return:
             list of analysis targets based on every row in a content
```

### Comparing `credsweeper-1.4.8/credsweeper/file_handler/content_provider.py` & `credsweeper-1.4.9/credsweeper/file_handler/content_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import ABC, abstractmethod
+from abc import ABC, abstractmethod, abstractproperty
 from typing import List, Optional
 
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.utils import Util
 
 
 class ContentProvider(ABC):
@@ -60,14 +60,25 @@
         return self.__info
 
     @info.setter
     def info(self, _info: str) -> None:
         """info getter"""
         self.__info = _info if _info else ""
 
+    @abstractproperty
+    def data(self) -> Optional[bytes]:
+        """abstract data getter"""
+        raise NotImplementedError(__name__)
+
+    @data.setter
+    @abstractmethod
+    def data(self, data: Optional[bytes]) -> None:
+        """abstract data setter"""
+        raise NotImplementedError(__name__)
+
     def lines_to_targets(self, lines: List[str], line_nums: Optional[List[int]] = None) -> List[AnalysisTarget]:
         """Creates list of targets with multiline concatenation"""
         targets = []
         if line_nums:
             for line, line_num in zip(lines, line_nums):
                 target = AnalysisTarget(line, line_num, lines, self.file_path, self.file_type, self.info)
                 targets.append(target)
```

### Comparing `credsweeper-1.4.8/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.4.9/credsweeper/file_handler/diff_content_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,24 @@
             file_path: str,  #
             change_type: DiffRowType,  #
             diff: List[DiffDict]) -> None:
         super().__init__(file_path=file_path, info=change_type.value)
         self.change_type = change_type
         self.diff = diff
 
+    @property
+    def data(self) -> bytes:
+        """data getter for DiffContentProvider"""
+        raise NotImplementedError(__name__)
+
+    @data.setter
+    def data(self, data: bytes) -> None:
+        """data setter for DiffContentProvider"""
+        raise NotImplementedError(__name__)
+
     def parse_lines_data(self, lines_data: List[DiffRowData]) -> Tuple[List[int], List[str]]:
         """Parse diff lines data.
 
         Return list of line numbers with change type "self.change_type" and list of all lines in file
             in original order(replaced all lines not mentioned in diff file with blank line)
 
         Args:
@@ -77,10 +87,10 @@
                     l_numb,  #
                     all_lines,  #
                     self.file_path,  #
                     self.file_type,  #
                     self.change_type.value)  #
                 for l_numb in change_numbs
             ]
-        except OverflowError as exc:
-            logger.exception(exc)
+        except Exception as exc:
+            logger.error(f"Wrong diff {type(exc)} {exc}")
         return []
```

### Comparing `credsweeper-1.4.8/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.4.9/credsweeper/file_handler/file_path_extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import io
 import logging
 import os
 from pathlib import Path
-from typing import List, Dict
+from typing import List, Dict, Union, Tuple
 
 from git import InvalidGitRepositoryError, NoSuchPathError, Repo
 
 from credsweeper.config import Config
 from credsweeper.utils import Util
 
 logger = logging.getLogger(__name__)
@@ -28,15 +29,15 @@
 
         """
         filtered_files = [file_path for file_path in detected_files if FilePathExtractor.is_valid_path(file_path)]
 
         return filtered_files
 
     @classmethod
-    def get_file_paths(cls, config: Config, path: str) -> List[str]:
+    def get_file_paths(cls, config: Config, path: Union[str, Path]) -> List[str]:
         """Get all files in the directory. Automatically exclude files non-code or data files (such as .jpg).
 
         Args:
             config: credsweeper configuration
             path: path to the file or directory to be scanned
 
         Return:
@@ -134,26 +135,40 @@
         if file_extension in config.exclude_extensions:
             return True
         if not config.depth and file_extension in config.exclude_containers:
             return True
         return False
 
     @classmethod
-    def check_file_size(cls, config: Config, path: str) -> bool:
+    def check_file_size(
+            cls,  #
+            config: Config,  #
+            reference: Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]) -> bool:
         """
         Checks whether the file is oversize limit
 
         Args:
             config: Config
-            path: str - acceptable file
+            reference: various types of a file reference
 
         Return:
             True when the file is oversize
         """
         if config.size_limit is None:
             return False
-        file_size = os.path.getsize(path)
-        if file_size > config.size_limit:
+        file_size = None
+        path = reference[1] if isinstance(reference, tuple) else reference
+        if isinstance(path, str) or isinstance(path, Path):
+            file_size = os.path.getsize(path)
+        elif isinstance(path, io.BytesIO):
+            current_pos = path.tell()
+            path.seek(0, io.SEEK_END)
+            file_size = path.tell() - current_pos
+            path.seek(current_pos, io.SEEK_SET)
+        else:
+            logger.error(f"Unknown path type: {path}")
+
+        if file_size and file_size > config.size_limit:
             logger.warning(f"Size ({file_size}) of the file '{path}' is over limit ({config.size_limit})")
             return True
-        else:
-            return False
+
+        return False
```

### Comparing `credsweeper-1.4.8/credsweeper/file_handler/files_provider.py` & `credsweeper-1.4.9/credsweeper/file_handler/files_provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,41 @@
+import io
 from abc import ABC, abstractmethod
-from typing import List, Optional, Union
+from pathlib import Path
+from typing import List, Union, Tuple
 
 from credsweeper.config import Config
 from credsweeper.file_handler.diff_content_provider import DiffContentProvider
 from credsweeper.file_handler.text_content_provider import TextContentProvider
 
 
 class FilesProvider(ABC):
-    """Base class for all files provider objects.
+    """Base class for all files provider objects."""
 
-    Parameters:
-        paths: list of paths to scan
-        change_type: type of analyses changes in patch (added or deleted)
-        skip_ignored: Checking the directory to the list
-            of ignored directories from the gitignore file
-
-    """
-
-    @abstractmethod
-    def __init__(self,
-                 paths: List[str],
-                 change_type: Optional[str] = None,
-                 skip_ignored: Optional[bool] = None) -> None:
+    def __init__(self, paths: List[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]]) -> None:
         """Initialize Files Provider object for 'paths'.
 
         Args:
-            paths: file paths list to scan
-            change_type: type of analyses changes in patch (added or deleted)
-            skip_ignored: Checking the directory to the list
-                of ignored directories from the gitignore file
+            paths: file paths list to scan or io.BytesIO or tuple with both
 
         """
-        raise NotImplementedError()
+        self.paths = paths
+
+    @property
+    def paths(self) -> List[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]]:
+        """paths getter"""
+        return self.__paths
+
+    @paths.setter
+    def paths(self, paths: List[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]]) -> None:
+        """paths setter"""
+        self.__paths = paths
 
     @abstractmethod
-    def get_scannable_files(self, config: Config) -> Union[List[DiffContentProvider], List[TextContentProvider]]:
+    def get_scannable_files(self, config: Config) -> List[Union[DiffContentProvider, TextContentProvider]]:
         """Get list of file object for analysis based on attribute "paths".
 
         Args:
             config: dict of credsweeper configuration
 
         Return:
             file objects to analyse
```

### Comparing `credsweeper-1.4.8/credsweeper/file_handler/patch_provider.py` & `credsweeper-1.4.9/credsweeper/file_handler/patch_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,76 @@
-from typing import List, Optional, Union
+import io
+import logging
+from pathlib import Path
+from typing import List, Union, Tuple
 
 from credsweeper import TextContentProvider
 from credsweeper.common.constants import DiffRowType
 from credsweeper.config import Config
 from credsweeper.file_handler.diff_content_provider import DiffContentProvider
 from credsweeper.file_handler.file_path_extractor import FilePathExtractor
 from credsweeper.file_handler.files_provider import FilesProvider
 from credsweeper.utils import Util
 
+logger = logging.getLogger(__name__)
+
 
 class PatchProvider(FilesProvider):
     """Provide data from a list of `.patch` files.
 
     Allows to scan for data that has changed between git commits, rather than the entire project.
 
     Parameters:
         paths: file paths list to scan. All files should be in `.patch` format
         change_type: string, type of analyses changes in patch (added or deleted)
         skip_ignored: boolean variable, Checking the directory to the list
           of ignored directories from the gitignore file
 
     """
 
-    def __init__(
-            self,  #
-            paths: List[str],  #
-            change_type: DiffRowType,  #
-            skip_ignored: Optional[bool] = None) -> None:
+    def __init__(self, paths: List[Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]],
+                 change_type: DiffRowType) -> None:
         """Initialize Files Patch Provider for patch files from 'paths'.
 
         Args:
             paths: file paths list to scan. All files should be in `.patch` format
             change_type: string, type of analyses changes in patch (added or deleted)
             skip_ignored: boolean variable, Checking the directory to the list
               of ignored directories from the gitignore file
 
         """
-        self.paths = paths
+        super().__init__(paths)
         self.change_type = change_type
 
     def load_patch_data(self, config: Config) -> List[List[str]]:
         """Loads data from patch"""
         raw_patches = []
         for file_path in self.paths:
             if FilePathExtractor.check_file_size(config, file_path):
                 continue
-            raw_patches.append(Util.read_file(file_path))
+            if isinstance(file_path, str) or isinstance(file_path, Path):
+                raw_patches.append(Util.read_file(file_path))
+            elif isinstance(file_path, io.BytesIO):
+                the_patch = Util.decode_bytes(file_path.read())
+                raw_patches.append(the_patch)
+            else:
+                logger.error(f"Unknown path type: {file_path}")
+
         return raw_patches
 
-    def get_files_sequence(self, raw_patches: List[List[str]]) -> List[DiffContentProvider]:
+    def get_files_sequence(self, raw_patches: List[List[str]]) -> List[Union[DiffContentProvider, TextContentProvider]]:
         """Returns sequence of files"""
-        files = []
+        files: List[Union[DiffContentProvider, TextContentProvider]] = []
         for raw_patch in raw_patches:
             files_data = Util.patch2files_diff(raw_patch, self.change_type)
             for file_path, file_diff in files_data.items():
                 files.append(DiffContentProvider(file_path=file_path, change_type=self.change_type, diff=file_diff))
         return files
 
-    def get_scannable_files(self, config: Config) -> Union[List[DiffContentProvider], List[TextContentProvider]]:
+    def get_scannable_files(self, config: Config) -> List[Union[DiffContentProvider, TextContentProvider]]:
         """Get files to scan. Output based on the `paths` field.
 
         Args:
             config: dict of credsweeper configuration
 
         Return:
             file objects for analysing
```

### Comparing `credsweeper-1.4.8/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.4.9/credsweeper/file_handler/string_content_provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,14 +23,24 @@
         """
         super().__init__(file_path=file_path, file_type=file_type, info=info)
         self.lines = lines
         # fill line numbers only when amounts are equal
         self.line_numbers = line_numbers if line_numbers and len(self.lines) == len(line_numbers) \
             else (list(range(1, 1 + len(self.lines))) if self.lines else [])
 
+    @property
+    def data(self) -> bytes:
+        """data getter for StringContentProvider"""
+        raise NotImplementedError(__name__)
+
+    @data.setter
+    def data(self, data: bytes) -> None:
+        """data setter for StringContentProvider"""
+        raise NotImplementedError(__name__)
+
     def get_analysis_target(self) -> List[AnalysisTarget]:
         """Return lines to scan.
 
         Return:
             list of analysis targets based on every row in file
 
         """
```

### Comparing `credsweeper-1.4.8/credsweeper/file_handler/struct_content_provider.py` & `credsweeper-1.4.9/credsweeper/file_handler/struct_content_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,24 @@
         return self.__struct
 
     @struct.setter
     def struct(self, struct: Any) -> None:
         """obj setter"""
         self.__struct = struct
 
+    @property
+    def data(self) -> bytes:
+        """data getter for StructContentProvider"""
+        raise NotImplementedError(__name__)
+
+    @data.setter
+    def data(self, data: bytes) -> None:
+        """data setter for StructContentProvider"""
+        raise NotImplementedError(__name__)
+
     def get_analysis_target(self) -> List[AnalysisTarget]:
         """Return nothing. The class provides only data storage.
 
         Raise:
             NotImplementedError
 
         """
```

### Comparing `credsweeper-1.4.8/credsweeper/filters/__init__.py` & `credsweeper-1.4.9/credsweeper/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/group/group.py` & `credsweeper-1.4.9/credsweeper/filters/group/group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.4.9/credsweeper/filters/group/url_credentials_group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.4.9/credsweeper/filters/line_specific_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.4.9/credsweeper/filters/separator_unusual_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_allowlist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_array_dictionary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_blocklist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_camel_case_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_dictionary_keyword_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_dictionary_value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_entropy_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_entropy_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_file_path_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_first_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_last_word_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_last_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_length_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_method_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_method_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_similarity_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_string_type_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_token_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.4.9/credsweeper/filters/value_useless_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/filters/variable_not_allowed_pattern_check.py` & `credsweeper-1.4.9/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/logger/logger.py` & `credsweeper-1.4.9/credsweeper/logger/logger.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/ml_model/features.py` & `credsweeper-1.4.9/credsweeper/ml_model/features.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/ml_model/ml_model.onnx` & `credsweeper-1.4.9/credsweeper/ml_model/ml_model.onnx`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.4.9/credsweeper/ml_model/ml_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/ml_model/model_config.json` & `credsweeper-1.4.9/credsweeper/ml_model/model_config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/rules/config.yaml` & `credsweeper-1.4.9/credsweeper/rules/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+- name: Credit card number
+  severity: medium
+  type: pattern
+  values:
+    - (?<!([0-9]\.|[=*+\/\-] |.[=*+\/\-]))((?<![0-9A-Za-z_=*+\-\/.])(?P<value>[0-9]{16})(?![0-9A-Za-z_=*+\-\/.]))(?!(\.[0-9]| [=*+\/\-]|.[=*+\/\-]))
+  filter_type: CreditCardNumberSequence
+  use_ml: false
+  validations: []
+  min_line_len: 16
+
 - name: API
   severity: medium
   type: keyword
   values:
     - api
   filter_type: GeneralKeyword
   use_ml: true
```

### Comparing `credsweeper-1.4.8/credsweeper/rules/rule.py` & `credsweeper-1.4.9/credsweeper/rules/rule.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.4.9/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/scanner/scan_type/pem_key_pattern.py` & `credsweeper-1.4.9/credsweeper/scanner/scan_type/pem_key_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.4.9/credsweeper/scanner/scan_type/scan_type.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.4.9/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/scanner/scanner.py` & `credsweeper-1.4.9/credsweeper/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/secret/config.json` & `credsweeper-1.4.9/credsweeper/secret/config.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999332264957265%*

 * *Differences: {"'exclude'": "{'containers': {insert: [(4, '.pdf')]}, 'extension': {delete: [27]}}"}*

```diff
@@ -10,14 +10,15 @@
     "check_for_literals": true,
     "exclude": {
         "containers": [
             ".apk",
             ".bz2",
             ".docx",
             ".gz",
+            ".pdf",
             ".tar",
             ".xlsx",
             ".zip"
         ],
         "extension": [
             ".7z",
             ".aac",
@@ -42,15 +43,14 @@
             ".mo",
             ".mp3",
             ".mp4",
             ".npy",
             ".npz",
             ".ogg",
             ".pak",
-            ".pdf",
             ".png",
             ".pptx",
             ".pyc",
             ".pyd",
             ".pyo",
             ".rar",
             ".realm",
```

### Comparing `credsweeper-1.4.8/credsweeper/secret/log.yaml` & `credsweeper-1.4.9/credsweeper/secret/log.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 
 version: 1
 
 disable_existing_loggers: False
 
-ignore: [git]
+ignore: [git, pdfminer]
 
 formatters:
     simple:
         format: "%(asctime)s | %(levelname)s | %(module)s:%(lineno)d | %(message)s"
     verbose:
         format: "%(asctime)s | %(levelname)s | %(module)s | %(processName)s:%(threadName)s | %(filename)s:%(lineno)s | %(message)s"
```

### Comparing `credsweeper-1.4.8/credsweeper/utils/util.py` & `credsweeper-1.4.9/credsweeper/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import ast
 import json
 import logging
 import math
 import os
 import tarfile
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Dict, List, Tuple, Optional, Any, Union
 
 import whatthepatch
 import yaml
 from lxml import etree
 from regex import regex
 from typing_extensions import TypedDict
@@ -93,15 +94,15 @@
             p_x = float(data.count(x)) / len(data)
             if p_x > 0:
                 entropy += -p_x * math.log(p_x, 2)
 
         return entropy
 
     @staticmethod
-    def read_file(path: str, encodings: Tuple[str, ...] = default_encodings) -> List[str]:
+    def read_file(path: Union[str, Path], encodings: Tuple[str, ...] = default_encodings) -> List[str]:
         """Read the file content using different encodings.
 
         Try to read the contents of the file according to the list of encodings "encodings" as soon as reading
         occurs without any exceptions, the data is returned in the current encoding
 
         Args:
             path: path to file
@@ -310,14 +311,22 @@
         """According https://www.rfc-editor.org/rfc/rfc1952"""
         if isinstance(data, bytes) and 3 <= len(data):
             if 0x1F == data[0] and 0x8B == data[1] and 0x08 == data[2]:
                 return True
         return False
 
     @staticmethod
+    def is_pdf(data: bytes) -> bool:
+        """According https://en.wikipedia.org/wiki/List_of_file_signatures - pdf"""
+        if isinstance(data, bytes) and 5 <= len(data):
+            if data[0] == 0x25 and data[1] == 0x50 and data[2] == 0x44 and data[3] == 0x46 and data[4] == 0x2D:
+                return True
+        return False
+
+    @staticmethod
     def read_data(path: str) -> Optional[bytes]:
         """Read the file bytes as is.
 
         Try to read the data of the file.
 
         Args:
             path: path to file
@@ -341,47 +350,29 @@
 
         Args:
             xml_lines: list of lines of xml data
 
         Return:
             List of formatted string(f"{root.tag} : {root.text}")
 
+        Raises:
+            xml exception
+
         """
         lines = []
         line_nums = []
         tree = etree.fromstringlist(xml_lines)
         for element in tree.iter():
             tag = Util._extract_element_data(element, "tag")
             text = Util._extract_element_data(element, "text")
             lines.append(f"{tag} : {text}")
             line_nums.append(element.sourceline)
         return lines, line_nums
 
     @staticmethod
-    def get_xml_data(file_path: str) -> Tuple[Optional[List[str]], Optional[List[int]]]:
-        """Read xml data and return List of str.
-
-        Try to read the xml data and return formatted string.
-
-        Args:
-            file_path: path of xml file
-
-        Return:
-            List of formatted string(f"{root.tag} : {root.text}")
-
-        """
-        try:
-            with open(file_path, "r") as f:
-                xml_lines = f.readlines()
-            return Util.get_xml_from_lines(xml_lines)
-        except Exception as exc:
-            logger.error(f"Cannot parse '{file_path}' to xml {exc}")
-            return None, None
-
-    @staticmethod
     def _extract_element_data(element, attr) -> str:
         """Extract xml element data to string.
 
         Try to extract the xml data and strip() the string.
 
         Args:
             element: xml element
@@ -497,15 +488,15 @@
                     result.extend(Util.ast_to_dict(i))
             if hasattr(node, "values"):
                 for i in getattr(node, "values"):
                     result.extend(Util.ast_to_dict(i))
             else:
                 logger.debug(f"skip:{str(node)}")
         else:
-            logger.error(f"unknown:{str(node)}")
+            logger.debug(f"unknown:{str(node)}")
         return result
 
     @staticmethod
     def parse_python(source: str) -> List[Any]:
         """Parse python source to list of strings and assignments"""
         src = ast.parse(source)
         result = Util.ast_to_dict(src)
```

### Comparing `credsweeper-1.4.8/credsweeper/validations/__init__.py` & `credsweeper-1.4.9/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/apply_validation.py` & `credsweeper-1.4.9/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/github_token_validation.py` & `credsweeper-1.4.9/credsweeper/validations/github_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.4.9/credsweeper/validations/google_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.4.9/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.4.9/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.4.9/credsweeper/validations/slack_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.4.9/credsweeper/validations/square_access_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.4.9/credsweeper/validations/square_client_id_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.4.9/credsweeper/validations/stripe_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper/validations/validation.py` & `credsweeper-1.4.9/credsweeper/validations/validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.8/credsweeper.egg-info/PKG-INFO` & `credsweeper-1.4.9/credsweeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.4.8
+Version: 1.4.9
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.4.8/credsweeper.egg-info/SOURCES.txt` & `credsweeper-1.4.9/credsweeper.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -15,33 +15,48 @@
 credsweeper/common/__init__.py
 credsweeper/common/constants.py
 credsweeper/common/keyword_checklist.py
 credsweeper/common/keyword_checklist.txt
 credsweeper/config/__init__.py
 credsweeper/config/config.py
 credsweeper/credentials/__init__.py
+credsweeper/credentials/augment_candidates.py
 credsweeper/credentials/candidate.py
 credsweeper/credentials/candidate_group_generator.py
 credsweeper/credentials/candidate_key.py
 credsweeper/credentials/credential_manager.py
 credsweeper/credentials/line_data.py
+credsweeper/deep_scanner/__init__.py
+credsweeper/deep_scanner/abstract_scanner.py
+credsweeper/deep_scanner/byte_scanner.py
+credsweeper/deep_scanner/bzip2_scanner.py
+credsweeper/deep_scanner/deep_scaner.py
+credsweeper/deep_scanner/encoder_scanner.py
+credsweeper/deep_scanner/gzip_scanner.py
+credsweeper/deep_scanner/html_scanner.py
+credsweeper/deep_scanner/lang_scanner.py
+credsweeper/deep_scanner/pdf_scanner.py
+credsweeper/deep_scanner/tar_scanner.py
+credsweeper/deep_scanner/xml_scanner.py
+credsweeper/deep_scanner/zip_scanner.py
 credsweeper/file_handler/__init__.py
 credsweeper/file_handler/analysis_target.py
 credsweeper/file_handler/byte_content_provider.py
 credsweeper/file_handler/content_provider.py
 credsweeper/file_handler/data_content_provider.py
 credsweeper/file_handler/diff_content_provider.py
 credsweeper/file_handler/file_path_extractor.py
 credsweeper/file_handler/files_provider.py
 credsweeper/file_handler/patch_provider.py
 credsweeper/file_handler/string_content_provider.py
 credsweeper/file_handler/struct_content_provider.py
 credsweeper/file_handler/text_content_provider.py
 credsweeper/file_handler/text_provider.py
 credsweeper/filters/__init__.py
+credsweeper/filters/cred_card_number_check.py
 credsweeper/filters/filter.py
 credsweeper/filters/line_specific_key_check.py
 credsweeper/filters/separator_unusual_check.py
 credsweeper/filters/value_allowlist_check.py
 credsweeper/filters/value_array_dictionary_check.py
 credsweeper/filters/value_blocklist_check.py
 credsweeper/filters/value_camel_case_check.py
@@ -57,14 +72,15 @@
 credsweeper/filters/value_pattern_check.py
 credsweeper/filters/value_similarity_check.py
 credsweeper/filters/value_string_type_check.py
 credsweeper/filters/value_token_check.py
 credsweeper/filters/value_useless_word_check.py
 credsweeper/filters/variable_not_allowed_pattern_check.py
 credsweeper/filters/group/__init__.py
+credsweeper/filters/group/credit_card_number_sequense.py
 credsweeper/filters/group/general_keyword.py
 credsweeper/filters/group/general_pattern.py
 credsweeper/filters/group/group.py
 credsweeper/filters/group/password_keyword.py
 credsweeper/filters/group/pem_pattern.py
 credsweeper/filters/group/url_credentials_group.py
 credsweeper/logger/__init__.py
@@ -94,8 +110,10 @@
 credsweeper/validations/google_api_key_validation.py
 credsweeper/validations/google_multi_validation.py
 credsweeper/validations/mailchimp_key_validation.py
 credsweeper/validations/slack_token_validation.py
 credsweeper/validations/square_access_token_validation.py
 credsweeper/validations/square_client_id_validation.py
 credsweeper/validations/stripe_api_key_validation.py
-credsweeper/validations/validation.py
+credsweeper/validations/validation.py
+tests/test_app.py
+tests/test_main.py
```

### Comparing `credsweeper-1.4.8/setup.py` & `credsweeper-1.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+import sys
+
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 install_requires = [
+    "beautifulsoup4",  #
     "GitPython",  #
     "google_auth_oauthlib",  #
     "humanfriendly",  #
     "lxml",  #
     "oauthlib",  #
     "openpyxl",  #
     "pandas",  #
+    "pdfminer.six",  #
     "PyYAML",  #
     "regex",  #
     "requests",  #
     "scipy",  #
     "typing_extensions",  #
     "whatthepatch",  #
     "numpy",  #
     "scikit-learn",  #
-    "onnxruntime"  #
+    "onnxruntime",  #
 ]
 
 setuptools.setup(
     name="credsweeper",
     description="Credential Sweeper",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

