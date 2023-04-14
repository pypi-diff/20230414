# Comparing `tmp/dfcx-scrapi-1.6.2.tar.gz` & `tmp/dfcx-scrapi-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/pmarlow/eng/scrapi-github/dfcx-scrapi/dist/tmp4gbrjhmq/dfcx-scrapi-1.6.2.tar", last modified: Mon Apr  3 20:13:31 2023, max compression
+gzip compressed data, was "/Users/pmarlow/eng/scrapi-github/dfcx-scrapi/dist/tmp9nwhs6bd/dfcx-scrapi-1.6.3.tar", last modified: Fri Apr 14 18:18:03 2023, max compression
```

## Comparing `dfcx-scrapi-1.6.2.tar` & `dfcx-scrapi-1.6.3.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10136 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/PKG-INFO
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13860 2022-09-29 22:10:42.000000 dfcx-scrapi-1.6.2/.pylintrc
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      248 2022-09-29 15:38:40.000000 dfcx-scrapi-1.6.2/requirements.txt
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/images/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    56107 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/images/logo.png
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      735 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/Makefile
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      776 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/pyproject.toml
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/tests/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1504 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/tests/conftest.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/tests/license/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1030 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/tests/license/license_check.sh
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/tests/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1405 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/tests/test_search_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4767 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/tests/test_agents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      766 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/config.yaml
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9290 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/README.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1803 2023-04-03 20:12:32.000000 dfcx-scrapi-1.6.2/setup.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      765 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/.gitignore
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1103 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/CONTRIBUTING.md
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/examples/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11982 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/scrapi_prebuilt.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/examples/misc/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5080 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/misc/agent_backups.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/examples/nlu_analysis_series/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10106 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/nlu_analysis_series/intent_levenshtein_demo.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10420 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/nlu_analysis_series/nlu_semantic_similarity_demo.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/examples/google_sheets_series/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5426 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/google_sheets_series/sheets_to_cx.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5246 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/google_sheets_series/cx_to_sheets.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6414 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/google_sheets_series/cx_to_sheets_by_flow.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6769 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/google_sheets_series/custom_entities_to_sheets.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/examples/bot_building_series/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3634 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/bot_building_series/bot_building_101.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7555 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10505 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/bot_building_series/bot_building_101.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6519 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15143 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/bot_building_series/builders_101.ipynb
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9284 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/template.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/examples/copy_paste_series/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12067 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/examples/copy_paste_series/copy_paste_pages.ipynb
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/.github/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/.github/workflows/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      519 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/.github/workflows/linter.yml
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      831 2022-02-04 04:14:34.000000 dfcx-scrapi-1.6.2/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1115 2022-02-04 04:14:34.000000 dfcx-scrapi-1.6.2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1810 2022-02-04 04:14:34.000000 dfcx-scrapi-1.6.2/.github/ISSUE_TEMPLATE/pull-request.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       78 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/setup.cfg
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11357 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/LICENSE.txt
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/data/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      535 2022-09-06 20:35:13.000000 dfcx-scrapi-1.6.2/data/intent_sample_with_parts.csv
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/data/ccai_service_kit/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/data/ccai_service_kit/conf_score_cfx/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       11 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/data/ccai_service_kit/conf_score_cfx/requirements.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2215 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/data/ccai_service_kit/conf_score_cfx/main.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    92746 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/data/ccai_service_kit/example_agent_ccai_sk.blob
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4079 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/data/sample_test_cases.blob
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      359 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/data/sample_intent_tp.csv
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      120 2022-09-06 20:35:13.000000 dfcx-scrapi-1.6.2/data/intent_sample_params.csv
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    29501 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/data/sample_agent.blob
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7606 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/maker_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    39988 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/dataframe_functions.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8789 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/semantic_clustering.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      559 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    36759 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/search_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7304 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/levenshtein.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14610 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/utterance_generator_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5178 2023-03-27 20:57:04.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/webhook_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11855 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/nlu_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    50537 2023-04-03 20:10:57.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/copy_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6967 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/validation_util.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4869 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/stats_util.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10396 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/sessions.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12405 2023-03-27 20:57:04.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/transition_route_groups.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    24678 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/intents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11696 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/scrapi_base.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    22050 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/conversation.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7082 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/security_settings.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14779 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    16662 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/agents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2168 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/operations.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3048 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/experiments.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7425 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/pages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14793 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/environments.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7632 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/changelogs.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14556 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/flows.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8770 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/versions.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7173 2023-03-27 14:44:33.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/webhooks.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15320 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/session_entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14575 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/test_cases.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4048 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/project.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11394 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/builders_common.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6402 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/transition_route_groups.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    23961 2023-03-27 20:57:04.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/intents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10092 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/fulfillments.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12143 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-04-04 18:49:12.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8045 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/agents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    26689 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/pages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    20285 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/flows.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9812 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/response_messages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13551 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/routes.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core_ml/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core_ml/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4649 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core_ml/utterance_generator.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/__init__.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core_async/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-04-04 18:49:12.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core_async/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14237 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi/core_async/test_cases.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/agent_assist/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    18850 2023-04-03 20:04:03.000000 dfcx-scrapi-1.6.2/src/agent_assist/agent_assist.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-12-10 02:15:04.000000 dfcx-scrapi-1.6.2/src/agent_assist/__init__.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi.egg-info/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10136 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi.egg-info/PKG-INFO
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3537 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi.egg-info/SOURCES.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       27 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi.egg-info/requires.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       25 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi.egg-info/top_level.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        1 2023-04-03 20:13:31.000000 dfcx-scrapi-1.6.2/src/dfcx_scrapi.egg-info/dependency_links.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10136 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/PKG-INFO
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13860 2022-09-29 22:10:42.000000 dfcx-scrapi-1.6.3/.pylintrc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      248 2022-09-29 15:38:40.000000 dfcx-scrapi-1.6.3/requirements.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/images/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    56107 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/images/logo.png
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      735 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/Makefile
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      776 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/pyproject.toml
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/tests/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1504 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/tests/conftest.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/tests/license/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1030 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/tests/license/license_check.sh
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/tests/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1405 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/tests/test_search_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4767 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/tests/test_agents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      766 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/config.yaml
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9290 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/README.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1803 2023-04-14 18:17:28.000000 dfcx-scrapi-1.6.3/setup.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      765 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/.gitignore
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1103 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/CONTRIBUTING.md
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11982 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/scrapi_prebuilt.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/misc/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5080 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/misc/agent_backups.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/nlu_analysis_series/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10106 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/nlu_analysis_series/intent_levenshtein_demo.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10420 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/nlu_analysis_series/nlu_semantic_similarity_demo.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5426 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/sheets_to_cx.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5246 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/cx_to_sheets.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6414 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/cx_to_sheets_by_flow.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6769 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/google_sheets_series/custom_entities_to_sheets.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3634 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_101.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7555 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10505 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_101.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6519 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15143 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/bot_building_series/builders_101.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9284 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/template.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/examples/copy_paste_series/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12067 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/examples/copy_paste_series/copy_paste_pages.ipynb
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/.github/
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/.github/workflows/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      519 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/.github/workflows/linter.yml
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      831 2022-02-04 04:14:34.000000 dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1115 2022-02-04 04:14:34.000000 dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1810 2022-02-04 04:14:34.000000 dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/pull-request.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       78 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/setup.cfg
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11357 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/LICENSE.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/data/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      535 2022-09-06 20:35:13.000000 dfcx-scrapi-1.6.3/data/intent_sample_with_parts.csv
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/conf_score_cfx/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       11 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/conf_score_cfx/requirements.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2215 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/conf_score_cfx/main.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    92746 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/ccai_service_kit/example_agent_ccai_sk.blob
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4079 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/sample_test_cases.blob
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      359 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/sample_intent_tp.csv
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      120 2022-09-06 20:35:13.000000 dfcx-scrapi-1.6.3/data/intent_sample_params.csv
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    29501 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/data/sample_agent.blob
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7606 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/maker_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    39988 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/dataframe_functions.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8789 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/semantic_clustering.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      559 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    36759 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/search_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7304 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/levenshtein.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14610 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/utterance_generator_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5178 2023-03-27 20:57:04.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/webhook_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11855 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/nlu_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    50537 2023-04-03 20:10:57.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/copy_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6967 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/validation_util.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4869 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/stats_util.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10396 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/sessions.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12405 2023-03-27 20:57:04.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/transition_route_groups.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    24678 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/intents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11979 2023-04-14 18:06:49.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/scrapi_base.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    23425 2023-04-14 18:06:49.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/conversation.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7082 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/security_settings.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14779 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    16662 2023-04-14 17:27:13.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/agents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2168 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/operations.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3048 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/experiments.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7425 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/pages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14793 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/environments.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7632 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/changelogs.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14556 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/flows.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8770 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/versions.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7173 2023-03-27 14:44:33.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/webhooks.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    15320 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/session_entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14575 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/test_cases.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4048 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/project.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11394 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/builders_common.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6402 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/transition_route_groups.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    23961 2023-03-27 20:57:04.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/intents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10092 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/fulfillments.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12143 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-04-04 18:49:12.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8045 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/agents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    26689 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/pages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    20285 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/flows.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9812 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/response_messages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13551 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/routes.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_ml/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_ml/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4649 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_ml/utterance_generator.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2021-12-30 17:29:06.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/__init__.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_async/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-04-04 18:49:12.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_async/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    14237 2023-03-27 13:37:45.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_async/test_cases.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/agent_assist/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    18850 2023-04-03 20:04:03.000000 dfcx-scrapi-1.6.3/src/agent_assist/agent_assist.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2022-12-10 02:15:04.000000 dfcx-scrapi-1.6.3/src/agent_assist/__init__.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10136 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/PKG-INFO
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3537 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       27 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/requires.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       25 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/top_level.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        1 2023-04-14 18:18:03.000000 dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/dependency_links.txt
```

### Comparing `dfcx-scrapi-1.6.2/PKG-INFO` & `dfcx-scrapi-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcx-scrapi
-Version: 1.6.2
+Version: 1.6.3
 Summary: A high level scripting API for bot builders, developers, and      maintainers.
 Home-page: https://github.com/GoogleCloudPlatform/dfcx-scrapi
 Author: Patrick Marlow
 Author-email: pmarlow@google.com
 License: UNKNOWN
 Keywords: dialogflow,cx,google,bot,chatbot,intent,dfcx,entity
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dfcx-scrapi Version: 1.6.2 Summary: A high level
+Metadata-Version: 2.1 Name: dfcx-scrapi Version: 1.6.3 Summary: A high level
 scripting API for bot builders, developers, and maintainers. Home-page: https:/
 /github.com/GoogleCloudPlatform/dfcx-scrapi Author: Patrick Marlow Author-
 email: pmarlow@google.com License: UNKNOWN Keywords:
 dialogflow,cx,google,bot,chatbot,intent,dfcx,entity Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Communications :: Chat Classifier: Topic ::
```

### Comparing `dfcx-scrapi-1.6.2/.pylintrc` & `dfcx-scrapi-1.6.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/images/logo.png` & `dfcx-scrapi-1.6.3/images/logo.png`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/Makefile` & `dfcx-scrapi-1.6.3/Makefile`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/pyproject.toml` & `dfcx-scrapi-1.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/tests/conftest.py` & `dfcx-scrapi-1.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/tests/license/license_check.sh` & `dfcx-scrapi-1.6.3/tests/license/license_check.sh`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/tests/test_search_util.py` & `dfcx-scrapi-1.6.3/tests/test_search_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/tests/test_agents.py` & `dfcx-scrapi-1.6.3/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/config.yaml` & `dfcx-scrapi-1.6.3/config.yaml`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/README.md` & `dfcx-scrapi-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/setup.py` & `dfcx-scrapi-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dfcx-scrapi',
-    version='1.6.2',
+    version='1.6.3',
     description='A high level scripting API for bot builders, developers, and\
       maintainers.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/dfcx-scrapi',
     author='Patrick Marlow',
     author_email='pmarlow@google.com',
```

### Comparing `dfcx-scrapi-1.6.2/.gitignore` & `dfcx-scrapi-1.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/CONTRIBUTING.md` & `dfcx-scrapi-1.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/scrapi_prebuilt.ipynb` & `dfcx-scrapi-1.6.3/examples/scrapi_prebuilt.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/misc/agent_backups.ipynb` & `dfcx-scrapi-1.6.3/examples/misc/agent_backups.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/nlu_analysis_series/intent_levenshtein_demo.ipynb` & `dfcx-scrapi-1.6.3/examples/nlu_analysis_series/intent_levenshtein_demo.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/nlu_analysis_series/nlu_semantic_similarity_demo.ipynb` & `dfcx-scrapi-1.6.3/examples/nlu_analysis_series/nlu_semantic_similarity_demo.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/google_sheets_series/sheets_to_cx.ipynb` & `dfcx-scrapi-1.6.3/examples/google_sheets_series/sheets_to_cx.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/google_sheets_series/cx_to_sheets.ipynb` & `dfcx-scrapi-1.6.3/examples/google_sheets_series/cx_to_sheets.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/google_sheets_series/cx_to_sheets_by_flow.ipynb` & `dfcx-scrapi-1.6.3/examples/google_sheets_series/cx_to_sheets_by_flow.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/google_sheets_series/custom_entities_to_sheets.ipynb` & `dfcx-scrapi-1.6.3/examples/google_sheets_series/custom_entities_to_sheets.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/bot_building_series/bot_building_101.py` & `dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_101.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.ipynb` & `dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/bot_building_series/bot_building_101.ipynb` & `dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_101.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.py` & `dfcx-scrapi-1.6.3/examples/bot_building_series/bot_building_102_intents_with_annotated_tp.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/bot_building_series/builders_101.ipynb` & `dfcx-scrapi-1.6.3/examples/bot_building_series/builders_101.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/template.ipynb` & `dfcx-scrapi-1.6.3/examples/template.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/examples/copy_paste_series/copy_paste_pages.ipynb` & `dfcx-scrapi-1.6.3/examples/copy_paste_series/copy_paste_pages.ipynb`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/.github/workflows/linter.yml` & `dfcx-scrapi-1.6.3/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/.github/ISSUE_TEMPLATE/feature-request.md` & `dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/.github/ISSUE_TEMPLATE/bug-report.md` & `dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/.github/ISSUE_TEMPLATE/pull-request.md` & `dfcx-scrapi-1.6.3/.github/ISSUE_TEMPLATE/pull-request.md`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/LICENSE.txt` & `dfcx-scrapi-1.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/data/intent_sample_with_parts.csv` & `dfcx-scrapi-1.6.3/data/intent_sample_with_parts.csv`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/data/ccai_service_kit/conf_score_cfx/main.py` & `dfcx-scrapi-1.6.3/data/ccai_service_kit/conf_score_cfx/main.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/data/ccai_service_kit/example_agent_ccai_sk.blob` & `dfcx-scrapi-1.6.3/data/ccai_service_kit/example_agent_ccai_sk.blob`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/data/sample_test_cases.blob` & `dfcx-scrapi-1.6.3/data/sample_test_cases.blob`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/data/sample_agent.blob` & `dfcx-scrapi-1.6.3/data/sample_agent.blob`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/maker_util.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/maker_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/dataframe_functions.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/semantic_clustering.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/semantic_clustering.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/__init__.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/search_util.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/search_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/levenshtein.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/levenshtein.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/utterance_generator_util.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/utterance_generator_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/webhook_util.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/webhook_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/nlu_util.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/nlu_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/copy_util.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/copy_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/validation_util.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/validation_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/tools/stats_util.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/tools/stats_util.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/sessions.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/sessions.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/transition_route_groups.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/transition_route_groups.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/intents.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/intents.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/scrapi_base.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/scrapi_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,39 +68,48 @@
             self.creds = None
             self.token = None
 
         if agent_id:
             self.agent_id = agent_id
 
     @staticmethod
-    def _set_region(item_id):
+    def _set_region(resource_id: str):
         """Different regions have different API endpoints
 
         Args:
           item_id: agent/flow/page - any type of long path id like
             `projects/<GCP PROJECT ID>/locations/<LOCATION ID>
 
         Returns:
           A dictionary containing the api_endpoint to use when
           instantiating other library client objects, or None
           if the location is "global"
         """
         try:
-            location = item_id.split("/")[3]
+            location = resource_id.split("/")[3]
         except IndexError as err:
-            logging.error("IndexError - path too short? %s", item_id)
+            logging.error("IndexError - path too short? %s", resource_id)
             raise err
 
+        project_id = resource_id.split("/")[1]
+
         if location != "global":
             api_endpoint = f"{location}-dialogflow.googleapis.com:443"
-            client_options = {"api_endpoint": api_endpoint}
+            client_options = {
+                "api_endpoint": api_endpoint,
+                "quota_project_id": project_id}
             return client_options
 
         else:
-            return None  # explicit None return when not required
+            api_endpoint = "dialogflow.googleapis.com:443"
+            client_options = {
+                "api_endpoint": api_endpoint,
+                "quota_project_id": project_id}
+
+            return client_options
 
     @staticmethod
     def pbuf_to_dict(pbuf):
         """Extractor of json from a protobuf"""
         blobstr = json_format.MessageToJson(
             pbuf
         )  # i think this returns JSON as a string
```

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/conversation.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/conversation.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 import logging
 import time
 import traceback
 import uuid
 
-from typing import Dict
+from typing import Dict, Any
 from operator import attrgetter
 from threading import Thread
 
 import pandas as pd
 
 from google.cloud.dialogflowcx_v3beta1 import services
 from google.cloud.dialogflowcx_v3beta1 import types
@@ -60,33 +60,70 @@
         super().__init__(
             creds_path=creds_path,
             creds_dict=creds_dict,
             creds=creds,
             agent_id=agent_id,
         )
 
-        logging.info(
+        logging.debug(
             "create conversation with creds_path: %s | agent_id: %s",
             creds_path, agent_id)
 
-        if agent_id or config["agent_path"]:
-            self.agent_id = agent_id or config["agent_path"]
-
-        self.language_code = language_code or config["language_code"]
-
+        self.agent_id = self._set_agent_id(agent_id, config)
+        self.language_code = self._set_language_code(language_code, config)
         self.start_time = None
         self.query_result = None
         self.session_id = None
         self.turn_count = None
         self.agent_env = {}  # empty
         self.restart()
         self.flows = flows.Flows(creds=self.creds)
         self.pages = pages.Pages(creds=self.creds)
 
     @staticmethod
+    def _set_language_code(language_code: str, config: Dict[str, Any]) -> str:
+        """Determines how to set the language_code based on user inputs.
+
+        We implement this for backwards compatability.
+        """
+        # Config will take precedence if provided
+        if config:
+            config_lang_code = config.get("language_code", None)
+
+            # We'll only return if it exist in the config on the off chance that
+            # some users have provided the langauge_code as a top level arg in
+            # addition to providing the config
+            if config_lang_code:
+                return config_lang_code
+
+        return language_code
+
+    @staticmethod
+    def _set_agent_id(input_agent_id: str, config: Dict[str, Any]) -> str:
+        """Determines how to set the agent_id based on user inputs.
+
+        We implement this for backwards compatability.
+        """
+
+        # Config will take precedence if provided
+        if config:
+            config_agent_path = config.get("agent_path", None)
+
+            # We'll only return if it exist in the config on the off chance that
+            # some users have provided the agent_id as a top level arg in
+            # addition to providing the config
+            if config_agent_path:
+                return config_agent_path
+
+        elif input_agent_id:
+            return input_agent_id
+
+        return None
+
+    @staticmethod
     def _get_match_type_from_map(match_type: int):
         """Translates the match_type enum int value into a more descriptive
         string.
         """
         match_type_map = {
             0: "MATCH_TYPE_UNSPECIFIED",
             1: "INTENT",
```

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/security_settings.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/security_settings.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/entity_types.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/entity_types.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/agents.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/agents.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/operations.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/operations.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/experiments.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/experiments.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/pages.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/pages.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/environments.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/environments.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/changelogs.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/changelogs.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/flows.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/flows.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/versions.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/versions.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/webhooks.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/webhooks.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/session_entity_types.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/session_entity_types.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/test_cases.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/test_cases.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core/project.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core/project.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/builders_common.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/builders_common.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/transition_route_groups.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/transition_route_groups.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/intents.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/intents.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/fulfillments.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/fulfillments.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/entity_types.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/entity_types.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/agents.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/agents.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/pages.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/pages.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/flows.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/flows.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/response_messages.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/response_messages.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/builders/routes.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/builders/routes.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core_ml/utterance_generator.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_ml/utterance_generator.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi/core_async/test_cases.py` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi/core_async/test_cases.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/agent_assist/agent_assist.py` & `dfcx-scrapi-1.6.3/src/agent_assist/agent_assist.py`

 * *Files identical despite different names*

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi.egg-info/PKG-INFO` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcx-scrapi
-Version: 1.6.2
+Version: 1.6.3
 Summary: A high level scripting API for bot builders, developers, and      maintainers.
 Home-page: https://github.com/GoogleCloudPlatform/dfcx-scrapi
 Author: Patrick Marlow
 Author-email: pmarlow@google.com
 License: UNKNOWN
 Keywords: dialogflow,cx,google,bot,chatbot,intent,dfcx,entity
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dfcx-scrapi Version: 1.6.2 Summary: A high level
+Metadata-Version: 2.1 Name: dfcx-scrapi Version: 1.6.3 Summary: A high level
 scripting API for bot builders, developers, and maintainers. Home-page: https:/
 /github.com/GoogleCloudPlatform/dfcx-scrapi Author: Patrick Marlow Author-
 email: pmarlow@google.com License: UNKNOWN Keywords:
 dialogflow,cx,google,bot,chatbot,intent,dfcx,entity Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Communications :: Chat Classifier: Topic ::
```

### Comparing `dfcx-scrapi-1.6.2/src/dfcx_scrapi.egg-info/SOURCES.txt` & `dfcx-scrapi-1.6.3/src/dfcx_scrapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

