# Comparing `tmp/resc_backend-1.1.0.tar.gz` & `tmp/resc_backend-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-1.1.0.tar", last modified: Thu Mar  9 12:54:28 2023, max compression
+gzip compressed data, was "resc_backend-1.2.0.tar", last modified: Fri Apr 14 15:10:27 2023, max compression
```

## Comparing `resc_backend-1.1.0.tar` & `resc_backend-1.2.0.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.256124 resc_backend-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-03-09 12:54:28.256124 resc_backend-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-09 12:54:28.256124 resc_backend-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-09 12:54:21.000000 resc_backend-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.236124 resc_backend-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.236124 resc_backend-1.1.0/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.240124 resc_backend-1.1.0/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.240124 resc_backend-1.1.0/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.244124 resc_backend-1.1.0/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.244124 resc_backend-1.1.0/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/helpers/git_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.244124 resc_backend-1.1.0/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.248124 resc_backend-1.1.0/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.248124 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24796 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    20091 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.252124 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.252124 resc_backend-1.1.0/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/helpers/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.256124 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.256124 resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-09 12:54:21.000000 resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 12:54:28.240124 resc_backend-1.1.0/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-03-09 12:54:28.000000 resc_backend-1.1.0/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-03-09 12:54:28.000000 resc_backend-1.1.0/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 12:54:28.000000 resc_backend-1.1.0/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-09 12:54:28.000000 resc_backend-1.1.0/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 12:54:28.000000 resc_backend-1.1.0/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-09 12:54:28.000000 resc_backend-1.1.0/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-09 12:54:28.000000 resc_backend-1.1.0/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.245564 resc_backend-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-14 15:10:27.245564 resc_backend-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-14 15:10:27.245564 resc_backend-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 15:10:23.000000 resc_backend-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.233563 resc_backend-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.233563 resc_backend-1.2.0/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/git_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.241563 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.241563 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17644 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.241563 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.245564 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.245564 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-1.1.0/PKG-INFO` & `resc_backend-1.2.0/src/resc_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resc_backend
-Version: 1.1.0
+Name: resc-backend
+Version: 1.2.0
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -176,15 +176,15 @@
 ```
 
 If you can override the images by providing below arguments to the script.
 ```bash
 cd tests/newman_tests
 ./run_newman_tests.sh -b <resc-backend image:tag> -d <resc-database image:tag>  -n <newman image:tag> 
 
-Example: ./run_integration_tests.sh -b 'rescabnamro/resc-backend:1.0.1' -d 'mcr.microsoft.com/azure-sql-edge:1.0.5' -n 'postman/newman:5.3.1-alpine'
+Example: ./run_newman_tests.sh -b 'rescabnamro/resc-backend:1.0.1' -d 'mcr.microsoft.com/azure-sql-edge:1.0.5' -n 'postman/newman:5.3.1-alpine'
 ```
 
 
 
 ## Create a migration for database changes
 [(Back to top)](#table-of-contents)
```

### Comparing `resc_backend-1.1.0/setup.cfg` & `resc_backend-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_backend
 description = Repository Scanner - Backend
-version = 1.1.0
+version = 1.2.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_backend-1.1.0/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-1.2.0/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/common.py` & `resc_backend-1.2.0/src/resc_backend/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/constants.py` & `resc_backend-1.2.0/src/resc_backend/constants.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/db/connection.py` & `resc_backend-1.2.0/src/resc_backend/db/connection.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/db/model/__init__.py` & `resc_backend-1.2.0/src/resc_backend/db/model/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Base = declarative_base()
 basedir = os.path.abspath(os.path.dirname(__file__))
 logger = logging.getLogger(__name__)
 
 
 # First Party
+from resc_backend.db.model.audit import DBaudit
 from resc_backend.db.model.branch import DBbranch
 from resc_backend.db.model.finding import DBfinding
 from resc_backend.db.model.repository import DBrepository
 from resc_backend.db.model.rule import DBrule
 from resc_backend.db.model.rule_allow_list import DBruleAllowList
 from resc_backend.db.model.rule_pack import DBrulePack
 from resc_backend.db.model.scan import DBscan
```

### Comparing `resc_backend-1.1.0/src/resc_backend/db/model/branch.py` & `resc_backend-1.2.0/src/resc_backend/db/model/branch.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/db/model/finding.py` & `resc_backend-1.2.0/src/resc_backend/db/model/finding.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # pylint: disable=R0902
 # Standard Library
-import html
 from datetime import datetime
 
 # Third Party
-from sqlalchemy import Column, DateTime, Enum, ForeignKey, Integer, String, Text, UniqueConstraint
+from sqlalchemy import Column, DateTime, ForeignKey, Integer, String, Text, UniqueConstraint
 
 # First Party
 from resc_backend.db.model import Base
-from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 
 
 class DBfinding(Base):
     __tablename__ = "finding"
     id_ = Column("id", Integer, primary_key=True)
     branch_id = Column(Integer, ForeignKey("branch.id"), nullable=False)
     rule_name = Column(String(400), nullable=False)
@@ -21,52 +19,44 @@
     column_start = Column(Integer, nullable=False, default=0)
     column_end = Column(Integer, nullable=False, default=0)
     commit_id = Column(String(120))
     commit_message = Column(Text)
     commit_timestamp = Column(DateTime, default=datetime.utcnow().isoformat())
     author = Column(String(200))
     email = Column(String(100))
-    status = Column(Enum(FindingStatus), default=FindingStatus.NOT_ANALYZED, server_default="NOT_ANALYZED",
-                    nullable=False)
-    comment = Column(String(255), nullable=True)
     event_sent_on = Column(DateTime, nullable=True)
 
     __table_args__ = (UniqueConstraint("commit_id", "branch_id", "rule_name", "file_path", "line_number",
                                        "column_start", "column_end", name="uc_finding_per_branch"),)
 
     def __init__(self, rule_name, file_path, line_number, commit_id, commit_message, commit_timestamp, author,
-                 email, status, comment, event_sent_on, branch_id, column_start, column_end):
+                 email, event_sent_on, branch_id, column_start, column_end):
         self.email = email
         self.author = author
         self.commit_timestamp = commit_timestamp
         self.commit_message = commit_message
         self.commit_id = commit_id
         self.line_number = line_number
         self.file_path = file_path
         self.rule_name = rule_name
-        self.status = status
-        self.comment = comment
         self.event_sent_on = event_sent_on
         self.branch_id = branch_id
         self.column_start = column_start
         self.column_end = column_end
 
     @staticmethod
     def create_from_finding(finding):
-        sanitized_comment = html.escape(finding.comment) if finding.comment else finding.comment
         db_finding = DBfinding(
             rule_name=finding.rule_name,
             file_path=finding.file_path,
             line_number=finding.line_number,
             email=finding.email,
             commit_id=finding.commit_id,
             commit_message=finding.commit_message,
             commit_timestamp=finding.commit_timestamp,
             author=finding.author,
-            status=finding.status,
-            comment=sanitized_comment,
             event_sent_on=finding.event_sent_on,
             branch_id=finding.branch_id,
             column_start=finding.column_start,
             column_end=finding.column_end
         )
         return db_finding
```

### Comparing `resc_backend-1.1.0/src/resc_backend/db/model/repository.py` & `resc_backend-1.2.0/src/resc_backend/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/db/model/rule.py` & `resc_backend-1.2.0/src/resc_backend/db/model/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-1.2.0/src/resc_backend/db/model/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/db/model/rule_pack.py` & `resc_backend-1.2.0/src/resc_backend/db/model/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/db/model/scan.py` & `resc_backend-1.2.0/src/resc_backend/db/model/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/db/model/vcs_instance.py` & `resc_backend-1.2.0/src/resc_backend/db/model/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-1.2.0/src/resc_backend/helpers/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-1.2.0/src/resc_backend/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/helpers/git_operation.py` & `resc_backend-1.2.0/src/resc_backend/helpers/git_operation.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/api.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/api.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/branch.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/branch.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/detailed_finding.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/detailed_finding.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# pylint: disable=R0912
+# pylint: disable=R0912,C0121
 # Standard Library
 from typing import List
 
 # Third Party
-from sqlalchemy import and_, func
+from sqlalchemy import and_, func, or_
 from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
 from resc_backend.db import model
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.schema import detailed_finding as detailed_finding_schema
+from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 
 
 def get_detailed_findings(db_connection: Session, findings_filter: FindingsFilter, skip: int = 0,
                           limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT
                           ) -> List[detailed_finding_schema.DetailedFindingRead]:
     """
     Retrieve all detailed findings objects matching the provided FindingsFilter
@@ -32,36 +33,41 @@
         or an empty list if no finding was found for the given findings_filter
     """
     max_scan_subquery = db_connection.query(model.DBscanFinding.finding_id,
                                             func.max(model.DBscanFinding.scan_id).label("scan_id"))
 
     if findings_filter.rule_pack_versions:
         max_scan_subquery = max_scan_subquery.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id) \
-                .filter(model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
+            .filter(model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
 
     if findings_filter.scan_ids:
         max_scan_subquery = max_scan_subquery.filter(model.DBscanFinding.scan_id.in_(findings_filter.scan_ids))
 
     max_scan_subquery = max_scan_subquery.group_by(model.DBscanFinding.finding_id).subquery()
 
+    # subquery to select latest audit ids of findings
+    max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
+                                             func.max(model.DBaudit.id_).label("audit_id")) \
+        .group_by(model.DBaudit.finding_id).subquery()
+
     limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
     scan_id = model.DBscan.id_.label("scan_id")
     query = db_connection.query(
         model.DBfinding.id_,
         model.DBfinding.file_path,
         model.DBfinding.line_number,
         model.DBfinding.column_start,
         model.DBfinding.column_end,
         model.DBfinding.commit_id,
         model.DBfinding.commit_message,
         model.DBfinding.commit_timestamp,
         model.DBfinding.author,
         model.DBfinding.email,
-        model.DBfinding.status,
-        model.DBfinding.comment,
+        model.DBaudit.status,
+        model.DBaudit.comment,
         model.DBfinding.rule_name,
         model.DBscan.rule_pack,
         model.DBfinding.event_sent_on,
         model.DBscan.timestamp,
         scan_id,
         model.DBbranch.branch_name,
         model.DBscan.last_scanned_commit,
@@ -73,15 +79,19 @@
         .join(model.DBscan,
               model.scan.DBscan.id_ == max_scan_subquery.c.scan_id) \
         .join(model.DBbranch,
               model.branch.DBbranch.id_ == model.finding.DBfinding.branch_id) \
         .join(model.DBrepository,
               model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
         .join(model.DBVcsInstance,
-              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
+              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance) \
+        .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+              isouter=True) \
+        .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+              isouter=True)
 
     if findings_filter.rule_tags:
         query = query.join(model.DBrule, and_(model.DBrule.rule_name == model.DBfinding.rule_name,
                                               model.DBrule.rule_pack == model.DBscan.rule_pack))
         for tag in findings_filter.rule_tags:
             query = query.filter(model.DBrule.tags.like(f"%{tag}%"))
 
@@ -103,15 +113,19 @@
     if findings_filter.vcs_providers and findings_filter.vcs_providers is not None:
         query = query.filter(model.vcs_instance.DBVcsInstance.provider_type.in_(findings_filter.vcs_providers))
     if findings_filter.project_name:
         query = query.filter(model.repository.DBrepository.project_key == findings_filter.project_name)
     if findings_filter.rule_names:
         query = query.filter(model.DBfinding.rule_name.in_(findings_filter.rule_names))
     if findings_filter.finding_statuses:
-        query = query.filter(model.finding.DBfinding.status.in_(findings_filter.finding_statuses))
+        if FindingStatus.NOT_ANALYZED in findings_filter.finding_statuses:
+            query = query.filter(or_(model.DBaudit.status.in_(findings_filter.finding_statuses),
+                                     model.DBaudit.status == None))  # noqa: E711
+        else:
+            query = query.filter(model.DBaudit.status.in_(findings_filter.finding_statuses))
 
     query = query.order_by(model.finding.DBfinding.id_)
     findings: List[detailed_finding_schema.DetailedFindingRead] = query.offset(skip).limit(limit_val).all()
 
     return findings
 
 
@@ -125,14 +139,19 @@
         Session of the database connection
     :return: total_count
         count of findings
     """
     max_scan_subquery = db_connection.query(model.DBscanFinding.finding_id,
                                             func.max(model.DBscanFinding.scan_id).label("scan_id"))
 
+    # subquery to select latest audit ids of findings
+    max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
+                                             func.max(model.DBaudit.id_).label("audit_id")) \
+        .group_by(model.DBaudit.finding_id).subquery()
+
     if findings_filter.rule_pack_versions:
         max_scan_subquery = max_scan_subquery.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id) \
             .filter(model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
 
     if findings_filter.scan_ids:
         max_scan_subquery = max_scan_subquery.filter(model.DBscanFinding.scan_id.in_(findings_filter.scan_ids))
 
@@ -143,15 +162,19 @@
         .join(model.DBscan,
               model.scan.DBscan.id_ == max_scan_subquery.c.scan_id) \
         .join(model.DBbranch,
               model.branch.DBbranch.id_ == model.finding.DBfinding.branch_id) \
         .join(model.DBrepository,
               model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
         .join(model.DBVcsInstance,
-              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
+              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance) \
+        .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+              isouter=True) \
+        .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+              isouter=True)
 
     if findings_filter.rule_tags:
         query = query.join(model.DBrule, and_(model.DBrule.rule_name == model.DBfinding.rule_name,
                                               model.DBrule.rule_pack == model.DBscan.rule_pack))
         for tag in findings_filter.rule_tags:
             query = query.filter(model.DBrule.tags.like(f"%{tag}%"))
 
@@ -173,15 +196,19 @@
     if findings_filter.vcs_providers and findings_filter.vcs_providers is not None:
         query = query.filter(model.vcs_instance.DBVcsInstance.provider_type.in_(findings_filter.vcs_providers))
     if findings_filter.project_name:
         query = query.filter(model.repository.DBrepository.project_key == findings_filter.project_name)
     if findings_filter.rule_names:
         query = query.filter(model.DBfinding.rule_name.in_(findings_filter.rule_names))
     if findings_filter.finding_statuses:
-        query = query.filter(model.finding.DBfinding.status.in_(findings_filter.finding_statuses))
+        if FindingStatus.NOT_ANALYZED in findings_filter.finding_statuses:
+            query = query.filter(or_(model.DBaudit.status.in_(findings_filter.finding_statuses),
+                                     model.DBaudit.status == None))  # noqa: E711
+        else:
+            query = query.filter(model.DBaudit.status.in_(findings_filter.finding_statuses))
 
     findings_count = query.scalar()
     return findings_count
 
 
 def get_detailed_finding(db_connection: Session, finding_id: int) -> detailed_finding_schema.DetailedFindingRead:
     """
@@ -194,28 +221,33 @@
         The output will contain an object of type DetailedFindingRead,
             or a null object finding was found for the given finding_id
     """
     max_scan_subquery = db_connection.query(model.DBscanFinding.finding_id,
                                             func.max(model.DBscanFinding.scan_id).label("scan_id"))
     max_scan_subquery = max_scan_subquery.group_by(model.DBscanFinding.finding_id).subquery()
 
+    # subquery to select latest audit ids of findings
+    max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
+                                             func.max(model.DBaudit.id_).label("audit_id")) \
+        .group_by(model.DBaudit.finding_id).subquery()
+
     scan_id = model.DBscan.id_.label("scan_id")
-    finding = db_connection.query(
+    query = db_connection.query(
         model.DBfinding.id_,
         model.DBfinding.file_path,
         model.DBfinding.line_number,
         model.DBfinding.column_start,
         model.DBfinding.column_end,
         model.DBfinding.commit_id,
         model.DBfinding.commit_message,
         model.DBfinding.commit_timestamp,
         model.DBfinding.author,
         model.DBfinding.email,
-        model.DBfinding.status,
-        model.DBfinding.comment,
+        model.DBaudit.status,
+        model.DBaudit.comment,
         model.DBfinding.rule_name,
         model.DBscan.rule_pack,
         model.DBscan.timestamp,
         scan_id,
         model.DBbranch.branch_name,
         model.DBscan.last_scanned_commit,
         model.DBVcsInstance.provider_type.label("vcs_provider"),
@@ -226,11 +258,15 @@
         .join(model.DBscan,
               model.scan.DBscan.id_ == max_scan_subquery.c.scan_id) \
         .join(model.DBbranch,
               model.branch.DBbranch.id_ == model.scan.DBscan.branch_id) \
         .join(model.DBrepository,
               model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
         .join(model.DBVcsInstance,
-              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)\
-        .filter(model.finding.DBfinding.id_ == finding_id).first()
-
+              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance) \
+        .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+              isouter=True) \
+        .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+              isouter=True) \
+        .filter(model.finding.DBfinding.id_ == finding_id)
+    finding = query.first()
     return finding
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,43 @@
-# pylint: disable=R0916,R0912
+# pylint: disable=R0916,R0912,C0121
 # Standard Library
-import html
 import logging
 from datetime import datetime
 from typing import List
 
 # Third Party
-from sqlalchemy import and_, extract, func
+from sqlalchemy import and_, extract, func, or_
 from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
 from resc_backend.db import model
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.schema import finding as finding_schema
 from resc_backend.resc_web_service.schema.date_filter import DateFilter
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
+from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 logger = logging.getLogger(__name__)
 
 
-def update_finding(db_connection: Session, finding_id: int, finding: finding_schema.FindingUpdate):
-    sanitized_comment = html.escape(finding.comment) if finding.comment else finding.comment
-    db_finding = db_connection.query(model.DBfinding).filter_by(id_=finding_id).first()
-    db_finding.status = finding.status
-    db_finding.comment = sanitized_comment
-    db_connection.commit()
-    db_connection.refresh(db_finding)
-    return db_finding
-
-
 def patch_finding(db_connection: Session, finding_id: int, finding_update: finding_schema.FindingPatch):
     db_finding = db_connection.query(model.DBfinding).filter_by(id_=finding_id).first()
 
     finding_update_dict = finding_update.dict(exclude_unset=True)
     for key in finding_update_dict:
         setattr(db_finding, key, finding_update_dict[key])
 
     db_connection.commit()
     db_connection.refresh(db_finding)
     return db_finding
 
 
-def audit_finding(db_connection: Session, db_finding: finding_schema.FindingRead,
-                  status: FindingStatus, comment: str = "") -> model.DBfinding:
-    """
-        Audit finding, updating the status and comment
-    :param db_connection:
-        Session of the database connection
-    :param db_finding:
-        database finding object to update
-    :param status:
-        audit status to set, type FindingStatus
-    :param comment:
-        audit comment to set
-    :return: FindingRead
-        The output will contain the findings that was updated
-    """
-    sanitized_comment = html.escape(comment) if comment else comment
-    db_finding.status = status
-    db_finding.comment = sanitized_comment
-
-    db_connection.commit()
-    db_connection.refresh(db_finding)
-    return db_finding
-
-
 def create_findings(db_connection: Session, findings: List[finding_schema.FindingCreate]) -> List[model.DBfinding]:
     if len(findings) < 1:
         # Function is called with an empty list of findings
         return []
     branch_id = findings[0].branch_id
 
     # get a list of known / registered findings for this branch
@@ -152,22 +118,36 @@
         return []
     limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
 
     query = db_connection.query(model.DBfinding)
     query = query.join(model.DBscanFinding,
                        model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_)
 
+    if statuses_filter:
+        # subquery to select latest audit ids findings
+        max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
+                                                 func.max(model.DBaudit.id_).label("audit_id")) \
+            .group_by(model.DBaudit.finding_id).subquery()
+
+        query = query \
+            .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+                  isouter=True) \
+            .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+                  isouter=True)
+        if FindingStatus.NOT_ANALYZED in statuses_filter:
+            query = query.filter(or_(model.DBaudit.status.in_(statuses_filter),
+                                     model.DBaudit.status == None))  # noqa: E711
+        else:
+            query = query.filter(model.DBaudit.status.in_(statuses_filter))
+
     query = query.filter(model.DBscanFinding.scan_id.in_(scan_ids))
 
     if rules_filter:
         query = query.filter(model.DBfinding.rule_name.in_(rules_filter))
 
-    if statuses_filter:
-        query = query.filter(model.DBfinding.status.in_(statuses_filter))
-
     findings = query.order_by(model.finding.DBfinding.id_).offset(skip).limit(limit_val).all()
     return findings
 
 
 def get_total_findings_count(db_connection: Session, findings_filter: FindingsFilter = None) -> int:
     """
         Retrieve count of finding records of a given scan
@@ -176,14 +156,25 @@
         Session of the database connection
     :return: total_count
         count of findings
     """
 
     total_count_query = db_connection.query(func.count(model.DBfinding.id_))
     if findings_filter:
+        if findings_filter.finding_statuses:
+            # subquery to select latest audit ids findings
+            max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
+                                                     func.max(model.DBaudit.id_).label("audit_id")) \
+                .group_by(model.DBaudit.finding_id).subquery()
+
+            total_count_query = total_count_query \
+                .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+                      isouter=True) \
+                .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+                      isouter=True)
         if (findings_filter.vcs_providers and findings_filter.vcs_providers is not None) \
                 or findings_filter.project_name or findings_filter.branch_name \
                 or findings_filter.repository_name or findings_filter.start_date_time \
                 or findings_filter.end_date_time:
             total_count_query = total_count_query \
                 .join(model.DBscanFinding,
                       model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_) \
@@ -196,15 +187,15 @@
                 .join(model.DBVcsInstance,
                       model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
         elif findings_filter.rule_tags:
             max_scan_subquery = db_connection.query(model.DBscanFinding.finding_id,
                                                     func.max(model.DBscanFinding.scan_id).label("scan_id"))
             max_scan_subquery = max_scan_subquery.group_by(model.DBscanFinding.finding_id).subquery()
             total_count_query = total_count_query.join(max_scan_subquery,
-                                                       model.finding.DBfinding.id_ == max_scan_subquery.c.finding_id)\
+                                                       model.finding.DBfinding.id_ == max_scan_subquery.c.finding_id) \
                 .join(model.DBscan, model.scan.DBscan.id_ == max_scan_subquery.c.scan_id)
 
         if findings_filter.rule_tags:
             total_count_query = total_count_query.join(model.DBrule,
                                                        and_(model.DBrule.rule_name == model.DBfinding.rule_name,
                                                             model.DBrule.rule_pack == model.DBscan.rule_pack))
             for tag in findings_filter.rule_tags:
@@ -227,16 +218,20 @@
                 model.vcs_instance.DBVcsInstance.provider_type.in_(findings_filter.vcs_providers))
         if findings_filter.project_name:
             total_count_query = total_count_query.filter(
                 model.repository.DBrepository.project_key == findings_filter.project_name)
         if findings_filter.rule_names:
             total_count_query = total_count_query.filter(model.DBfinding.rule_name.in_(findings_filter.rule_names))
         if findings_filter.finding_statuses:
-            total_count_query = total_count_query.filter(
-                model.finding.DBfinding.status.in_(findings_filter.finding_statuses))
+            if FindingStatus.NOT_ANALYZED in findings_filter.finding_statuses:
+                total_count_query = total_count_query. \
+                    filter(or_(model.DBaudit.status.in_(findings_filter.finding_statuses),
+                               model.DBaudit.status == None))  # noqa: E711
+            else:
+                total_count_query = total_count_query.filter(model.DBaudit.status.in_(findings_filter.finding_statuses))
         if findings_filter.scan_ids and len(findings_filter.scan_ids) == 1:
             total_count_query = total_count_query.join(
                 model.DBscanFinding, model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_)
             total_count_query = total_count_query.filter(
                 model.scan_finding.DBscanFinding.scan_id == findings_filter.scan_ids[0])
 
         if findings_filter.scan_ids and len(findings_filter.scan_ids) >= 2:
@@ -301,22 +296,37 @@
                   model.scan.DBscan.id_ == model.scan_finding.DBscanFinding.scan_id) \
             .join(model.DBbranch,
                   model.branch.DBbranch.id_ == model.scan.DBscan.branch_id) \
             .join(model.DBrepository,
                   model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
             .join(model.DBVcsInstance,
                   model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
+    if finding_statuses:
+        # subquery to select latest audit ids findings
+        max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
+                                                 func.max(model.DBaudit.id_).label("audit_id")) \
+            .group_by(model.DBaudit.finding_id).subquery()
 
+        query = query \
+            .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+                  isouter=True) \
+            .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+                  isouter=True)
     if scan_id > 0:
         query = query.join(model.DBscanFinding,
                            model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_)
         query = query.filter(model.DBscanFinding.scan_id == scan_id)
     else:
         if finding_statuses:
-            query = query.filter(model.DBfinding.status.in_(finding_statuses))
+            if FindingStatus.NOT_ANALYZED in finding_statuses:
+                query = query. \
+                    filter(or_(model.DBaudit.status.in_(finding_statuses),
+                               model.DBaudit.status == None))  # noqa: E711
+            else:
+                query = query.filter(model.DBaudit.status.in_(finding_statuses))
 
         if vcs_providers:
             query = query.filter(model.DBVcsInstance.provider_type.in_(vcs_providers))
 
         if project_name:
             query = query.filter(model.DBrepository.project_key == project_name)
 
@@ -347,33 +357,107 @@
     :param finding_statuses:
         finding statuses to filter, type FindingStatus
     :param rule_name:
         rule_name to filter on
     :return: findings_count
         count of findings
     """
-    query = db_connection.query(model.DBfinding.status, func.count(model.DBfinding.status).label('status_count'))
+    # subquery to select latest audit ids findings
+    max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
+                                             func.max(model.DBaudit.id_).label("audit_id")) \
+        .group_by(model.DBaudit.finding_id).subquery()
+
+    query = db_connection.query(func.count(model.DBfinding.id_).label('status_count'), model.DBaudit.status)
+
+    query = query \
+        .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+              isouter=True) \
+        .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+              isouter=True)
 
     if scan_ids and len(scan_ids) > 0:
         query = query \
             .join(model.DBscanFinding,
                   model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_) \
             .join(model.DBscan,
                   model.scan.DBscan.id_ == model.scan_finding.DBscanFinding.scan_id) \
             .filter(model.DBscan.id_.in_(scan_ids))
     if finding_statuses:
-        query = query.filter(model.DBfinding.status.in_(finding_statuses))
+        if FindingStatus.NOT_ANALYZED in finding_statuses:
+            query = query. \
+                filter(or_(model.DBaudit.status.in_(finding_statuses),
+                           model.DBaudit.status == None))  # noqa: E711
+        else:
+            query = query.filter(model.DBaudit.status.in_(finding_statuses))
     if rule_name:
         query = query.filter(model.DBfinding.rule_name == rule_name)
 
-    findings_count_by_status = query.group_by(model.DBfinding.status).all()
+    findings_count_by_status = query.group_by(model.DBaudit.status).all()
 
     return findings_count_by_status
 
 
+def get_rule_findings_count_by_status(db_connection: Session):
+    """
+        Retrieve count of findings based on rulename and status
+    :param db_connection:
+        Session of the database connection
+    :return: findings_count
+        per rulename and status the count of findings
+    """
+    query = db_connection.query(model.DBfinding.rule_name,
+                                model.DBaudit.status,
+                                func.count(model.DBfinding.id_))
+
+    max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+                                                 func.max(model.DBscan.id_).label("latest_base_scan_id"))
+    max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
+    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
+
+    max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
+                                             func.max(model.DBaudit.id_).label("audit_id")) \
+        .group_by(model.DBaudit.finding_id).subquery()
+
+    query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
+    query = query.join(max_base_scan_subquery, model.DBfinding.branch_id == max_base_scan_subquery.c.branch_id)
+    query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
+                                          model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
+    query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.DBscanFinding.finding_id,
+                       isouter=True)
+    query = query.join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id, isouter=True)
+    query = query.group_by(model.DBfinding.rule_name, model.DBaudit.status)
+    query = query.order_by(model.DBfinding.rule_name, model.DBaudit.status)
+    status_counts = query.all()
+
+    rule_count_dict = {}
+    for status_count in status_counts:
+        rule_count_dict[status_count[0]] = {
+            "true_positive": 0,
+            "false_positive": 0,
+            "not_analyzed": 0,
+            "under_review": 0,
+            "clarification_required": 0,
+            "total_findings_count": 0
+        }
+    for status_count in status_counts:
+        rule_count_dict[status_count[0]]["total_findings_count"] += status_count[2]
+        if status_count[1] == FindingStatus.NOT_ANALYZED or status_count[1] is None:
+            rule_count_dict[status_count[0]]["not_analyzed"] += status_count[2]
+        elif status_count[1] == FindingStatus.FALSE_POSITIVE:
+            rule_count_dict[status_count[0]]["false_positive"] += status_count[2]
+        elif status_count[1] == FindingStatus.TRUE_POSITIVE:
+            rule_count_dict[status_count[0]]["true_positive"] += status_count[2]
+        elif status_count[1] == FindingStatus.UNDER_REVIEW:
+            rule_count_dict[status_count[0]]["under_review"] += status_count[2]
+        elif status_count[1] == FindingStatus.CLARIFICATION_REQUIRED:
+            rule_count_dict[status_count[0]]["clarification_required"] += status_count[2]
+
+    return rule_count_dict
+
+
 def get_findings_count_by_time(db_connection: Session,
                                date_type: DateFilter,
                                start_date_time: datetime = None,
                                end_date_time: datetime = None,
                                skip: int = 0,
                                limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT):
     """
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/scan.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,39 +110,14 @@
     )
     db_connection.add(db_scan)
     db_connection.commit()
     db_connection.refresh(db_scan)
     return db_scan
 
 
-def get_latest_scan_for_repository_for_master_branch(db_connection: Session, repository_id: int) -> model.DBscan:
-    """
-        Retrieve the most recent scan of a given repository object
-    :param db_connection:
-        Session of the database connection
-    :param repository_id:
-        id of the repository object for which to retrieve the most recent scan
-    :return: scan
-        scan object having the most recent timestamp for a given repository object
-    """
-    master_branch = ['master', 'main']
-    subquery = (db_connection.query(func.max(model.DBscan.timestamp).label("max_time"))
-                .filter(model.scan.DBscan.branch_id == model.branch.DBbranch.id_)
-                .filter(model.branch.DBbranch.repository_id == repository_id)
-                .filter(func.lower(model.branch.DBbranch.branch_name).in_(master_branch))
-                ).subquery()
-
-    scan = db_connection.query(model.DBscan) \
-        .join(subquery,
-              and_(model.DBscan.timestamp == subquery.c.max_time)) \
-        .first()
-
-    return scan
-
-
 def get_branch_findings_metadata_for_latest_scan(db_connection: Session, branch_id: int,
                                                  scan_timestamp: datetime):
     """
         Retrieves the finding metadata for latest scan of a branch from the database
     :param db_connection:
         Session of the database connection
     :param branch_id:
@@ -164,22 +139,22 @@
 
     true_positive_count = false_positive_count = not_analyzed_count = \
         under_review_count = clarification_required_count = 0
     if len(scan_ids_latest_to_base) > 0:
         findings_count_by_status = finding_crud.get_findings_count_by_status(
             db_connection, scan_ids=scan_ids_latest_to_base, finding_statuses=FindingStatus)
         for finding in findings_count_by_status:
-            finding_status = finding[0]
-            count = finding[1]
+            finding_status = finding[1]
+            count = finding[0]
             if finding_status == FindingStatus.TRUE_POSITIVE:
                 true_positive_count = count
             if finding_status == FindingStatus.FALSE_POSITIVE:
                 false_positive_count = count
-            if finding_status == FindingStatus.NOT_ANALYZED:
-                not_analyzed_count = count
+            if finding_status == FindingStatus.NOT_ANALYZED or finding_status is None:
+                not_analyzed_count += count
             if finding_status == FindingStatus.UNDER_REVIEW:
                 under_review_count = count
             if finding_status == FindingStatus.CLARIFICATION_REQUIRED:
                 clarification_required_count = count
 
     total_findings_count = true_positive_count + false_positive_count + not_analyzed_count \
         + under_review_count + clarification_required_count
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/scan_finding.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/scan_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/dependencies.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/dependencies.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 import ssl
 import urllib.error
 
 # Third Party
 import jwt
 import sqlalchemy.orm
-from fastapi import Depends, HTTPException, status
+from fastapi import Depends, HTTPException, Request, status
 from fastapi.security import HTTPBasicCredentials, HTTPBearer
 from jwt import PyJWKClient
 from tenacity import retry, stop_after_attempt, wait_exponential
 
 # First Party
 from resc_backend.constants import RESC_OPERATOR_ROLE
 from resc_backend.db.connection import Session, engine
 from resc_backend.db.model import DBbranch, DBfinding, DBrepository, DBrule, DBscan, DBscanFinding
 
 security = HTTPBearer()
 logger = logging.getLogger(__name__)
 
 
-async def requires_auth(credentials: HTTPBasicCredentials = Depends(security)):
+async def requires_auth(request: Request, credentials: HTTPBasicCredentials = Depends(security)):
     """
         Function that is used to validate the JWT access token
     """
     access_token = credentials.credentials
     algorithm = ["RS256"]
     issuer = os.getenv('SSO_ACCESS_TOKEN_ISSUER_URL', '')
     jwks_url = os.getenv('SSO_ACCESS_TOKEN_JWKS_URL', '')
@@ -46,15 +46,15 @@
             options=jwt_options,
         )
 
         if not user_has_resc_operator_role(claims):
             logger.error(f"Invalid login attempt for user {claims['email']}")
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN,
                                 detail="You don't have permission to access this resource.")
-
+        request.scope["user"] = claims['email']
     except urllib.error.URLError as error:
         logger.error(f"Unable to contact server for token validation {jwks_url} Message: {error}")
         raise HTTPException(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
                             detail="Unable to contact server for token validation") from error
 
     except jwt.InvalidAlgorithmError as error:
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="Algorithm is invalid for decoding token",
@@ -87,19 +87,19 @@
 def user_has_resc_operator_role(claims: dict) -> bool:
     """
         Function that is used to determine if the user has the RESC_OPERATOR_ROLE
     """
     return bool("roles" in claims and claims["roles"] == RESC_OPERATOR_ROLE)
 
 
-def requires_no_auth():
+def requires_no_auth(request: Request):
     """
         Function that is used for unauthenticated access
     """
-    return None
+    request.scope["user"] = "Anonymous"
 
 
 def get_db_connection():
     db_connection = Session(bind=engine)
     try:
         yield db_connection
     finally:
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/branches.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/branches.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Standard Library
 from datetime import datetime
 from typing import List, Optional
 
 # Third Party
-from fastapi import APIRouter, Depends, HTTPException, Query, Response, status
+from fastapi import APIRouter, Depends, HTTPException, Query, Request, Response, status
 
 # First Party
 from resc_backend.constants import (
     CACHE_MAX_AGE,
     DEFAULT_RECORDS_PER_PAGE_LIMIT,
     ERROR_MESSAGE_500,
     ERROR_MESSAGE_503,
@@ -16,14 +16,15 @@
     RWS_ROUTE_BY_RULE,
     RWS_ROUTE_COUNT_BY_TIME,
     RWS_ROUTE_FINDINGS,
     RWS_ROUTE_SUPPORTED_STATUSES,
     RWS_ROUTE_TOTAL_COUNT_BY_RULE
 )
 from resc_backend.db.connection import Session
+from resc_backend.resc_web_service.crud import audit as audit_crud
 from resc_backend.resc_web_service.crud import finding as finding_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model400, Model404
 from resc_backend.resc_web_service.schema import audit as audit_schema
 from resc_backend.resc_web_service.schema import finding as finding_schema
@@ -85,17 +86,14 @@
     - **file_path**: file path
     - **line_number**: Line number
     - **commit_id**: commit hash
     - **commit_message**: Commit message
     - **commit_timestamp**: Commit timestamp
     - **author**: Author name
     - **email**: Email of the author
-    - **status**: Status of the finding, Valid values are NOT_ANALYZED, UNDER_REVIEW,
-                  CLARIFICATION_REQUIRED, FALSE_POSITIVE, TRUE_POSITIVE
-    - **comment**: Comment
     - **event_sent_on**: event sent timestamp
     - **rule_name**: rule name
     - **branch_id**: branch id of the finding
     - **return**: int
           The output will contain the number of successful created findings
       """
     try:
@@ -160,49 +158,14 @@
         raise HTTPException(status_code=404, detail="Finding not found")
     return FindingRead.create_from_db_entities(
         finding_crud.patch_finding(db_connection, finding_id=finding_id, finding_update=finding_update),
         scan_ids
     )
 
 
-@router.put("/{finding_id}",
-            response_model=finding_schema.FindingRead,
-            summary="Update a finding by ID",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Update finding <finding_id>"},
-                404: {"model": Model404, "description": "Finding <finding_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
-def update_finding(
-        finding_id: int,
-        finding: finding_schema.FindingUpdate,
-        db_connection: Session = Depends(get_db_connection)
-):
-    """
-        Update a finding by ID
-
-    - **db_connection**: Session of the database connection
-    - **finding_ids**: List of finding IDs for which details need to be updated
-    - **status**: Status of the finding, Valid values are NOT_ANALYZED, UNDER_REVIEW,
-                  CLARIFICATION_REQUIRED, FALSE_POSITIVE, TRUE_POSITIVE
-    - **comment**: Comment
-    """
-    db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
-    db_sca_findings = scan_finding_crud.get_scan_findings(db_connection, finding_id=finding_id)
-    scan_ids = [x.scan_id for x in db_sca_findings]
-    if db_finding is None:
-        raise HTTPException(status_code=404, detail="Finding not found")
-    return FindingRead.create_from_db_entities(
-        finding_crud.update_finding(db_connection=db_connection, finding_id=finding_id, finding=finding),
-        scan_ids
-    )
-
-
 @router.delete("/{finding_id}",
                summary="Delete a finding",
                status_code=status.HTTP_200_OK,
                responses={
                    200: {"description": "Delete finding <finding_id>"},
                    404: {"model": Model404, "description": "Finding <finding_id> not found"},
                    500: {"description": ERROR_MESSAGE_500},
@@ -268,54 +231,79 @@
     """
     findings = finding_crud.get_findings_by_rule(db_connection, skip=skip, limit=limit, rule_name=rule_name)
     total_findings = finding_crud.get_total_findings_count(
         db_connection, findings_filter=FindingsFilter(rule_names=[rule_name]))
     return PaginationModel[finding_schema.FindingRead](data=findings, total=total_findings, limit=limit, skip=skip)
 
 
-@router.put(f"{RWS_ROUTE_AUDIT}/",
-            response_model=List[finding_schema.FindingRead],
-            summary="audit single/multiple findings",
-            status_code=status.HTTP_200_OK,
-            responses={
-                200: {"description": "Audit finding(s) to update status and comments"},
-                404: {"model": Model404, "description": "Finding <finding_id> not found"},
-                500: {"description": ERROR_MESSAGE_500},
-                503: {"description": ERROR_MESSAGE_503}
-            })
+@router.post(f"{RWS_ROUTE_AUDIT}/",
+             response_model=int,
+             summary="audit single/multiple findings",
+             status_code=status.HTTP_201_CREATED,
+             responses={
+                 201: {"description": "Audit(s) successfully saved"},
+                 404: {"model": Model404, "description": "Finding <finding_id> not found"},
+                 500: {"description": ERROR_MESSAGE_500},
+                 503: {"description": ERROR_MESSAGE_503}
+             })
 def audit_findings(
+        request: Request,
         audit: audit_schema.AuditMultiple,
         db_connection: Session = Depends(get_db_connection)
-) -> List[finding_schema.FindingRead]:
+) -> int:
     """
         Audit single/multiple findings, updating the status and comment
 
     - **db_connection**: Session of the database connection
     - **finding_ids**: List of finding IDs for which audit to be performed
     - **status**: Status of the finding, Valid values are NOT_ANALYZED, UNDER_REVIEW,
                   CLARIFICATION_REQUIRED, FALSE_POSITIVE, TRUE_POSITIVE
     - **comment**: Comment
-    - **return**: [FindingRead]
-        The output will contain a list of the findings that where updated
+    - **return**: int
+        The output will contain count of successful saved audits
     """
-    audited_findings = []
+    audits = []
     for finding_id in audit.finding_ids:
         db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
-        db_scan_findings = scan_finding_crud.get_scan_findings(db_connection, finding_id=finding_id)
-        scan_ids = [x.scan_id for x in db_scan_findings]
         if db_finding is None:
             raise HTTPException(status_code=404, detail=f"Finding {finding_id} not found")
-
-        audited_findings.append(
-            FindingRead.create_from_db_entities(
-                finding_crud.audit_finding(db_connection=db_connection, db_finding=db_finding,
-                                           status=audit.status, comment=audit.comment),
-                scan_ids=scan_ids)
+        audits.append(
+            audit_crud.create_audit(db_connection=db_connection, finding_id=db_finding.id_,
+                                    auditor=request.user, status=audit.status, comment=audit.comment)
         )
-    return audited_findings
+    return len(audits)
+
+
+@router.get("/{finding_id}"f"{RWS_ROUTE_AUDIT}",
+            response_model=PaginationModel[audit_schema.AuditRead],
+            summary="Get audit(s) for finding",
+            status_code=status.HTTP_200_OK,
+            responses={
+                200: {"description": "Retrieve all the audit entries for a finding"},
+                500: {"description": ERROR_MESSAGE_500},
+                503: {"description": ERROR_MESSAGE_503}
+            })
+def get_finding_audits(finding_id: int, skip: int = Query(default=0, ge=0),
+                       limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
+                       db_connection: Session = Depends(get_db_connection)) \
+        -> PaginationModel[audit_schema.AuditRead]:
+    """
+        Retrieve all audit objects paginated for a finding
+
+    - **db_connection**: Session of the database connection
+    - **finding_id**: id of the finding to get the audit for
+    - **skip**: Integer amount of records to skip to support pagination
+    - **limit**: Integer amount of records to return, to support pagination
+    - **return**: [AuditRead]
+        The output will contain a PaginationModel containing the list of AuditRead type objects,
+        or an empty list if no audit info was found
+    """
+    audits = audit_crud.get_finding_audits(db_connection, skip=skip, limit=limit, finding_id=finding_id)
+    total_audits = audit_crud.get_finding_audits_count(db_connection, finding_id=finding_id)
+    return PaginationModel[audit_schema.AuditRead](data=audits, total=total_audits, limit=limit, skip=skip)
 
 
 @router.get(f"{RWS_ROUTE_SUPPORTED_STATUSES}/",
             response_model=List[str],
             summary="Get all supported statuses for findings",
             status_code=status.HTTP_200_OK,
             responses={
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,24 +346,24 @@
         or empty if no scan was found
     """
     repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
     if repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
 
     findings_meta_data = repository_crud.get_findings_metadata_by_repository_id(
-        db_connection, repository_id=repository_id)
+        db_connection, repository_ids=[repository_id])
 
     return FindingCountModel[repository_schema.RepositoryRead](
         data=repository,
-        true_positive=findings_meta_data["true_positive"],
-        false_positive=findings_meta_data["false_positive"],
-        not_analyzed=findings_meta_data["not_analyzed"],
-        under_review=findings_meta_data["under_review"],
-        clarification_required=findings_meta_data["clarification_required"],
-        total_findings_count=findings_meta_data["total_findings_count"])
+        true_positive=findings_meta_data[repository_id]["true_positive"],
+        false_positive=findings_meta_data[repository_id]["false_positive"],
+        not_analyzed=findings_meta_data[repository_id]["not_analyzed"],
+        under_review=findings_meta_data[repository_id]["under_review"],
+        clarification_required=findings_meta_data[repository_id]["clarification_required"],
+        total_findings_count=findings_meta_data[repository_id]["total_findings_count"])
 
 
 @router.get(f"{RWS_ROUTE_FINDINGS_METADATA}/",
             response_model=PaginationModel[repository_enriched_schema.RepositoryEnrichedRead],
             summary="Get all repositories with findings metadata",
             status_code=status.HTTP_200_OK,
             responses={
@@ -405,29 +405,30 @@
                                                     only_if_has_findings=onlyifhasfindings)
 
     total_repositories = repository_crud.get_repositories_count(db_connection, vcs_providers=vcsproviders,
                                                                 project_filter=projectfilter,
                                                                 repository_filter=repositoryfilter,
                                                                 only_if_has_findings=onlyifhasfindings)
     repository_list = []
+    repo_ids = [repo.id_ for repo in repositories]
+    repo_findings_meta_data = repository_crud.get_findings_metadata_by_repository_id(
+        db_connection, repository_ids=repo_ids)
     for repo in repositories:
-        findings_meta_data = repository_crud.get_findings_metadata_by_repository_id(
-            db_connection, repository_id=repo.id_)
         enriched_repository = repository_enriched_schema.RepositoryEnrichedRead(
             id_=repo.id_,
             project_key=repo.project_key,
             repository_id=repo.repository_id,
             repository_name=repo.repository_name,
             repository_url=repo.repository_url,
             vcs_provider=repo.provider_type,
-            true_positive=findings_meta_data["true_positive"],
-            false_positive=findings_meta_data["false_positive"],
-            not_analyzed=findings_meta_data["not_analyzed"],
-            under_review=findings_meta_data["under_review"],
-            clarification_required=findings_meta_data["clarification_required"],
-            total_findings_count=findings_meta_data["total_findings_count"]
+            true_positive=repo_findings_meta_data[repo.id_]["true_positive"],
+            false_positive=repo_findings_meta_data[repo.id_]["false_positive"],
+            not_analyzed=repo_findings_meta_data[repo.id_]["not_analyzed"],
+            under_review=repo_findings_meta_data[repo.id_]["under_review"],
+            clarification_required=repo_findings_meta_data[repo.id_]["clarification_required"],
+            total_findings_count=repo_findings_meta_data[repo.id_]["total_findings_count"]
         )
         repository_list.append(enriched_repository)
 
     return PaginationModel[repository_enriched_schema.RepositoryEnrichedRead](data=repository_list,
                                                                               total=total_repositories,
                                                                               limit=limit, skip=skip)
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files 22% similar despite different names*

```diff
@@ -85,38 +85,30 @@
 def get_rules_finding_status_count(db_connection: Session = Depends(get_db_connection)) -> List[RuleFindingCountModel]:
     """
         Retrieve all detected rules with finding counts per supported status
 
     - **db_connection**: Session of the database connection
     - **return**: List[str] The output will contain a list of strings of unique rules with counts per status
     """
-    distinct_rules = finding_crud.get_distinct_rules_from_findings(db_connection)
-
+    rule_finding_counts = finding_crud.get_rule_findings_count_by_status(db_connection)
     rule_findings_counts = []
-    for rule in distinct_rules:
-        finding_count = 0
-        rule_finding_count = RuleFindingCountModel(rule_name=rule.rule_name)
-        count_by_status = finding_crud.get_findings_count_by_status(db_connection,
-                                                                    rule_name=rule_finding_count.rule_name)
-        handled_statuses = []
-        for status_count in count_by_status:
-            finding_status_count = StatusCount(status=status_count[0], count=status_count[1])
-            finding_count = finding_count + finding_status_count.count
-            handled_statuses.append(finding_status_count.status)
-            rule_finding_count.finding_statuses_count.append(finding_status_count)
-
-        for finding_status in FindingStatus:
-            # add default values of 0 for statuses without findings
-            if finding_status not in handled_statuses:
-                finding_status_count = StatusCount(status=finding_status, count=0)
-                rule_finding_count.finding_statuses_count.append(finding_status_count)
 
-        rule_finding_count.finding_count = finding_count
-        rule_finding_count.finding_statuses_count = sorted(rule_finding_count.finding_statuses_count,
-                                                           key=lambda status_counter: status_counter.status)
+    for rule_name, rule_counts in rule_finding_counts.items():
+        rule_finding_count = RuleFindingCountModel(rule_name=rule_name,
+                                                   finding_count=rule_counts["total_findings_count"])
+        rule_finding_count.finding_statuses_count.append(
+            StatusCount(status=FindingStatus.TRUE_POSITIVE, count=rule_counts["true_positive"]))
+        rule_finding_count.finding_statuses_count.append(
+            StatusCount(status=FindingStatus.FALSE_POSITIVE, count=rule_counts["false_positive"]))
+        rule_finding_count.finding_statuses_count.append(
+            StatusCount(status=FindingStatus.NOT_ANALYZED, count=rule_counts["not_analyzed"]))
+        rule_finding_count.finding_statuses_count.append(
+            StatusCount(status=FindingStatus.UNDER_REVIEW, count=rule_counts["under_review"]))
+        rule_finding_count.finding_statuses_count.append(
+            StatusCount(status=FindingStatus.CLARIFICATION_REQUIRED, count=rule_counts["clarification_required"]))
         rule_findings_counts.append(rule_finding_count)
 
     return rule_findings_counts
 
 
 def create_rule(
         rule: RuleCreate,
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/filters.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/filters.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/branch.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/branch.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     column_start: conint(gt=-1)
     column_end: conint(gt=-1)
     commit_id: constr(max_length=120)
     commit_message: str
     commit_timestamp: datetime.datetime
     author: constr(max_length=200)
     email: constr(max_length=100)
-    status: FindingStatus = FindingStatus.NOT_ANALYZED
+    status: Optional[FindingStatus] = FindingStatus.NOT_ANALYZED
     comment: Optional[constr(max_length=255)] = None
     rule_name: constr(max_length=200)
     rule_pack: constr(max_length=100)
     project_key: constr(min_length=1, max_length=100)
     repository_name: constr(min_length=1, max_length=100)
     repository_url: HttpUrl
     timestamp: datetime.datetime
@@ -79,14 +79,18 @@
                                 commit_id: str) -> str:
         github_commit_url = f"{repository_url}/commit/{commit_id}?" \
                             f"refName=refs/heads/{branch_name}&path=/{file_path}"
         return github_commit_url
 
     @root_validator
     def build_commit_url(cls, values) -> Dict:
+        if values["status"] is None:
+            values["status"] = FindingStatus.NOT_ANALYZED
+        if values["comment"] is None:
+            values["comment"] = ""
         if values["vcs_provider"] == VCSProviders.BITBUCKET:
             values["commit_url"] = cls.build_bitbucket_commit_url(repository_url=values["repository_url"],
                                                                   repository_name=values["repository_name"],
                                                                   project_key=values["project_key"],
                                                                   file_path=values["file_path"],
                                                                   commit_id=values["commit_id"])
         elif values["vcs_provider"] == VCSProviders.AZURE_DEVOPS:
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,38 +5,30 @@
 from typing import List, Optional
 
 # Third Party
 from pydantic import BaseModel, conint, conlist, constr
 
 # First Party
 from resc_backend.db.model import DBfinding
-from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 
 
 class FindingBase(BaseModel):
     file_path: constr(max_length=500)
     line_number: conint(gt=-1)
     column_start: conint(gt=-1)
     column_end: conint(gt=-1)
     commit_id: constr(max_length=120)
     commit_message: str
     commit_timestamp: datetime.datetime
     author: constr(max_length=200)
     email: constr(max_length=100)
-    status: FindingStatus = FindingStatus.NOT_ANALYZED
-    comment: Optional[constr(max_length=255)] = None
     event_sent_on: Optional[datetime.datetime]
     rule_name: constr(max_length=400)
 
 
-class FindingUpdate(BaseModel):
-    status: FindingStatus
-    comment: constr(max_length=255)
-
-
 class FindingPatch(BaseModel):
     event_sent_on: datetime.datetime
 
 
 class FindingCreate(FindingBase):
     branch_id: conint(gt=0)
 
@@ -65,14 +57,12 @@
             column_start=db_finding.column_start,
             column_end=db_finding.column_end,
             commit_id=db_finding.commit_id,
             commit_message=db_finding.commit_message,
             commit_timestamp=db_finding.commit_timestamp,
             author=db_finding.author,
             email=db_finding.email,
-            status=db_finding.status,
-            comment=db_finding.comment,
             event_sent_on=db_finding.event_sent_on,
             rule_name=db_finding.rule_name,
             branch_id=db_finding.branch_id,
             scan_ids=scan_ids
         )
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/repository.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/repository_enriched.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/repository_enriched.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/rule_count_model.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 # First Party
 from resc_backend.constants import AZURE_DEVOPS
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 
 class VCSInstanceBase(BaseModel):
-
     name: constr(max_length=200)
     provider_type: VCSProviders
     hostname: constr(max_length=200)
     port: conint(gt=-0, lt=65536)
     scheme: constr(max_length=20)
     exceptions: Optional[conlist(item_type=str, min_items=None, max_items=500)]
     scope: Optional[conlist(item_type=str, min_items=None, max_items=500)]
@@ -28,32 +27,25 @@
         if value not in allowed_schemes:
             raise ValueError(f"The scheme '{value}' must be one of the following {', '.join(allowed_schemes)}")
         return value
 
     @validator("organization", pre=True)
     @classmethod
     def check_organization(cls, value, values):
-        try:
-            if not value:
-                if values["provider_type"] == AZURE_DEVOPS:
-                    raise ValueError("The organization field needs to be specified for Azure devops vcs instances")
-            return value
-        except KeyError:
-            return value
+        if not value and values.get("provider_type", None) == AZURE_DEVOPS:
+            raise ValueError("The organization field needs to be specified for Azure devops vcs instances")
+        return value
 
     @validator("scope", pre=True)
     @classmethod
     def check_scope_and_exceptions(cls, value, values):
-        try:
-            if value and values["exceptions"]:
-                raise ValueError("You cannot specify bot the scope and exceptions to the scan, only one setting"
-                                 " is supported.")
-            return value
-        except KeyError:
-            return value
+        if value and values.get("exceptions", None):
+            raise ValueError("You cannot specify bot the scope and exceptions to the scan, only one setting"
+                             " is supported.")
+        return value
 
 
 class VCSInstanceCreate(VCSInstanceBase):
     pass
 
 
 class VCSInstanceRead(VCSInstanceBase):
```

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/branches.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/branches.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.1.0/src/resc_backend.egg-info/PKG-INFO` & `resc_backend-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resc-backend
-Version: 1.1.0
+Name: resc_backend
+Version: 1.2.0
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -176,15 +176,15 @@
 ```
 
 If you can override the images by providing below arguments to the script.
 ```bash
 cd tests/newman_tests
 ./run_newman_tests.sh -b <resc-backend image:tag> -d <resc-database image:tag>  -n <newman image:tag> 
 
-Example: ./run_integration_tests.sh -b 'rescabnamro/resc-backend:1.0.1' -d 'mcr.microsoft.com/azure-sql-edge:1.0.5' -n 'postman/newman:5.3.1-alpine'
+Example: ./run_newman_tests.sh -b 'rescabnamro/resc-backend:1.0.1' -d 'mcr.microsoft.com/azure-sql-edge:1.0.5' -n 'postman/newman:5.3.1-alpine'
 ```
 
 
 
 ## Create a migration for database changes
 [(Back to top)](#table-of-contents)
```

### Comparing `resc_backend-1.1.0/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-1.2.0/src/resc_backend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/resc_backend.egg-info/requires.txt
 src/resc_backend.egg-info/top_level.txt
 src/resc_backend/bin/__init__.py
 src/resc_backend/bin/rabbitmq_bootup.py
 src/resc_backend/db/__init__.py
 src/resc_backend/db/connection.py
 src/resc_backend/db/model/__init__.py
+src/resc_backend/db/model/audit.py
 src/resc_backend/db/model/branch.py
 src/resc_backend/db/model/finding.py
 src/resc_backend/db/model/repository.py
 src/resc_backend/db/model/rule.py
 src/resc_backend/db/model/rule_allow_list.py
 src/resc_backend/db/model/rule_pack.py
 src/resc_backend/db/model/scan.py
@@ -32,14 +33,15 @@
 src/resc_backend/helpers/rabbitmq/configuration.py
 src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
 src/resc_backend/resc_web_service/__init__.py
 src/resc_backend/resc_web_service/api.py
 src/resc_backend/resc_web_service/dependencies.py
 src/resc_backend/resc_web_service/filters.py
 src/resc_backend/resc_web_service/crud/__init__.py
+src/resc_backend/resc_web_service/crud/audit.py
 src/resc_backend/resc_web_service/crud/branch.py
 src/resc_backend/resc_web_service/crud/detailed_finding.py
 src/resc_backend/resc_web_service/crud/finding.py
 src/resc_backend/resc_web_service/crud/repository.py
 src/resc_backend/resc_web_service/crud/rule.py
 src/resc_backend/resc_web_service/crud/rule_pack.py
 src/resc_backend/resc_web_service/crud/scan.py
```

