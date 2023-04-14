# Comparing `tmp/jobbergate-api-3.5.0a0.tar.gz` & `tmp/jobbergate-api-3.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate-api-3.5.0a0.tar", max compression
+gzip compressed data, was "jobbergate-api-3.5.0a1.tar", max compression
```

## Comparing `jobbergate-api-3.5.0a0.tar` & `jobbergate-api-3.5.0a1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1082 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/LICENSE
--rw-r--r--   0        0        0      738 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/README.rst
--rw-r--r--   0        0        0      169 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       41 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/__init__.py
--rw-r--r--   0        0        0     5655 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/application_files.py
--rw-r--r--   0        0        0      234 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/constants.py
--rw-r--r--   0        0        0     9408 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/file_validation.py
--rw-r--r--   0        0        0     1404 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/models.py
--rw-r--r--   0        0        0    12261 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/routers.py
--rw-r--r--   0        0        0     7239 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/schemas.py
--rw-r--r--   0        0        0       40 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0    12157 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_scripts/job_script_files.py
--rw-r--r--   0        0        0     1185 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    11073 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     3847 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0       44 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0      529 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     1910 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    12331 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/properties_parser.py
--rw-r--r--   0        0        0    17775 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0    14852 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0      554 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     3621 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/config.py
--rw-r--r--   0        0        0     2466 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     3268 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/main.py
--rw-r--r--   0        0        0     3433 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0       96 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/metadata.py
--rw-r--r--   0        0        0     3470 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/pagination.py
--rw-r--r--   0        0        0     2284 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/s3_manager.py
--rw-r--r--   0        0        0     2166 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/security.py
--rw-r--r--   0        0        0     5580 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/storage.py
--rw-r--r--   0        0        0       40 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/__init__.py
--rw-r--r--   0        0        0       44 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/applications/__init__.py
--rw-r--r--   0        0        0    10634 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/applications/test_application_files.py
--rw-r--r--   0        0        0     1967 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/applications/test_file_validation.py
--rw-r--r--   0        0        0    37966 2023-03-28 06:43:20.158277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/applications/test_routers.py
--rw-r--r--   0        0        0     5180 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/applications/test_schemas.py
--rw-r--r--   0        0        0     2756 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/conftest.py
--rw-r--r--   0        0        0       42 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     1376 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_scripts/conftest.py
--rw-r--r--   0        0        0    11518 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
--rw-r--r--   0        0        0    42583 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_scripts/test_routers.py
--rw-r--r--   0        0        0       46 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0    23970 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
--rw-r--r--   0        0        0    77917 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_submissions/test_routers.py
--rw-r--r--   0        0        0      511 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/test_main.py
--rw-r--r--   0        0        0     8900 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/conftest.py
--rw-r--r--   0        0        0     4503 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
--rw-r--r--   0        0        0     3215 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/test_config.py
--rw-r--r--   0        0        0     4974 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/test_email_notification.py
--rw-r--r--   0        0        0     3177 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/test_meta_mapper.py
--rw-r--r--   0        0        0     3959 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/test_pagination.py
--rw-r--r--   0        0        0     1146 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/test_s3_manager.py
--rw-r--r--   0        0        0     2718 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/test_security.py
--rw-r--r--   0        0        0     4512 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/test_storage.py
--rw-r--r--   0        0        0     2777 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/tests/test_version.py
--rw-r--r--   0        0        0     1102 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/jobbergate_api/version.py
--rw-r--r--   0        0        0     2904 2023-03-28 06:43:20.162277 jobbergate-api-3.5.0a0/pyproject.toml
--rw-r--r--   0        0        0     2488 2023-03-28 06:43:37.833988 jobbergate-api-3.5.0a0/setup.py
--rw-r--r--   0        0        0     2657 2023-03-28 06:43:37.834357 jobbergate-api-3.5.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/LICENSE
+-rw-r--r--   0        0        0      738 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/README.rst
+-rw-r--r--   0        0        0      169 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       41 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/__init__.py
+-rw-r--r--   0        0        0     5655 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/application_files.py
+-rw-r--r--   0        0        0      234 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/constants.py
+-rw-r--r--   0        0        0     9408 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/file_validation.py
+-rw-r--r--   0        0        0     1404 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/models.py
+-rw-r--r--   0        0        0    13548 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/routers.py
+-rw-r--r--   0        0        0     7239 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/schemas.py
+-rw-r--r--   0        0        0       40 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    12157 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/job_script_files.py
+-rw-r--r--   0        0        0     1185 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    11747 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     3890 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0       44 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     1910 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    12331 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/properties_parser.py
+-rw-r--r--   0        0        0    18431 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0    14894 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0      554 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     3621 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2466 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     3268 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3433 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0       96 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/metadata.py
+-rw-r--r--   0        0        0     3470 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/pagination.py
+-rw-r--r--   0        0        0     2284 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/s3_manager.py
+-rw-r--r--   0        0        0     2166 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/security.py
+-rw-r--r--   0        0        0     5580 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/storage.py
+-rw-r--r--   0        0        0       40 2023-04-14 17:46:36.120546 jobbergate-api-3.5.0a1/jobbergate_api/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/__init__.py
+-rw-r--r--   0        0        0    10634 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_application_files.py
+-rw-r--r--   0        0        0     1967 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_file_validation.py
+-rw-r--r--   0        0        0    41708 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_routers.py
+-rw-r--r--   0        0        0     5180 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_schemas.py
+-rw-r--r--   0        0        0     2756 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/conftest.py
+-rw-r--r--   0        0        0       42 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     1376 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/conftest.py
+-rw-r--r--   0        0        0    11518 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
+-rw-r--r--   0        0        0    42583 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/test_routers.py
+-rw-r--r--   0        0        0       46 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0    23970 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
+-rw-r--r--   0        0        0    78149 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/test_routers.py
+-rw-r--r--   0        0        0      511 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/test_main.py
+-rw-r--r--   0        0        0     8900 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/conftest.py
+-rw-r--r--   0        0        0     4503 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
+-rw-r--r--   0        0        0     3215 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_config.py
+-rw-r--r--   0        0        0     4974 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_email_notification.py
+-rw-r--r--   0        0        0     3177 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_meta_mapper.py
+-rw-r--r--   0        0        0     3959 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_pagination.py
+-rw-r--r--   0        0        0     1146 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_s3_manager.py
+-rw-r--r--   0        0        0     2718 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_security.py
+-rw-r--r--   0        0        0     4512 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_storage.py
+-rw-r--r--   0        0        0     2777 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/tests/test_version.py
+-rw-r--r--   0        0        0     1102 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/jobbergate_api/version.py
+-rw-r--r--   0        0        0     2904 2023-04-14 17:46:36.124546 jobbergate-api-3.5.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2488 2023-04-14 17:46:54.497939 jobbergate-api-3.5.0a1/setup.py
+-rw-r--r--   0        0        0     2657 2023-04-14 17:46:54.498371 jobbergate-api-3.5.0a1/PKG-INFO
```

### Comparing `jobbergate-api-3.5.0a0/LICENSE` & `jobbergate-api-3.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/README.rst` & `jobbergate-api-3.5.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/application_files.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/file_validation.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/models.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/routers.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/routers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Router for the Application resource.
 """
+from pathlib import PurePath
 from typing import List, Optional, Union
 
 from armasec import TokenPayload
 from fastapi import APIRouter, Depends, File, Header, HTTPException, Query
 from fastapi import Response as FastAPIResponse
 from fastapi import UploadFile, status
 from loguru import logger
@@ -74,17 +75,15 @@
     "/applications/{application_id}/upload",
     status_code=status.HTTP_201_CREATED,
     description="Endpoint for uploading application files.",
     dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
 )
 async def applications_upload(
     application_id: int = Query(..., description="id of the application for which to upload a file"),
-    upload_files: List[UploadFile] = File(
-        ..., media_type="text/plain", description="The application files to be uploaded"
-    ),
+    upload_files: List[UploadFile] = File(..., description="The application files to be uploaded"),
     content_length: int = Header(...),
 ):
     """
     Upload application files using an authenticated user token.
     """
     logger.debug(f"Preparing to receive upload files for {application_id=}")
 
@@ -104,14 +103,42 @@
         .values(dict(application_uploaded=True))
     )
 
     logger.trace(f"update_query = {render_sql(update_query)}")
     await database.execute(update_query)
 
 
+@router.patch(
+    "/applications/{application_id}/upload/individually",
+    status_code=status.HTTP_204_NO_CONTENT,
+    responses={204: {"description": "File(s) was(were) patched successfully"}},
+    dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
+)
+async def update_application_source_file(
+    application_id: int = Query(..., description="id of the application for which to upload a file"),
+    source_file: Union[UploadFile, None] = File(default=None),
+    config_file: Union[UploadFile, None] = File(default=None),
+    template_files: Union[List[UploadFile], None] = None,
+):
+    """Update the application files individually."""
+    # TODO: limit by file size
+    ApplicationFiles(
+        application_config=config_file.file.read().decode("utf-8") if config_file is not None else None,
+        application_source_file=source_file.file.read().decode("utf-8") if source_file is not None else None,
+        application_templates={
+            PurePath(template_file.filename).name: template_file.file.read().decode("utf-8")
+            for template_file in template_files
+        }
+        if template_files is not None
+        else {},
+    ).write_to_s3(application_id, remove_previous_files=False)
+
+    return FastAPIResponse(status_code=status.HTTP_204_NO_CONTENT)
+
+
 @router.delete(
     "/applications/{application_id}/upload",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint for deleting application files",
     dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
 )
 async def applications_delete_upload(
```

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/applications/schemas.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/applications/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/job_scripts/job_script_files.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/job_scripts/models.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/routers.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Router for the JobScript resource.
 """
 from typing import Optional
 
 from armasec import TokenPayload
 from fastapi import APIRouter, Depends, HTTPException, Query, status
 from loguru import logger
+from sqlalchemy import join, select
 
 from jobbergate_api.apps.applications.application_files import ApplicationFiles
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.applications.schemas import ApplicationResponse
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptCreationError, JobScriptFiles
 from jobbergate_api.apps.job_scripts.models import job_scripts_table, searchable_fields, sortable_fields
 from jobbergate_api.apps.job_scripts.schemas import (
@@ -112,14 +113,15 @@
             logger.error(f"Reverting database transaction: {str(e)}")
             raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e))
 
     logger.debug(f"Job-script created: {dict(job_script_data)}")
 
     response = JobScriptResponse(
         **job_script_data,
+        application_name=application.application_name,
         job_script_files=jobscript_files,
     )
     return response
 
 
 @router.get(
     "/job-scripts/{job_script_id}",
@@ -129,15 +131,25 @@
 )
 async def job_script_get(job_script_id: int = Query(...)):
     """
     Return the job_script given its id.
     """
     logger.debug(f"Getting {job_script_id=}")
 
-    query = job_scripts_table.select().where(job_scripts_table.c.id == job_script_id)
+    query = (
+        select([job_scripts_table, applications_table.c.application_name])
+        .select_from(
+            join(
+                job_scripts_table,
+                applications_table,
+                applications_table.columns.id == job_scripts_table.columns.application_id,
+            )
+        )
+        .where(job_scripts_table.c.id == job_script_id)
+    )
     logger.trace(f"get_query = {render_sql(query)}")
     job_script = await database.fetch_one(query)
 
     if not job_script:
         message = f"JobScript with id={job_script_id} not found."
         logger.warning(message)
         raise HTTPException(
@@ -187,26 +199,34 @@
 
        Use responses instead of response_model to skip a second round of validation and serialization. This
        is already happening in the ``package_response`` method. So, we uses ``responses`` so that FastAPI
        can generate the correct OpenAPI spec but not post-process the response.
     """
     logger.debug("Preparing to list job-scripts")
 
-    query = job_scripts_table.select()
+    query = select([job_scripts_table, applications_table.c.application_name]).select_from(
+        join(
+            job_scripts_table,
+            applications_table,
+            applications_table.c.id == job_scripts_table.c.application_id,
+        )
+    )
     identity_claims = IdentityClaims.from_token_payload(token_payload)
     if not all:
         query = query.where(job_scripts_table.c.job_script_owner_email == identity_claims.email)
     if from_application_id is not None:
         query = query.where(job_scripts_table.c.application_id == from_application_id)
     if search is not None:
         query = query.where(search_clause(search, searchable_fields))
     if sort_field is not None:
         query = query.order_by(sort_clause(sort_field, sortable_fields, sort_ascending))
+    else:
+        query = query.order_by(job_scripts_table.c.id.asc())
 
-    logger.trace(f"Query = {render_sql(query)}")
+    logger.debug(f"Query = {render_sql(query)}")
     return await package_response(JobScriptPartialResponse, query, pagination)
 
 
 @router.delete(
     "/job-scripts/{job_script_id}",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete job script",
```

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     id: Optional[int] = None
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
     job_script_name: str
     job_script_description: Optional[str] = None
     job_script_owner_email: str
     application_id: int
+    application_name: Optional[str] = None
 
     class Config:
         orm_mode = True
         schema_extra = job_script_meta_mapper
 
 
 class JobScriptResponse(JobScriptPartialResponse):
```

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/models.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/properties_parser.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Router for the JobSubmission resource.
 """
 from typing import Any, Dict, List, Optional
 
 from armasec import TokenPayload
 from fastapi import APIRouter, Body, Depends, HTTPException, Query, status
 from loguru import logger
-from sqlalchemy import select
+from sqlalchemy import join, select
 
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptFiles
 from jobbergate_api.apps.job_scripts.models import job_scripts_table
 from jobbergate_api.apps.job_submissions.constants import JobSubmissionStatus
 from jobbergate_api.apps.job_submissions.models import (
     job_submissions_table,
@@ -111,30 +111,42 @@
 
         except INTEGRITY_CHECK_EXCEPTIONS as e:
             logger.error(f"Reverting database transaction: {str(e)}")
             raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e))
 
     logger.debug(f"Job-submission created: {job_submission_data=}")
 
-    return JobSubmissionResponse(**job_submission_data)  # type: ignore
+    return JobSubmissionResponse(
+        **job_submission_data, job_script_name=raw_job_script.get("job_script_name")  # type: ignore
+    )
 
 
 @router.get(
     "/job-submissions/{job_submission_id}",
     description="Endpoint to get a job_submission",
     response_model=JobSubmissionResponse,
     dependencies=[Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_VIEW))],
 )
 async def job_submission_get(job_submission_id: int = Query(...)):
     """
     Return the job_submission given it's id.
     """
     logger.debug(f"Getting {job_submission_id=}")
 
-    query = job_submissions_table.select().where(job_submissions_table.c.id == job_submission_id)
+    query = (
+        select([job_submissions_table, job_scripts_table.c.job_script_name])
+        .select_from(
+            join(
+                job_submissions_table,
+                job_scripts_table,
+                job_submissions_table.c.job_script_id == job_scripts_table.c.id,
+            )
+        )
+        .where(job_submissions_table.c.id == job_submission_id)
+    )
     logger.trace(f"query = {render_sql(query)}")
     job_submission_data = await database.fetch_one(query)
 
     if not job_submission_data:
         message = f"JobSubmission with id={job_submission_id} not found."
         logger.warning(message)
         raise HTTPException(
@@ -177,15 +189,21 @@
 ):
     """
     List job_submissions for the authenticated user.
     """
     logger.debug("Fetching job submissions")
     identity_claims = IdentityClaims.from_token_payload(token_payload)
     logger.debug(f"Extracted identity claims from token: {identity_claims}")
-    query = job_submissions_table.select()
+    query = select([job_submissions_table, job_scripts_table.c.job_script_name]).select_from(
+        join(
+            job_submissions_table,
+            job_scripts_table,
+            job_submissions_table.c.job_script_id == job_scripts_table.c.id,
+        )
+    )
 
     logger.debug("Building query")
     if submit_status:
         query = query.where(job_submissions_table.c.status == submit_status)
 
     if not all:
         query = query.where(job_submissions_table.c.job_submission_owner_email == identity_claims.email)
@@ -201,14 +219,16 @@
                 detail="Invalid slurm_job_ids param. Must be a comma-separated list of integers",
             )
         query = query.where(job_submissions_table.c.slurm_job_id.in_(job_ids))
     if search is not None:
         query = query.where(search_clause(search, searchable_fields))
     if sort_field is not None:
         query = query.order_by(sort_clause(sort_field, sortable_fields, sort_ascending))
+    else:
+        query = query.order_by(job_submissions_table.c.id.asc())
 
     logger.trace(f"Query built as: {render_sql(query)}")
 
     logger.debug("Awaiting query and response package")
     response = await package_response(JobSubmissionResponse, query, pagination)
     logger.debug(f"Response built as: {response}")
     return response
```

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,14 +319,15 @@
     job_script_id: int
     execution_directory: Optional[Path]
     slurm_job_id: Optional[int]
     client_id: Optional[str]
     status: JobSubmissionStatus
     report_message: Optional[str]
     execution_parameters: Optional[JobProperties]
+    job_script_name: Optional[str] = None
 
     class Config:
         orm_mode = True
         schema_extra = job_submission_meta_mapper
 
 
 class PendingJobSubmission(BaseModel, extra=Extra.ignore):
```

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/apps/permissions.py` & `jobbergate-api-3.5.0a1/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/config.py` & `jobbergate-api-3.5.0a1/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/email_notification.py` & `jobbergate-api-3.5.0a1/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/main.py` & `jobbergate-api-3.5.0a1/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/meta_mapper.py` & `jobbergate-api-3.5.0a1/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/pagination.py` & `jobbergate-api-3.5.0a1/jobbergate_api/pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/s3_manager.py` & `jobbergate-api-3.5.0a1/jobbergate_api/s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/security.py` & `jobbergate-api-3.5.0a1/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/storage.py` & `jobbergate-api-3.5.0a1/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/applications/test_application_files.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/applications/test_file_validation.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/applications/test_routers.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_routers.py`

 * *Files 3% similar despite different names*

```diff
@@ -939,14 +939,118 @@
 
     application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
     assert application.application_uploaded
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.write_to_s3")
+async def test_upload_file_individually(
+    mocked_application_writer,
+    client,
+    inject_security_header,
+    fill_application_data,
+    tweak_settings,
+    make_dummy_file,
+    dummy_application_config,
+    dummy_template,
+    dummy_application_source_file,
+    make_files_param,
+):
+    """
+    Test that the application files can be patched individually.
+
+    This test proves that any application file, i.e. config, source or template,
+    can be patched individually.
+    """
+    inserted_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
+    assert not application.application_uploaded
+
+    dummy_config_file = make_dummy_file("jobbergate.yaml", content=dummy_application_config)
+    dummy_source_file = make_dummy_file("jobbergate.py", content=dummy_application_source_file)
+    dummy_template_file = make_dummy_file("jobbergate.yaml", content=dummy_template)
+
+    inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
+
+    # test upload only the source file
+    response = await client.patch(
+        f"/jobbergate/applications/{inserted_id}/upload/individually",
+        files={"source_file": open(dummy_source_file, "rb")},
+    )
+
+    assert response.status_code == status.HTTP_204_NO_CONTENT
+
+    # test upload only the config file
+    response = await client.patch(
+        f"/jobbergate/applications/{inserted_id}/upload/individually",
+        files={"config_file": open(dummy_config_file, "rb")},
+    )
+
+    assert response.status_code == status.HTTP_204_NO_CONTENT
+
+    # test upload only the template file
+    response = await client.patch(
+        f"/jobbergate/applications/{inserted_id}/upload/individually",
+        files={"template_file": open(dummy_template_file, "rb")},
+    )
+
+    assert response.status_code == status.HTTP_204_NO_CONTENT
+
+    # test upload the source file and the template file
+    response = await client.patch(
+        f"/jobbergate/applications/{inserted_id}/upload/individually",
+        files={
+            "source_file": open(dummy_source_file, "rb"),
+            "template_file": open(dummy_template_file, "rb"),
+        },
+    )
+
+    assert response.status_code == status.HTTP_204_NO_CONTENT
+
+    # test upload the source file and the config file
+    response = await client.patch(
+        f"/jobbergate/applications/{inserted_id}/upload/individually",
+        files={"source_file": open(dummy_source_file, "rb"), "config_file": open(dummy_config_file, "rb")},
+    )
+
+    assert response.status_code == status.HTTP_204_NO_CONTENT
+
+    # test upload the config file and the template file
+    response = await client.patch(
+        f"/jobbergate/applications/{inserted_id}/upload/individually",
+        files={
+            "template_file": open(dummy_template_file, "rb"),
+            "config_file": open(dummy_config_file, "rb"),
+        },
+    )
+
+    assert response.status_code == status.HTTP_204_NO_CONTENT
+
+    # test upload all files
+    response = await client.patch(
+        f"/jobbergate/applications/{inserted_id}/upload/individually",
+        files={
+            "template_file": open(dummy_template_file, "rb"),
+            "source_file": open(dummy_source_file, "rb"),
+            "config_file": open(dummy_config_file, "rb"),
+        },
+    )
+
+    assert response.status_code == status.HTTP_204_NO_CONTENT
+
+    mocked_application_writer.assert_has_calls(
+        [mock.call(inserted_id, remove_previous_files=False) for _ in range(7)]
+    )
+
+
+@pytest.mark.asyncio
+@mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.write_to_s3")
 async def test_upload_file__fails_with_413_on_large_file(
     mocked_application_writer,
     client,
     inject_security_header,
     tweak_settings,
     make_dummy_file,
     make_files_param,
```

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/applications/test_schemas.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/applications/test_schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/conftest.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_scripts/conftest.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_scripts/test_routers.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_scripts/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/apps/job_submissions/test_routers.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/apps/job_submissions/test_routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission__with_client_id_in_token(
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
+    job_script_data,
     client,
     inject_security_header,
     time_frame,
 ):
     """
     Test POST /job-submissions/ correctly creates a job_submission.
 
@@ -84,15 +85,17 @@
     job_submission = JobSubmissionResponse(**response.json())
 
     # Check that the response correspond to the entry in the database
     job_submission_raw_data = await database.fetch_one(
         query=job_submissions_table.select().where(job_submissions_table.c.id == id_rows[0][0])
     )
     assert job_submission_raw_data is not None
-    assert job_submission == JobSubmissionResponse(**job_submission_raw_data)  # type: ignore
+    assert job_submission == JobSubmissionResponse(
+        **{**job_submission_raw_data, **job_script_data}
+    )  # type: ignore
 
     # Check that each field is correctly set
     assert job_submission.id == job_submission_raw_data.get("id")
     assert job_submission.job_submission_name == "sub1"
     assert job_submission.job_submission_owner_email == "owner1@org.com"
     assert job_submission.job_submission_description is None
     assert job_submission.job_script_id == inserted_job_script_id
@@ -108,14 +111,15 @@
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission__without_execution_parameters(
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
+    job_script_data,
     client,
     inject_security_header,
     time_frame,
 ):
     """
     Test POST /job-submissions/ correctly creates a job_submission.
 
@@ -174,15 +178,17 @@
     job_submission = JobSubmissionResponse(**response.json())
 
     # Check that the response correspond to the entry in the database
     job_submission_raw_data = await database.fetch_one(
         query=job_submissions_table.select().where(job_submissions_table.c.id == id_rows[0][0])
     )
     assert job_submission_raw_data is not None
-    assert job_submission == JobSubmissionResponse(**job_submission_raw_data)  # type: ignore
+    assert job_submission == JobSubmissionResponse(
+        **{**job_submission_raw_data, **job_script_data}
+    )  # type: ignore
 
     # Check that each field is correctly set
     assert job_submission.id == job_submission_raw_data.get("id")
     assert job_submission.job_submission_name == create_data.get("job_submission_name")
     assert job_submission.job_submission_owner_email == create_data.get("job_submission_owner_email")
     assert job_submission.job_submission_description == create_data.get("job_submission_description")
     assert job_submission.job_script_id == create_data.get("job_script_id")
@@ -200,14 +206,15 @@
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission__with_client_id_in_request_body(
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
+    job_script_data,
     client,
     inject_security_header,
     time_frame,
 ):
     """
     Test POST /job-submissions/ correctly creates a job_submission.
 
@@ -263,15 +270,17 @@
     job_submission = JobSubmissionResponse(**response.json())
 
     # Check that the response correspond to the entry in the database
     job_submission_raw_data = await database.fetch_one(
         query=job_submissions_table.select().where(job_submissions_table.c.id == id_rows[0][0])
     )
     assert job_submission_raw_data is not None
-    assert job_submission == JobSubmissionResponse(**job_submission_raw_data)  # type: ignore
+    assert job_submission == JobSubmissionResponse(
+        **{**job_submission_raw_data, **job_script_data}
+    )  # type: ignore
 
     # Check that each field is correctly set
     assert job_submission.id == job_submission_raw_data.get("id")
     assert job_submission.job_submission_name == "sub1"
     assert job_submission.job_submission_owner_email == "owner1@org.com"
     assert job_submission.job_submission_description is None
     assert job_submission.job_script_id == inserted_job_script_id
@@ -286,14 +295,15 @@
 
 
 @pytest.mark.asyncio
 async def test_create_job_submission__with_execution_directory(
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
+    job_script_data,
     client,
     inject_security_header,
     time_frame,
 ):
     """
     Test POST /job-submissions/ correctly creates a job_submission with an execution directory.
 
@@ -349,15 +359,17 @@
     job_submission = JobSubmissionResponse(**response.json())
 
     # Check that the response correspond to the entry in the database
     job_submission_raw_data = await database.fetch_one(
         query=job_submissions_table.select().where(job_submissions_table.c.id == id_rows[0][0])
     )
     assert job_submission_raw_data is not None
-    assert job_submission == JobSubmissionResponse(**job_submission_raw_data)  # type: ignore
+    assert job_submission == JobSubmissionResponse(
+        **{**job_submission_raw_data, **job_script_data}
+    )  # type: ignore
 
     assert job_submission.id == job_submission_raw_data.get("id")
     assert job_submission.job_submission_name == "sub1"
     assert job_submission.job_submission_owner_email == "owner1@org.com"
     assert job_submission.job_submission_description is None
     assert job_submission.job_script_id == inserted_job_script_id
     assert job_submission.execution_directory == pathlib.Path("/some/fake/path")
```

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/conftest.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/test_config.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/test_email_notification.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/test_meta_mapper.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/test_pagination.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/test_s3_manager.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/test_security.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/test_storage.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/tests/test_version.py` & `jobbergate-api-3.5.0a1/jobbergate_api/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/jobbergate_api/version.py` & `jobbergate-api-3.5.0a1/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate-api-3.5.0a0/pyproject.toml` & `jobbergate-api-3.5.0a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "3.5.0-alpha.0"
+version = "3.5.0-alpha.1"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate-api-3.5.0a0/setup.py` & `jobbergate-api-3.5.0a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
  'yarl>=1.7.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['dev-tools = dev_tools:app']}
 
 setup_kwargs = {
     'name': 'jobbergate-api',
-    'version': '3.5.0a0',
+    'version': '3.5.0a1',
     'description': 'Jobbergate API',
     'long_description': '================\n Jobbergate API\n================\n\n\nThe Jobbergate API provides a RESTful interface over the Jobbergate data and is used\nby both the ``jobbergate-agent`` and the ``jobbergate-cli`` to view and manage the\nJobbergate resources.\n\nJobbergate API is a Python project implemented with\n`FastAPI <https://fastapi.tiangolo.com/>`_. Its dependencies and environment are\nmanaged by `Poetry <https://python-poetry.org/>`_.\n\nIt integrates with an OIDC server to provide identity and auth for its endpoints.\n\nSee also:\n\n* `jobbergate-cli <https://github.com/omnivector-solutions/jobbergate/jobbergate-cli>`_\n\nLicense\n-------\n* `MIT <LICENSE>`_\n\n\nCopyright\n---------\n* Copyright (c) 2020 OmniVector Solutions <info@omnivector.solutions>\n',
     'author': 'Omnivector Solutions',
     'author_email': 'info@omnivector.solutions',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/omnivector-solutions/jobbergate',
```

### Comparing `jobbergate-api-3.5.0a0/PKG-INFO` & `jobbergate-api-3.5.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 3.5.0a0
+Version: 3.5.0a1
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

