# Comparing `tmp/usdm-0.24.0.tar.gz` & `tmp/usdm-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.24.0.tar", last modified: Wed Apr 12 18:24:16 2023, max compression
+gzip compressed data, was "usdm-0.25.0.tar", last modified: Fri Apr 14 13:51:32 2023, max compression
```

## Comparing `usdm-0.24.0.tar` & `usdm-0.25.0.tar`

### file list

```diff
@@ -1,126 +1,134 @@
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.807154 usdm-0.24.0/
--rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-01-12 15:50:29.000000 usdm-0.24.0/LICENSE
--rw-r--r--   0 daveih     (501) staff       (20)    18175 2023-04-12 18:24:16.806944 usdm-0.24.0/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)    17725 2023-04-12 18:20:23.000000 usdm-0.24.0/README.md
--rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 15:14:44.000000 usdm-0.24.0/pyproject.toml
--rw-r--r--   0 daveih     (501) staff       (20)       38 2023-04-12 18:24:16.807205 usdm-0.24.0/setup.cfg
--rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:32:56.000000 usdm-0.24.0/setup.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.736124 usdm-0.24.0/src/
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.743951 usdm-0.24.0/src/usdm.egg-info/
--rw-r--r--   0 daveih     (501) staff       (20)    18175 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)     3928 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/SOURCES.txt
--rw-r--r--   0 daveih     (501) staff       (20)        1 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/dependency_links.txt
--rw-r--r--   0 daveih     (501) staff       (20)       45 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/requires.txt
--rw-r--r--   0 daveih     (501) staff       (20)       32 2023-04-12 18:24:16.000000 usdm-0.24.0/src/usdm.egg-info/top_level.txt
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.774532 usdm-0.24.0/src/usdm_excel/
--rw-r--r--   0 daveih     (501) staff       (20)     1122 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      269 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/alias.py
--rw-r--r--   0 daveih     (501) staff       (20)     8005 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3766 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      787 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/cdisc_ct_library.py
--rw-r--r--   0 daveih     (501) staff       (20)     1366 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/cross_ref.py
--rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/ct_version_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.777106 usdm-0.24.0/src/usdm_excel/data/
--rw-r--r--   0 daveih     (501) staff       (20)      927 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/data/cdisc_ct_config.yaml
--rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/data/iso_3166.json
--rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/data/missing_ct.yaml
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.782871 usdm-0.24.0/src/usdm_excel/errors/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-05 16:50:22.000000 usdm-0.24.0/src/usdm_excel/errors/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      627 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/errors/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      650 2023-04-11 18:31:21.000000 usdm-0.24.0/src/usdm_excel/errors/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-04-04 17:49:00.000000 usdm-0.24.0/src/usdm_excel/id_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)      737 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      111 2023-03-31 15:48:06.000000 usdm-0.24.0/src/usdm_excel/logger.py
--rw-r--r--   0 daveih     (501) staff       (20)      309 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     3730 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/nodes_and_edges.py
--rw-r--r--   0 daveih     (501) staff       (20)      512 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/option_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.784535 usdm-0.24.0/src/usdm_excel/study_design_element_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_element_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1834 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.785643 usdm-0.24.0/src/usdm_excel/study_design_encounter_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2429 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.786520 usdm-0.24.0/src/usdm_excel/study_design_estimands_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2259 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.787749 usdm-0.24.0/src/usdm_excel/study_design_ii_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_ii_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1655 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.788649 usdm-0.24.0/src/usdm_excel/study_design_objective_endpoint_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2023 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.789363 usdm-0.24.0/src/usdm_excel/study_design_population_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_population_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1631 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.789855 usdm-0.24.0/src/usdm_excel/study_design_procedure_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1590 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.790292 usdm-0.24.0/src/usdm_excel/study_design_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_design_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     5859 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.790763 usdm-0.24.0/src/usdm_excel/study_identifiers_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_identifiers_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2559 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.791209 usdm-0.24.0/src/usdm_excel/study_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     7158 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_excel/study_sheet/study_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.794033 usdm-0.24.0/src/usdm_excel/study_soa_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/activities.py
--rw-r--r--   0 daveih     (501) staff       (20)     2899 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/cycle.py
--rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/cycles.py
--rw-r--r--   0 daveih     (501) staff       (20)      993 2023-04-05 16:39:25.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/encounters.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
--rw-r--r--   0 daveih     (501) staff       (20)     4547 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5048 2023-04-12 17:57:02.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/timepoint.py
--rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-12 17:57:02.000000 usdm-0.24.0/src/usdm_excel/study_soa_sheet/timepoints.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.794242 usdm-0.24.0/src/usdm_info/
--rw-r--r--   0 daveih     (501) staff       (20)       59 2023-04-12 17:04:52.000000 usdm-0.24.0/src/usdm_info/__init__.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.804393 usdm-0.24.0/src/usdm_model/
--rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/address.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/aliasCode.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/alias_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/analysis_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/api_base_model.py
--rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/biomedical_concept_category.py
--rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/biomedical_concept_property.py
--rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/biomedical_concept_surrogate.py
--rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/code.py
--rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/encounter.py
--rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/endpoint.py
--rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/estimand.py
--rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/indication.py
--rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/intercurrent_event.py
--rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/investigational_intervention.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/objective.py
--rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/organisation.py
--rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/procedure.py
--rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/response_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/schedule_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/schedule_timeline_exit.py
--rw-r--r--   0 daveih     (501) staff       (20)      691 2023-04-12 17:57:02.000000 usdm-0.24.0/src/usdm_model/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study.py
--rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/study_arm.py
--rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_cell.py
--rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/study_design.py
--rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_design_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_element.py
--rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_epoch.py
--rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_identifier.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/study_protocol_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 16:05:11.000000 usdm-0.24.0/src/usdm_model/timing.py
--rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 15:14:44.000000 usdm-0.24.0/src/usdm_model/transition_rule.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-12 18:24:16.806594 usdm-0.24.0/tests/
--rw-r--r--   0 daveih     (501) staff       (20)    12726 2023-04-11 16:05:11.000000 usdm-0.24.0/tests/test_base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 15:14:12.000000 usdm-0.24.0/tests/test_cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      679 2023-04-11 16:05:11.000000 usdm-0.24.0/tests/test_error.py
--rw-r--r--   0 daveih     (501) staff       (20)     1126 2023-04-11 16:05:11.000000 usdm-0.24.0/tests/test_errors.py
--rw-r--r--   0 daveih     (501) staff       (20)      950 2023-04-04 18:02:59.000000 usdm-0.24.0/tests/test_iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-04 18:04:47.000000 usdm-0.24.0/tests/test_ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)      969 2023-04-12 17:04:52.000000 usdm-0.24.0/tests/test_option_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.374523 usdm-0.25.0/
+-rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.25.0/LICENSE
+-rw-r--r--   0 daveih     (501) staff       (20)    19581 2023-04-14 13:51:32.374247 usdm-0.25.0/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)    19131 2023-04-14 12:14:15.000000 usdm-0.25.0/README.md
+-rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.25.0/pyproject.toml
+-rw-r--r--   0 daveih     (501) staff       (20)       38 2023-04-14 13:51:32.374586 usdm-0.25.0/setup.cfg
+-rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.25.0/setup.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.329578 usdm-0.25.0/src/
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.332738 usdm-0.25.0/src/usdm.egg-info/
+-rw-r--r--   0 daveih     (501) staff       (20)    19581 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)     4238 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/SOURCES.txt
+-rw-r--r--   0 daveih     (501) staff       (20)        1 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/dependency_links.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       45 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/requires.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       32 2023-04-14 13:51:32.000000 usdm-0.25.0/src/usdm.egg-info/top_level.txt
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.340448 usdm-0.25.0/src/usdm_excel/
+-rw-r--r--   0 daveih     (501) staff       (20)     1122 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.25.0/src/usdm_excel/alias.py
+-rw-r--r--   0 daveih     (501) staff       (20)     8005 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3766 2023-04-05 14:21:45.000000 usdm-0.25.0/src/usdm_excel/cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.25.0/src/usdm_excel/cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.25.0/src/usdm_excel/cdisc_ct_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1366 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/cross_ref.py
+-rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/ct_version_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.341652 usdm-0.25.0/src/usdm_excel/data/
+-rw-r--r--   0 daveih     (501) staff       (20)      963 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/data/cdisc_ct_config.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/data/iso_3166.json
+-rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.25.0/src/usdm_excel/data/missing_ct.yaml
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.342552 usdm-0.25.0/src/usdm_excel/errors/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.25.0/src/usdm_excel/errors/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      627 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/errors/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      650 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/errors/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/id_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)      744 2023-04-13 09:34:38.000000 usdm-0.25.0/src/usdm_excel/iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.25.0/src/usdm_excel/logger.py
+-rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.25.0/src/usdm_excel/ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3730 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/nodes_and_edges.py
+-rw-r--r--   0 daveih     (501) staff       (20)      512 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/option_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.343116 usdm-0.25.0/src/usdm_excel/study_design_arm_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_arm_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1443 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.343880 usdm-0.25.0/src/usdm_excel/study_design_element_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_element_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1834 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.344639 usdm-0.25.0/src/usdm_excel/study_design_encounter_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2429 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.345310 usdm-0.25.0/src/usdm_excel/study_design_epoch_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1124 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.346023 usdm-0.25.0/src/usdm_excel/study_design_estimands_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2259 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.346711 usdm-0.25.0/src/usdm_excel/study_design_ii_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_ii_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1655 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.347421 usdm-0.25.0/src/usdm_excel/study_design_objective_endpoint_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2025 2023-04-14 13:39:15.000000 usdm-0.25.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.348146 usdm-0.25.0/src/usdm_excel/study_design_population_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_population_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1631 2023-04-11 13:28:10.000000 usdm-0.25.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.348732 usdm-0.25.0/src/usdm_excel/study_design_procedure_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1590 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.349391 usdm-0.25.0/src/usdm_excel/study_design_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_design_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5094 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.350053 usdm-0.25.0/src/usdm_excel/study_identifiers_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_identifiers_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2559 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.350699 usdm-0.25.0/src/usdm_excel/study_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7444 2023-04-14 12:14:15.000000 usdm-0.25.0/src/usdm_excel/study_sheet/study_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.356163 usdm-0.25.0/src/usdm_excel/study_soa_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/activities.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2899 2023-04-05 14:06:46.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/cycle.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/cycles.py
+-rw-r--r--   0 daveih     (501) staff       (20)      993 2023-04-05 14:06:46.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/encounters.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4645 2023-04-13 09:55:50.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5048 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/timepoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_excel/study_soa_sheet/timepoints.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.356556 usdm-0.25.0/src/usdm_info/
+-rw-r--r--   0 daveih     (501) staff       (20)       59 2023-04-13 09:55:50.000000 usdm-0.25.0/src/usdm_info/__init__.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.369329 usdm-0.25.0/src/usdm_model/
+-rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/address.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/aliasCode.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/alias_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/analysis_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/api_base_model.py
+-rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/biomedical_concept_category.py
+-rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/biomedical_concept_property.py
+-rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/biomedical_concept_surrogate.py
+-rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/encounter.py
+-rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/endpoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/estimand.py
+-rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/indication.py
+-rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/intercurrent_event.py
+-rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/investigational_intervention.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/objective.py
+-rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/organisation.py
+-rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/procedure.py
+-rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/response_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/schedule_timeline.py
+-rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/schedule_timeline_exit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      691 2023-04-13 04:26:45.000000 usdm-0.25.0/src/usdm_model/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study.py
+-rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/study_arm.py
+-rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_cell.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/study_design.py
+-rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_design_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_element.py
+-rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_epoch.py
+-rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_identifier.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/study_protocol_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 13:59:38.000000 usdm-0.25.0/src/usdm_model/timing.py
+-rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 13:46:27.000000 usdm-0.25.0/src/usdm_model/transition_rule.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-04-14 13:51:32.373707 usdm-0.25.0/tests/
+-rw-r--r--   0 daveih     (501) staff       (20)    12726 2023-04-11 13:28:11.000000 usdm-0.25.0/tests/test_base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.25.0/tests/test_cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      679 2023-04-11 13:28:11.000000 usdm-0.25.0/tests/test_error.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1126 2023-04-11 13:28:11.000000 usdm-0.25.0/tests/test_errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)      971 2023-04-13 09:35:41.000000 usdm-0.25.0/tests/test_iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.25.0/tests/test_ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      969 2023-04-13 04:26:45.000000 usdm-0.25.0/tests/test_option_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3320 2023-04-14 12:14:15.000000 usdm-0.25.0/tests/test_study_design_arm_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2716 2023-04-14 12:14:15.000000 usdm-0.25.0/tests/test_study_design_epoch_sheet.py
```

### Comparing `usdm-0.24.0/LICENSE` & `usdm-0.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/PKG-INFO` & `usdm-0.25.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: usdm
-Version: 0.24.0
-Summary: A python package for using the CDISC TransCelerate USDM
-Author: D Iberson-Hurst
-Author-email: 
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CDISC / Transcelerate DDF USDM Package
 
 This package provides an implementation of the Digital Data Flow (DDF) CDISC / TransCelerate Unified Study Definitions Model (USDM). Two main parts are provided:
 
 - Within the `usdm_model` directory are a set of classes reflecting the USDM model as transported using the DDF USDM API 
 - Within the `usdm_excel` directory is a class, `USDMExcel`, that can be used to import an entire study definition from an excel file and build the equivalent json as defined by the API
 
@@ -138,15 +124,15 @@
 | Column | Column Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
 | B | organisationIdentifier | Organisation identifier | Text string |
 | C | organisationName | Organisation name | Text string |
 | D | organisationType | Organisation type | CDISC code reference |
 | E | studyIdentifier | The identifier for the study | Text string |
-| F | organisationAddress | The organisation address | Formated using a pipe delimited - allows for commas in items within the address - form, i.e. `line|city|district|state|postal_code|<country code>`. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. |
+| F | organisationAddress | The organisation address | Formated using a pipe delimited form `line|city|district|state|postal_code|<country code>`. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. |
 
 ### Study Design sheet
 
 #### Sheet Name
 
 `studyDesign`
 
@@ -167,17 +153,51 @@
 | 7 | trialTypes | Code for the trial type | CDISC code reference|
 | 8 | interventionModel | | CDISC code reference |
 | 9 | mainTimeline | Name of main timeline sheet | This must be present |
 | 10 | otherTimelines | Names of other timeline sheeText string | Commma separated list of sheet names. Can be empty |
 
 For the arms and epochs, a simple table is required. The table starts in row 12 and can consists of a header row and 1 or more arm rows. 
 
-The header row consists of a cell that is ignored followed by 1 or more cells containing the epoch names.
+The header row consists of a cell in column A that is ignored followed by 1 or more cells (columns) containing the epoch names. Each epoch name should have a corresponding entry in the Study Design Epochs sheet, see below.
+
+The arm rows consist of the arm name in the first column followed by a cells for each epoch containing one or more references to study design elements defined in the studyDesignElements sheet. Each arm name should have a corresponding entry in the Study Design Arms sheet, see bwlow.
+
+### Study Design Arms sheet
+
+#### Sheet Name
+
+`studyDesignArms`
 
-The arm rows consist of the arm name in the first column followed by a cells for each epoch containing one or more references to study design elements defined in the studyDesignElements sheet.
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2, containing the details of a study arm: 
+
+| Column | Column Name | Description | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | studyArmName | The study name | Text string. Should match an arm name in the Study Design sheet | 
+| B | studyArmDescription | A Text string description for the arm | Text string |
+| C | studyArmType | The arm type| CDISC code reference |
+| D | studyArmDataOriginDescription	| The description of the data origin for the arm | Text string |
+| E | studyArmDataOriginType | The type of arm data origin | CDISC code reference|
+
+### Study Design Epochs sheet
+
+#### Sheet Name
+
+`studyDesignEpochs`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2, containing the details of a study epoch: 
+
+| Column | Column Name | Description | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | studyEpochName | The epoch name | Text string. Should match an epoch name in the Study Design sheet | 
+| B | studyEpochDescription | A Text string description for the epoch | Text string |
+| C | studyEpochType | The epoch type| CDISC code reference |
 
 ### Timeline sheets
 
 #### Sheet Name
 
 As defined within the study design sheet, see above.
 
@@ -412,8 +432,8 @@
 
 It is intended to support all of the content in the USDM. The following features are not yet supported:
 
 - Full Arm definitions
 - Full Epoch definitions
 - BC categories
 
-See the [github issues](https://github.com/data4knowledge/usdm/issues)
+See the [github issues](https://github.com/data4knowledge/usdm/issues)
```

### Comparing `usdm-0.24.0/README.md` & `usdm-0.25.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: usdm
+Version: 0.25.0
+Summary: A python package for using the CDISC TransCelerate USDM
+Author: D Iberson-Hurst
+Author-email: 
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CDISC / Transcelerate DDF USDM Package
 
 This package provides an implementation of the Digital Data Flow (DDF) CDISC / TransCelerate Unified Study Definitions Model (USDM). Two main parts are provided:
 
 - Within the `usdm_model` directory are a set of classes reflecting the USDM model as transported using the DDF USDM API 
 - Within the `usdm_excel` directory is a class, `USDMExcel`, that can be used to import an entire study definition from an excel file and build the equivalent json as defined by the API
 
@@ -124,15 +138,15 @@
 | Column | Column Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
 | B | organisationIdentifier | Organisation identifier | Text string |
 | C | organisationName | Organisation name | Text string |
 | D | organisationType | Organisation type | CDISC code reference |
 | E | studyIdentifier | The identifier for the study | Text string |
-| F | organisationAddress | The organisation address | Formated using a pipe delimited - allows for commas in items within the address - form, i.e. `line|city|district|state|postal_code|<country code>`. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. |
+| F | organisationAddress | The organisation address | Formated using a pipe delimited form `line|city|district|state|postal_code|<country code>`. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. |
 
 ### Study Design sheet
 
 #### Sheet Name
 
 `studyDesign`
 
@@ -153,17 +167,51 @@
 | 7 | trialTypes | Code for the trial type | CDISC code reference|
 | 8 | interventionModel | | CDISC code reference |
 | 9 | mainTimeline | Name of main timeline sheet | This must be present |
 | 10 | otherTimelines | Names of other timeline sheeText string | Commma separated list of sheet names. Can be empty |
 
 For the arms and epochs, a simple table is required. The table starts in row 12 and can consists of a header row and 1 or more arm rows. 
 
-The header row consists of a cell that is ignored followed by 1 or more cells containing the epoch names.
+The header row consists of a cell in column A that is ignored followed by 1 or more cells (columns) containing the epoch names. Each epoch name should have a corresponding entry in the Study Design Epochs sheet, see below.
+
+The arm rows consist of the arm name in the first column followed by a cells for each epoch containing one or more references to study design elements defined in the studyDesignElements sheet. Each arm name should have a corresponding entry in the Study Design Arms sheet, see bwlow.
+
+### Study Design Arms sheet
+
+#### Sheet Name
+
+`studyDesignArms`
 
-The arm rows consist of the arm name in the first column followed by a cells for each epoch containing one or more references to study design elements defined in the studyDesignElements sheet.
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2, containing the details of a study arm: 
+
+| Column | Column Name | Description | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | studyArmName | The study name | Text string. Should match an arm name in the Study Design sheet | 
+| B | studyArmDescription | A Text string description for the arm | Text string |
+| C | studyArmType | The arm type| CDISC code reference |
+| D | studyArmDataOriginDescription	| The description of the data origin for the arm | Text string |
+| E | studyArmDataOriginType | The type of arm data origin | CDISC code reference|
+
+### Study Design Epochs sheet
+
+#### Sheet Name
+
+`studyDesignEpochs`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2, containing the details of a study epoch: 
+
+| Column | Column Name | Description | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | studyEpochName | The epoch name | Text string. Should match an epoch name in the Study Design sheet | 
+| B | studyEpochDescription | A Text string description for the epoch | Text string |
+| C | studyEpochType | The epoch type| CDISC code reference |
 
 ### Timeline sheets
 
 #### Sheet Name
 
 As defined within the study design sheet, see above.
 
@@ -398,8 +446,8 @@
 
 It is intended to support all of the content in the USDM. The following features are not yet supported:
 
 - Full Arm definitions
 - Full Epoch definitions
 - BC categories
 
-See the [github issues](https://github.com/data4knowledge/usdm/issues)
+See the [github issues](https://github.com/data4knowledge/usdm/issues)
```

### Comparing `usdm-0.24.0/setup.py` & `usdm-0.25.0/setup.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm.egg-info/PKG-INFO` & `usdm-0.25.0/src/usdm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.24.0
+Version: 0.25.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -138,15 +138,15 @@
 | Column | Column Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
 | B | organisationIdentifier | Organisation identifier | Text string |
 | C | organisationName | Organisation name | Text string |
 | D | organisationType | Organisation type | CDISC code reference |
 | E | studyIdentifier | The identifier for the study | Text string |
-| F | organisationAddress | The organisation address | Formated using a pipe delimited - allows for commas in items within the address - form, i.e. `line|city|district|state|postal_code|<country code>`. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. |
+| F | organisationAddress | The organisation address | Formated using a pipe delimited form `line|city|district|state|postal_code|<country code>`. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. |
 
 ### Study Design sheet
 
 #### Sheet Name
 
 `studyDesign`
 
@@ -167,17 +167,51 @@
 | 7 | trialTypes | Code for the trial type | CDISC code reference|
 | 8 | interventionModel | | CDISC code reference |
 | 9 | mainTimeline | Name of main timeline sheet | This must be present |
 | 10 | otherTimelines | Names of other timeline sheeText string | Commma separated list of sheet names. Can be empty |
 
 For the arms and epochs, a simple table is required. The table starts in row 12 and can consists of a header row and 1 or more arm rows. 
 
-The header row consists of a cell that is ignored followed by 1 or more cells containing the epoch names.
+The header row consists of a cell in column A that is ignored followed by 1 or more cells (columns) containing the epoch names. Each epoch name should have a corresponding entry in the Study Design Epochs sheet, see below.
 
-The arm rows consist of the arm name in the first column followed by a cells for each epoch containing one or more references to study design elements defined in the studyDesignElements sheet.
+The arm rows consist of the arm name in the first column followed by a cells for each epoch containing one or more references to study design elements defined in the studyDesignElements sheet. Each arm name should have a corresponding entry in the Study Design Arms sheet, see bwlow.
+
+### Study Design Arms sheet
+
+#### Sheet Name
+
+`studyDesignArms`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2, containing the details of a study arm: 
+
+| Column | Column Name | Description | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | studyArmName | The study name | Text string. Should match an arm name in the Study Design sheet | 
+| B | studyArmDescription | A Text string description for the arm | Text string |
+| C | studyArmType | The arm type| CDISC code reference |
+| D | studyArmDataOriginDescription	| The description of the data origin for the arm | Text string |
+| E | studyArmDataOriginType | The type of arm data origin | CDISC code reference|
+
+### Study Design Epochs sheet
+
+#### Sheet Name
+
+`studyDesignEpochs`
+
+#### Sheet Contents
+
+A header row in row 1 followed by repeating rows from row 2, containing the details of a study epoch: 
+
+| Column | Column Name | Description | Format and Values |
+| :--- | :--- | :--- | :--- |
+| A | studyEpochName | The epoch name | Text string. Should match an epoch name in the Study Design sheet | 
+| B | studyEpochDescription | A Text string description for the epoch | Text string |
+| C | studyEpochType | The epoch type| CDISC code reference |
 
 ### Timeline sheets
 
 #### Sheet Name
 
 As defined within the study design sheet, see above.
```

### Comparing `usdm-0.24.0/src/usdm.egg-info/SOURCES.txt` & `usdm-0.25.0/src/usdm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,22 @@
 src/usdm_excel/option_manager.py
 src/usdm_excel/data/cdisc_ct_config.yaml
 src/usdm_excel/data/iso_3166.json
 src/usdm_excel/data/missing_ct.yaml
 src/usdm_excel/errors/__init__.py
 src/usdm_excel/errors/error.py
 src/usdm_excel/errors/errors.py
+src/usdm_excel/study_design_arm_sheet/__init__.py
+src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
 src/usdm_excel/study_design_element_sheet/__init__.py
 src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
 src/usdm_excel/study_design_encounter_sheet/__init__.py
 src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+src/usdm_excel/study_design_epoch_sheet/__init__.py
+src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
 src/usdm_excel/study_design_estimands_sheet/__init__.py
 src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
 src/usdm_excel/study_design_ii_sheet/__init__.py
 src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
 src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
 src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
 src/usdm_excel/study_design_population_sheet/__init__.py
@@ -97,8 +101,10 @@
 src/usdm_model/transition_rule.py
 tests/test_base_sheet.py
 tests/test_cdisc_biomedical_concept.py
 tests/test_error.py
 tests/test_errors.py
 tests/test_iso_3166.py
 tests/test_ncit.py
-tests/test_option_manager.py
+tests/test_option_manager.py
+tests/test_study_design_arm_sheet.py
+tests/test_study_design_epoch_sheet.py
```

### Comparing `usdm-0.24.0/src/usdm_excel/__init__.py` & `usdm-0.25.0/src/usdm_excel/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/base_sheet.py` & `usdm-0.25.0/src/usdm_excel/base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/cdisc_biomedical_concept.py` & `usdm-0.25.0/src/usdm_excel/cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/cdisc_ct.py` & `usdm-0.25.0/src/usdm_excel/cdisc_ct.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/cdisc_ct_library.py` & `usdm-0.25.0/src/usdm_excel/cdisc_ct_library.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/configuration_sheet.py` & `usdm-0.25.0/src/usdm_excel/configuration_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/data/cdisc_ct_config.yaml` & `usdm-0.25.0/src/usdm_excel/data/cdisc_ct_config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -20,27 +20,29 @@
 - C188726 
 - C188725
 - C188723
 - C188724
 - C66728
 - C66735
 - C66732
+- C174222
 klass:
   Study:
     studyType: C99077
     studyPhase: C66737
   StudyProtocolVersion:
     protocolStatus: C188723
   Organisation:
     organisationType: C188724
   Objective:
     objectiveLevel: C188725
   Endpoint:
     endpointLevel: C188726
   StudyArm:
+    studyArmType: C174222
     studyArmDataOriginType: C188727
   StudyEpoch:
     studyEpochType: C99079
   Encounter:
     encounterType: C188728
     encounterEnvironmentalSetting: C127262
     encounterContactModes: C171445
```

### Comparing `usdm-0.24.0/src/usdm_excel/data/iso_3166.json` & `usdm-0.25.0/src/usdm_excel/data/iso_3166.json`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/data/missing_ct.yaml` & `usdm-0.25.0/src/usdm_excel/data/missing_ct.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/errors/error.py` & `usdm-0.25.0/src/usdm_excel/errors/error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/errors/errors.py` & `usdm-0.25.0/src/usdm_excel/errors/errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/id_manager.py` & `usdm-0.25.0/src/usdm_excel/id_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/iso_3166.py` & `usdm-0.25.0/src/usdm_excel/iso_3166.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
   def __init__(self):
     f = open(os.path.join(os.path.dirname(__file__), 'data', 'iso_3166.json'))
     self.db = json.load(f)
 
   def code(self, code):
     code, decode = self._get_decode(code)
-    return Code(codeId=id_manager.build_id(Code), code=code, codeSystem='ISO 3166 1 alpha3', codeSystemVersion='', decode=decode)
+    return Code(codeId=id_manager.build_id(Code), code=code, codeSystem='ISO 3166 1 alpha3', codeSystemVersion='2020-08', decode=decode)
 
   def _get_decode(self, code):
     if len(code) == 2:
       field = 'alpha-2'
     else:
       field = 'alpha-3'
     entry = next((item for item in self.db if item[field] == code), None)
```

### Comparing `usdm-0.24.0/src/usdm_excel/nodes_and_edges.py` & `usdm-0.25.0/src/usdm_excel/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/option_manager.py` & `usdm-0.25.0/src/usdm_excel/option_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
       #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name='studyDesignOE'))
       super().__init__(file_path=file_path, sheet_name='studyDesignOE')
       self.objectives = []
       current = None
       for index, row in self.sheet.iterrows():
         o_xref = self.read_cell_by_name(index, "objectiveXref")
         o_description = self.read_cell_by_name(index, "objectiveDescription")
-        o_level = self.read_cdisc_klass_attribute_cell_by_name('Objective', 'objectiveLevel', index, "objectiveLevel")
         e_xref = self.read_cell_by_name(index, "endpointXref")
         e_description = self.read_cell_by_name(index, "endpointDescription")
         e_p_description = self.read_cell_by_name(index, "endpointPurposeDescription")
         e_level = self.read_cdisc_klass_attribute_cell_by_name('Endpoint', 'endpointLevel', index, "endpointLevel")
         if not o_description == "":
+          o_level = self.read_cdisc_klass_attribute_cell_by_name('Objective', 'objectiveLevel', index, "objectiveLevel")
           current = Objective(objectiveId=id_manager.build_id(Objective),
             objectiveDescription=o_description, 
             objectiveLevel=o_level,
             objectiveEndpoints=[]
           )
           self.objectives.append(current)
           cross_references.add(o_xref, current.objectiveId)
```

### Comparing `usdm-0.24.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_design_sheet/study_design_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_design_sheet/study_design_sheet.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
   EPOCH_ARMS_START_ROW = 11
   
   PARAMS_DATA_COL = 1
 
   def __init__(self, file_path):
     try:
-      #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name='studyDesign', header=None))
       super().__init__(file_path=file_path, sheet_name='studyDesign', header=None)
       self.name = "TEST"
       self.description = "An Microsoft Excel test study design"
       self.epochs = []
       self.arms = []
       self.cells = []
       self.study_designs = []
@@ -76,19 +75,19 @@
 
     for rindex, row in self.sheet.iterrows():
       if rindex >= self.EPOCH_ARMS_START_ROW:
         for cindex in range(0, len(self.sheet.columns)):
           cell = self.read_cell(rindex, cindex)
           if rindex == self.EPOCH_ARMS_START_ROW:
             if cindex != 0:
-              epoch = self._add_epoch(cell, cell)
+              epoch = self._add_epoch(cell)
               self.epochs.append(epoch)
           else:
             if cindex == 0:
-              self.arms.append(self._add_arm(cell, cell))
+              self.arms.append(self._add_arm(cell))
             else:
               elements = []
               element_names = self.read_cell_multiple(rindex, cindex)
               for name in element_names:
                 elements.append(cross_references.get(name))
               self.cells.append(self._add_cell(arm=self.arms[-1], epoch=self.epochs[cindex-1], elements=elements))
     
@@ -103,36 +102,19 @@
       intervention_model=self.intervention_model,
       rationale=self.rationale, 
       blinding=self.blinding, 
       therapeutic_areas=self.therapeutic_areas
     )
     self.study_designs.append(study_design)
 
-  def _add_arm(self, name, description):
-    # TODO read the arm origin and type
-    arm_origin = self.set_cdisc_code("C188866=Data Generated Within Study")
-    arm_type = self.set_cdisc_code("C174266=Experimental Arm")
-    return StudyArm(
-      studyArmId=id_manager.build_id(StudyArm), 
-      studyArmName=name,
-      studyArmDescription=description,
-      studyArmType=arm_type,
-      studyArmDataOriginDescription="",
-      studyArmDataOriginType=arm_origin
-    )
+  def _add_arm(self, name):
+    return cross_references.get(name)
 
-  def _add_epoch(self, name, description):
-    # TODO read the epoch type
-    epoch_type = self.set_cdisc_code("C165873=OBSERVATION")
-    return StudyEpoch(
-      studyEpochId=id_manager.build_id(StudyEpoch), 
-      studyEpochName=name, 
-      studyEpochDescription=description,
-      studyEpochType=epoch_type
-    )
+  def _add_epoch(self, name):
+    return cross_references.get(name)
   
   def _add_cell(self, arm, epoch, elements):
     return StudyCell(
       studyCellId=id_manager.build_id(StudyCell), 
       studyArm=arm,
       studyEpoch=epoch,
       studyElements=elements
```

### Comparing `usdm-0.24.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_sheet/study_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_sheet/study_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from usdm_excel.study_design_ii_sheet.study_design_ii_sheet import StudyDesignIISheet
 from usdm_excel.study_design_population_sheet.study_design_population_sheet import StudyDesignPopulationSheet
 from usdm_excel.study_design_objective_endpoint_sheet.study_design_objective_endpoint_sheet import StudyDesignObjectiveEndpointSheet
 from usdm_excel.study_design_estimands_sheet.study_design_estimands_sheet import StudyDesignEstimandsSheet
 from usdm_excel.study_design_procedure_sheet.study_design_procedure_sheet import StudyDesignProcedureSheet
 from usdm_excel.study_design_encounter_sheet.study_design_encounter_sheet import StudyDesignEncounterSheet
 from usdm_excel.study_design_element_sheet.study_design_element_sheet import StudyDesignElementSheet
+from usdm_excel.study_design_arm_sheet.study_design_arm_sheet import StudyDesignArmSheet
+from usdm_excel.study_design_epoch_sheet.study_design_epoch_sheet import StudyDesignEpochSheet
 from usdm_excel.alias import Alias
 from usdm_excel.id_manager import id_manager
 from usdm_excel.cross_ref import cross_references
 from usdm_excel.option_manager import *
 from usdm_model.api_base_model import ApiBaseModel
 from usdm_model.study import Study
 from usdm_model.study_protocol_version import StudyProtocolVersion
@@ -53,14 +55,16 @@
       self.therapeutic_areas = []
       self.timelines = {}
       self._process_sheet()
       self.study_identifiers = StudyIdentifiersSheet(file_path)
       self.procedures = StudyDesignProcedureSheet(file_path)
       self.encounters = StudyDesignEncounterSheet(file_path)
       self.elements = StudyDesignElementSheet(file_path)
+      self.arms = StudyDesignArmSheet(file_path)
+      self.epochs = StudyDesignEpochSheet(file_path)
       self.study_design = StudyDesignSheet(file_path)
       for timeline in self.study_design.other_timelines:
         tl = StudySoASheet(file_path, timeline)
         self.timelines[timeline] = tl
         cross_references.add(timeline, tl.timeline.scheduleTimelineId)
       self.soa = StudySoASheet(file_path, self.study_design.main_timeline)
       self.ii = StudyDesignIISheet(file_path)
```

### Comparing `usdm-0.24.0/src/usdm_excel/study_soa_sheet/activities.py` & `usdm-0.25.0/src/usdm_excel/study_soa_sheet/activities.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_soa_sheet/activity.py` & `usdm-0.25.0/src/usdm_excel/study_soa_sheet/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_soa_sheet/cycle.py` & `usdm-0.25.0/src/usdm_excel/study_soa_sheet/cycle.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_soa_sheet/cycles.py` & `usdm-0.25.0/src/usdm_excel/study_soa_sheet/cycles.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_soa_sheet/encounters.py` & `usdm-0.25.0/src/usdm_excel/study_soa_sheet/encounters.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py` & `usdm-0.25.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,20 @@
 
       for item in self._raw_activities.items:
         self.activities.append(item.usdm_activity)
         self.biomedical_concept_surrogates += item.usdm_biomedical_concept_surrogates
         self.biomedical_concepts += item.usdm_biomedical_concepts
       self.double_link(self.activities, 'activityId', 'previousActivityId', 'nextActivityId')
       
+      seq_number = 1
       for raw_timepoint in self._raw_timepoints.items:
         instance = raw_timepoint.usdm_timepoint
+        instance.scheduleSequenceNumber = seq_number
         instances.append(instance)
+        seq_number += 1
       exit = self._add_exit()
       self.timeline = self._add_timeline(self.name, self.description, self.condition, instances, exit)
 
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet")
       self._traceback(f"{traceback.format_exc()}")
```

### Comparing `usdm-0.24.0/src/usdm_excel/study_soa_sheet/timepoint.py` & `usdm-0.25.0/src/usdm_excel/study_soa_sheet/timepoint.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_excel/study_soa_sheet/timepoints.py` & `usdm-0.25.0/src/usdm_excel/study_soa_sheet/timepoints.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_model/__init__.py` & `usdm-0.25.0/src/usdm_model/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_model/activity.py` & `usdm-0.25.0/src/usdm_model/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_model/api_base_model.py` & `usdm-0.25.0/src/usdm_model/api_base_model.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_model/encounter.py` & `usdm-0.25.0/src/usdm_model/encounter.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_model/estimand.py` & `usdm-0.25.0/src/usdm_model/estimand.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_model/scheduled_instance.py` & `usdm-0.25.0/src/usdm_model/scheduled_instance.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_model/study.py` & `usdm-0.25.0/src/usdm_model/study.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_model/study_design.py` & `usdm-0.25.0/src/usdm_model/study_design.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/src/usdm_model/study_identifier.py` & `usdm-0.25.0/src/usdm_model/study_identifier.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/tests/test_base_sheet.py` & `usdm-0.25.0/tests/test_base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/tests/test_cdisc_biomedical_concept.py` & `usdm-0.25.0/tests/test_cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/tests/test_error.py` & `usdm-0.25.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/tests/test_errors.py` & `usdm-0.25.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.24.0/tests/test_iso_3166.py` & `usdm-0.25.0/tests/test_iso_3166.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
     mock_id = mocker.patch("usdm_excel.id_manager.build_id")
     mock_id.side_effect=['Code_1', 'Code_2', 'Code_3']
     item = ISO3166()
     code = item.code("GB")
     assert code.codeId == "Code_1"
     assert code.code == "GBR"
     assert code.codeSystem == "ISO 3166 1 alpha3"
-    assert code.codeSystemVersion == ""
+    assert code.codeSystemVersion == "2020-08"
     assert code.decode == "United Kingdom of Great Britain and Northern Ireland"
     code = item.code("GBR")
     assert code.codeId == "Code_2"
     assert code.code == "GBR"
     assert code.codeSystem == "ISO 3166 1 alpha3"
-    assert code.codeSystemVersion == ""
+    assert code.codeSystemVersion == "2020-08"
     assert code.decode == "United Kingdom of Great Britain and Northern Ireland"
     code = item.code("XXX")
     assert code.codeId == "Code_3"
     assert code.code == "DNK"
     assert code.codeSystem == "ISO 3166 1 alpha3"
-    assert code.codeSystemVersion == ""
+    assert code.codeSystemVersion == "2020-08"
     assert code.decode == "Denmark"
```

### Comparing `usdm-0.24.0/tests/test_option_manager.py` & `usdm-0.25.0/tests/test_option_manager.py`

 * *Files identical despite different names*

