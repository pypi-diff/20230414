# Comparing `tmp/dkist-processing-common-2.4.0rc2.tar.gz` & `tmp/dkist-processing-common-2.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-2.4.0rc2.tar", last modified: Mon Apr 10 20:18:37 2023, max compression
+gzip compressed data, was "dkist-processing-common-2.4.1rc1.tar", last modified: Fri Apr 14 20:01:30 2023, max compression
```

## Comparing `dkist-processing-common-2.4.0rc2.tar` & `dkist-processing-common-2.4.1rc1.tar`

### file list

```diff
@@ -1,117 +1,115 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    11208 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.866137 dkist-processing-common-2.4.0rc2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/changelog/129.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.866137 dkist-processing-common-2.4.0rc2/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.870137 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.870137 dkist-processing-common-2.4.0rc2/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.870137 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4959 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3304 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     2017 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     7365 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.874137 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6264 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5598 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.874137 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     8152 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10675 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.874137 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13155 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.874137 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8226 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47853 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7127 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)    17272 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     9758 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_l1_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10499 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36040 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11128 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    13919 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.870137 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4266 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      585 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.569337 dkist-processing-common-2.4.1rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/changelog/128.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.569337 dkist-processing-common-2.4.1rc1/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.573337 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.573337 dkist-processing-common-2.4.1rc1/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.573337 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3304 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7365 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.573337 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6264 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5598 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.577338 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10675 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.577338 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13155 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.577338 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8226 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     7123 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18801 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     9758 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_l1_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10499 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36040 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11128 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14982 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.569337 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/setup.py
```

### Comparing `dkist-processing-common-2.4.0rc2/.gitignore` & `dkist-processing-common-2.4.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/.pre-commit-config.yaml` & `dkist-processing-common-2.4.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/CHANGELOG.rst` & `dkist-processing-common-2.4.1rc1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+v2.4.0 (2023-04-12)
+===================
+
+Features
+--------
+
+- Make histogram plots of all parameters that are free in local PolCal fits. (`#132 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/132>`__)
+
+
+Misc
+----
+
+- Update polcal quality metric machinery for new `dkist-processing-pac` version (>=2.0.0). (`#129 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/129>`__)
+- Normalize use of `logger.[thing]` across repo. Previously had also been using `logging.[thing]`. (`#130 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/130>`__)
+
+
 v2.3.0 (2023-02-17)
 ===================
 
 Misc
 ----
 
 - Update dkist-processing-core to include new version of Airflow
```

### Comparing `dkist-processing-common-2.4.0rc2/PKG-INFO` & `dkist-processing-common-2.4.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.4.0rc2
+Version: 2.4.1rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.4.0rc2/README.rst` & `dkist-processing-common-2.4.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/bitbucket-pipelines.yml` & `dkist-processing-common-2.4.1rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/check_changelog_updated.sh` & `dkist-processing-common-2.4.1rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/config.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/constants.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/tags.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/manual.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/constants.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     experiment_id = "EXPERIMENT_ID"
     contributing_experiment_ids = "CONTRIBUTING_EXPERIMENT_IDS"
     average_cadence = "AVERAGE_CADENCE"
     maximum_cadence = "MAXIMUM_CADENCE"
     minimum_cadence = "MINIMUM_CADENCE"
     variance_cadence = "VARIANCE_CADENCE"
     num_dsps_repeats = "NUM_DSPS_REPEATS"
-    spectral_line = "SPECTRAL_LINE"
     dark_exposure_times = "DARK_EXPOSURE_TIMES"
 
 
 class ConstantsBase:
     """
     Aggregate (from the constant flowers flower pot) in a single property on task classes.
 
@@ -124,19 +123,14 @@
 
     @property
     def num_dsps_repeats(self) -> int:
         """Get the number of dsps repeats."""
         return self._db_dict[BudName.num_dsps_repeats]
 
     @property
-    def spectral_line(self) -> str:
-        """Get the spectral line for this task."""
-        return self._db_dict[BudName.spectral_line]
-
-    @property
     def dark_exposure_times(self) -> list[float]:
         """Get a list of exposure times used in the dark calibration."""
         return self._db_dict[BudName.dark_exposure_times]  # TODO type hinting mismatch here
 
     @property
     def stokes_params(self) -> [str]:
         """Return the list of stokes parameter names."""
```

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/graphql.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/json_encoder.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/message.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/parameters.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/quality.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/tags.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/time.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/base.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 from dkist_processing_common.models.quality import Plot2D
 from dkist_processing_common.models.quality import PlotHistogram
 from dkist_processing_common.models.quality import PlotRaincloud
 from dkist_processing_common.models.quality import ReportMetric
 from dkist_processing_common.models.quality import SimpleTable
 from dkist_processing_common.models.tags import Tag
 
+logger = logging.getLogger(__name__)
+
 
 class _SimpleQualityMixin:
     @staticmethod
     def _create_statement_metric(
         name: str, description: str, statement: str, warnings: Optional[str] = None
     ) -> dict:
         metric = ReportMetric(
@@ -638,41 +640,41 @@
         bins_2: int,
         bin_1_type: str,
         bin_2_type: str,
         skip_recording_constant_pars: bool = False,
     ):
         """Compute and store all PolCal related metrics."""
         if not skip_recording_constant_pars:
-            logging.info("Storing constant parameter values")
+            logger.info("Storing constant parameter values")
             self._store_polcal_constant_parameter_values(polcal_fitter=polcal_fitter, label=label)
 
-        logging.info("Storing global parameter values")
+        logger.info("Storing global parameter values")
         self._store_polcal_global_parameter_values(polcal_fitter=polcal_fitter, label=label)
 
-        logging.info("Storing local parameter values")
+        logger.info("Storing local parameter values")
         self._store_polcal_local_parameter_values(
             polcal_fitter=polcal_fitter,
             label=label,
             bins_1=bins_1,
             bins_2=bins_2,
             bin_1_type=bin_1_type,
             bin_2_type=bin_2_type,
         )
 
-        logging.info("Storing fit residuals")
+        logger.info("Storing fit residuals")
         self._store_polcal_fit_resdiuals(
             polcal_fitter=polcal_fitter,
             label=label,
             bins_1=bins_1,
             bins_2=bins_2,
             bin_1_type=bin_1_type,
             bin_2_type=bin_2_type,
         )
 
-        logging.info("Storing modulation matrix efficiencies")
+        logger.info("Storing modulation matrix efficiencies")
         self._store_polcal_modulation_efficiency(
             polcal_fitter=polcal_fitter,
             label=label,
             bins_1=bins_1,
             bins_2=bins_2,
             bin_1_type=bin_1_type,
             bin_2_type=bin_2_type,
```

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,27 +131,27 @@
             The flower pot to be updated
         Returns
         -------
         None
         """
         for flower in constant_pot:
             with self.apm_processing_step(f"Setting value of constant {flower.stem_name}"):
-                logging.info(f"Setting value of constant {flower.stem_name}")
+                logger.info(f"Setting value of constant {flower.stem_name}")
                 try:
                     if flower.bud.value is Thorn:
                         # Must've been a picky bud that passed. We don't want to pick it because it has no value
                         continue
                     # If the value is a set, sort it before storing in redis
                     if isinstance(flower.bud.value, set):
                         sorted_value = json.dumps(sorted(flower.bud.value))
                         self.constants._update({flower.stem_name: sorted_value})
-                        logging.info(f"Value of {flower.stem_name} set to {sorted_value}")
+                        logger.info(f"Value of {flower.stem_name} set to {sorted_value}")
                     else:
                         self.constants._update({flower.stem_name: flower.bud.value})
-                        logging.info(f"Value of {flower.stem_name} set to {flower.bud.value}")
+                        logger.info(f"Value of {flower.stem_name} set to {flower.bud.value}")
                 except StopIteration:
                     # There are no petals
                     pass
 
     def tag_petals(self, tag_pot: FlowerPot):
         """
         Apply tags to file paths.
@@ -162,12 +162,12 @@
             The flower pot to be tagged
         Returns
         -------
         None
         """
         for flower in tag_pot:
             with self.apm_processing_step(f"Applying {flower.stem_name} tag to files"):
-                logging.info(f"Applying {flower.stem_name} tag to files")
+                logger.info(f"Applying {flower.stem_name} tag to files")
                 for petal in flower.petals:
                     tag = Tag.format_tag(flower.stem_name, petal.value)
                     for path in petal.keys:
                         self.tag(path, tag)
```

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/write_l1.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,42 +13,64 @@
 from astropy.io import fits
 from astropy.time import Time
 from dkist_fits_specifications import __version__ as spec_version
 from dkist_fits_specifications.utils.formatter import reformat_spec214_header
 from dkist_header_validator import spec214_validator
 from dkist_header_validator.translator import remove_extra_axis_keys
 from dkist_header_validator.translator import sanitize_to_spec214_level1
+from dkist_spectral_lines.search import get_closest_spectral_line
+from dkist_spectral_lines.search import get_spectral_lines
+from pydantic import BaseModel
+from pydantic import validator
 from scipy.stats import kurtosis
 from scipy.stats import skew
 from sunpy.coordinates import HeliocentricInertial
 
 from dkist_processing_common._util.dkist_location import location_of_dkist
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.parsers.l0_fits_access import L0FitsAccess
 from dkist_processing_common.tasks import WorkflowTaskBase
 
+logger = logging.getLogger(__name__)
 
-__all__ = ["WriteL1Frame"]
+__all__ = ["WriteL1Frame", "WavelengthRange"]
 
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.metadata_store import MetadataStoreMixin
 
 
+class WavelengthRange(BaseModel):
+    """Model for holding the range of wavelengths assigned to a frame."""
+
+    min: u.Quantity
+    max: u.Quantity
+
+    @validator("min", "max")
+    def convert_to_nanometers(cls, v):
+        """Validate wavelength unit is for distance and convert to nanometers."""
+        return v.to(u.nm)
+
+    class Config:
+        """pydantic.BaseModel configuration."""
+
+        arbitrary_types_allowed = True
+
+
 class WriteL1Frame(WorkflowTaskBase, FitsDataMixin, MetadataStoreMixin, ABC):
     """
     Task to convert final calibrated science frames into spec 214 compliant level 1 frames.
 
     It is intended to be subclassed as the dataset header table is instrument specific.
     """
 
     def run(self) -> None:
         """Run method for this task."""
         for stokes_param in self.constants.stokes_params:
             with self.apm_task_step(f"Get calibrated frames for stokes param {stokes_param}"):
-                logging.info(f"Get calibrated frames for stokes param {stokes_param}")
+                logger.info(f"Get calibrated frames for stokes param {stokes_param}")
                 tags = [Tag.frame(), Tag.calibrated(), Tag.stokes(stokes_param)]
                 calibrated_fits_objects = self.fits_data_read_fits_access(
                     tags=tags,
                     cls=L0FitsAccess,
                     auto_squeeze=False,
                 )
                 num_files = self.scratch.count_all(tags)
@@ -74,15 +96,15 @@
                     hdu = fits.CompImageHDU(
                         header=formatted_header, data=hdu.data, tile_size=tile_size
                     )
                     all_tags = self.tags(calibrated_fits_object.name)
                     all_tags.remove(Tag.calibrated())
                     relative_path = self.l1_filename(header=l1_header, stokes=stokes_param)
                     temp_file_name = Path(calibrated_fits_object.name).name
-                    logging.debug(
+                    logger.debug(
                         f"{file_num} of {num_files}: Translate and write frame {temp_file_name} to {relative_path}"
                     )
                     self.fits_data_write(
                         hdu_list=fits.HDUList([fits.PrimaryHDU(), hdu]),
                         tags=[Tag.output()] + all_tags,
                         relative_path=relative_path,
                     )
@@ -149,15 +171,14 @@
         header["DATAKURT"] = kurtosis(data, nan_policy="omit")
         header["DATASKEW"] = skew(data, nan_policy="omit")
         return header
 
     def _add_datacenter_headers(
         self,
         header: fits.Header,
-        data: np.ndarray,
         hdu_size: float,
         stokes: Literal["I", "Q", "U", "V"],
     ) -> fits.Header:
         """Fill out the spec 214 datacenter header table."""
         header["DSETID"] = self.constants.dataset_id
         header["POINT_ID"] = self.constants.dataset_id
         header["FRAMEVOL"] = hdu_size / 1024 / 1024
@@ -180,17 +201,36 @@
         if ids_obs_id := self.metadata_store_input_dataset_observe_frames_part_id:
             header["IDSOBSID"] = ids_obs_id
         if ids_cal_id := self.metadata_store_input_dataset_calibration_frames_part_id:
             header["IDSCALID"] = ids_cal_id
         header["WKFLNAME"] = self.workflow_name
         header["WKFLVERS"] = self.workflow_version
         header = self._add_contributing_id_headers(header=header)
-
+        # Spectral line keywords
+        header["WAVEBAND"] = get_closest_spectral_line(wavelength=header["LINEWAV"] * u.nm).name
+        wavelength_range = self.get_wavelength_range(header=header)
+        spectral_lines = get_spectral_lines(
+            wavelength_min=wavelength_range.min,
+            wavelength_max=wavelength_range.max,
+        )
+        if spectral_lines:
+            header["NSPECLNS"] = len(spectral_lines)
+            for i, l in enumerate(spectral_lines):
+                header[f"SPECLN{str(i + 1).zfill(2)}"] = l.name
         return header
 
+    @abstractmethod
+    def get_wavelength_range(self, header: fits.Header) -> WavelengthRange:
+        """
+        Determine the wavelength range covered by the data in this frame.
+
+        For imagers, this is generally the wavelengths covered by the filter.
+        For spectrographs, this is the wavelengths covered by the spectral axis of the data.
+        """
+
     def _add_solarnet_headers(self, header: fits.Header) -> fits.Header:
         """Add headers recommended by solarnet that haven't already been added."""
         header["DATE-AVG"] = self._calculate_date_avg(header=header)
         header["TELAPSE"] = self._calculate_telapse(header=header)
         header["DATEREF"] = header["DATE-BEG"]
         itrs = location_of_dkist()
         header["OBSGEO-X"] = itrs.x.to_value(unit=u.m)
@@ -273,17 +313,15 @@
         A header translated to L1
         """
         # Replace header values in place
         header = self._replace_header_values(header=header, data=data)
         # Add the stats table
         header = self._add_stats_headers(header=header, data=data)
         # Add the datacenter table
-        header = self._add_datacenter_headers(
-            header=header, data=data, hdu_size=hdu_size, stokes=stokes_param
-        )
+        header = self._add_datacenter_headers(header=header, hdu_size=hdu_size, stokes=stokes_param)
         # Add extra headers recommended by solarnet (not all in a single table)
         header = self._add_solarnet_headers(header=header)
         # Add the documentation headers
         header = self._add_doc_headers(header=header)
         # Add the dataset headers (abstract - implement in instrument task)
         header = self.add_dataset_headers(header=header, stokes=stokes_param)
         # Remove any headers not contained in spec 214
```

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_l1_output_data_base.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_l1_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_write_l1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from dataclasses import asdict
 from dataclasses import dataclass
 from typing import Literal
 from unittest.mock import Mock
 
+import astropy.units as u
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.time import Time
 from astropy.time import TimeDelta
 from dkist_fits_specifications import __version__ as spec_version
 from dkist_header_validator import spec214_validator
 
 from dkist_processing_common import __version__ as common_version
 from dkist_processing_common.models.tags import Tag
+from dkist_processing_common.tasks.write_l1 import WavelengthRange
 from dkist_processing_common.tasks.write_l1 import WriteL1Frame
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from dkist_processing_common.tests.conftest import FakeGQLClientNoRecipeConfiguration
 from dkist_processing_common.tests.conftest import TILE_SIZE
 
 
 class CompleteWriteL1Frame(WriteL1Frame):
@@ -67,14 +69,17 @@
         return header
 
     def _calculate_date_end(self, header: fits.Header) -> str:
         start_time = Time(header["DATE-BEG"], format="isot", precision=6)
         exposure = TimeDelta(float(header["TEXPOSUR"]) / 1000, format="sec")
         return (start_time + exposure).to_value("isot")
 
+    def get_wavelength_range(self, header: fits.Header) -> WavelengthRange:
+        return WavelengthRange(min=1075.0 * u.nm, max=1085.0 * u.nm)
+
 
 @dataclass
 class FakeConstantDb:
     INSTRUMENT: str = "TEST"
     DATASET_ID: str = "DATASETID"
     AVERAGE_CADENCE: float = 10.0
     MINIMUM_CADENCE: float = 10.0
@@ -239,14 +244,15 @@
         header = fits.open(file)[1].header
         assert header["DATEREF"] == header["DATE-BEG"]
         assert round(header["OBSGEO-X"]) == -5466045
         assert round(header["OBSGEO-Y"]) == -2404389
         assert round(header["OBSGEO-Z"]) == 2242134
         assert header["SPECSYS"] == "TOPOCENT"
         assert header["VELOSYS"] == 0.0
+        assert header["WAVEBAND"] == "Fe XIII (1079.8 nm)"
 
 
 def test_documentation_keys(write_l1_task, mocker):
     """
     :Given: files with headers converted to SPEC 214 L1
     :When: checking the documentation header URLs
     :Then: the correct values are found
@@ -384,7 +390,29 @@
     # Ensure that there are contributing experiment IDs
     assert header["EXPRID01"] == "EXPERID1"
     assert header["EXPRID02"] == "EXPERID2"
     assert header["EXPRID03"] == "EXPERID3"
     # Check total numbers
     assert header["NPROPOS"] == 1
     assert header["NEXPERS"] == 3
+
+
+def test_spectral_line_keys(write_l1_task, complete_common_header, mocker):
+    """
+    :Given: a header
+    :When: adding spectral line information to the headers
+    :Then: the correct values are added
+    """
+    mocker.patch(
+        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient",
+        new=FakeGQLClient,
+    )
+    task, _ = write_l1_task
+    header = task._add_datacenter_headers(
+        header=complete_common_header, hdu_size=1024, stokes=["I", "Q", "U", "V"]
+    )
+    assert header["WAVEBAND"] == "Fe XIII (1079.8 nm)"
+    assert header["SPECLN01"] == "Fe XIII (1079.8 nm)"
+    assert header["SPECLN02"] == "He I (1083.0 nm)"
+    assert header["NSPECLNS"] == 2
+    with pytest.raises(KeyError):
+        assert header["SPECLN03"]
```

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.4.0rc2
+Version: 2.4.1rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
-changelog/129.misc.rst
+changelog/128.misc.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
@@ -31,15 +31,14 @@
 dkist_processing_common/models/fits_access.py
 dkist_processing_common/models/flower_pot.py
 dkist_processing_common/models/graphql.py
 dkist_processing_common/models/json_encoder.py
 dkist_processing_common/models/message.py
 dkist_processing_common/models/parameters.py
 dkist_processing_common/models/quality.py
-dkist_processing_common/models/spectral_line.py
 dkist_processing_common/models/tags.py
 dkist_processing_common/parsers/__init__.py
 dkist_processing_common/parsers/cs_step.py
 dkist_processing_common/parsers/dsps_repeat.py
 dkist_processing_common/parsers/experiment_id_bud.py
 dkist_processing_common/parsers/id_bud.py
 dkist_processing_common/parsers/l0_fits_access.py
@@ -82,15 +81,14 @@
 dkist_processing_common/tests/test_l1_output_data_base.py
 dkist_processing_common/tests/test_parameters.py
 dkist_processing_common/tests/test_parse_l0_input_data.py
 dkist_processing_common/tests/test_publish_catalog_messages.py
 dkist_processing_common/tests/test_quality.py
 dkist_processing_common/tests/test_quality_mixin.py
 dkist_processing_common/tests/test_scratch.py
-dkist_processing_common/tests/test_spectral_line.py
 dkist_processing_common/tests/test_tags.py
 dkist_processing_common/tests/test_teardown.py
 dkist_processing_common/tests/test_transfer_input_data.py
 dkist_processing_common/tests/test_transfer_l1_output_data.py
 dkist_processing_common/tests/test_workflow_task_base.py
 dkist_processing_common/tests/test_write_l1.py
 docs/Makefile
```

### Comparing `dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 dkist-processing-core==1.3.0
-dkist-processing-pac>=2.0.0rc1
+dkist-processing-pac>=2.0.0
 dkist-header-validator>=2.0.11
 dkist-fits-specifications>=3.0.0
 astropy>=5.1.1
 numpy>=1.20.2
 pandas>=1.4.2
 hashids==1.3.1
 globus-sdk>=3.12.0
 gqlclient==0.9.6
-talus==0.2.0
+talus==0.2.1
 redis==4.3.4
 object-clerk==0.1.0
 requests>=2.23
 scipy>=1.6.3
 sunpy>=3.0.0
 pillow>=8.3.0
 moviepy>=1.0.3
 matplotlib>=3.4
 pydantic>=1.8.1
 retry>=0.9.2
+dkist-spectral-lines
 
 [docs]
 sphinx
 sphinx-astropy
 sphinx-changelog
 sphinx-autoapi
 pytest
```

### Comparing `dkist-processing-common-2.4.0rc2/docs/Makefile` & `dkist-processing-common-2.4.1rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/docs/conf.py` & `dkist-processing-common-2.4.1rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/docs/make.bat` & `dkist-processing-common-2.4.1rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/licenses/LICENSE.rst` & `dkist-processing-common-2.4.1rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/pyproject.toml` & `dkist-processing-common-2.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc2/setup.cfg` & `dkist-processing-common-2.4.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -16,34 +16,35 @@
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
 	dkist-processing-core == 1.3.0
-	dkist-processing-pac >= 2.0.0rc1
+	dkist-processing-pac >= 2.0.0
 	dkist-header-validator >= 2.0.11
 	dkist-fits-specifications >= 3.0.0
 	astropy >= 5.1.1
 	numpy >= 1.20.2
 	pandas >= 1.4.2
 	hashids == 1.3.1
 	globus-sdk >= 3.12.0
 	gqlclient == 0.9.6
-	talus == 0.2.0
+	talus == 0.2.1
 	redis == 4.3.4
 	object-clerk == 0.1.0
 	requests >= 2.23
 	scipy >= 1.6.3
 	sunpy >= 3.0.0
 	pillow >= 8.3.0
 	moviepy >= 1.0.3
 	matplotlib >= 3.4
 	pydantic >= 1.8.1
 	retry >= 0.9.2
+	dkist-spectral-lines
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-xdist
 	pytest-cov
 	pytest-mock
```

