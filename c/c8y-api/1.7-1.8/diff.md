# Comparing `tmp/c8y_api-1.7.tar.gz` & `tmp/c8y_api-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c8y_api-1.7.tar", last modified: Thu Mar 23 15:28:44 2023, max compression
+gzip compressed data, was "c8y_api-1.8.tar", last modified: Fri Apr 14 14:20:08 2023, max compression
```

## Comparing `c8y_api-1.7.tar` & `c8y_api-1.8.tar`

### file list

```diff
@@ -1,130 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.066104 c8y_api-1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.050104 c8y_api-1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.054104 c8y_api-1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-23 15:28:25.000000 c8y_api-1.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-23 15:28:25.000000 c8y_api-1.7/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-23 15:28:25.000000 c8y_api-1.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-23 15:28:25.000000 c8y_api-1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-03-23 15:28:25.000000 c8y_api-1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-23 15:28:25.000000 c8y_api-1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-23 15:28:44.066104 c8y_api-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-23 15:28:25.000000 c8y_api-1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.054104 c8y_api-1.7/c8y_api/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/_main_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.054104 c8y_api-1.7/c8y_api/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.058104 c8y_api-1.7/c8y_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/administration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/binaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17926 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    22887 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/managedobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/notification2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_api/model/tenant_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.054104 c8y_api-1.7/c8y_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-23 15:28:44.000000 c8y_api-1.7/c8y_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-03-23 15:28:44.000000 c8y_api-1.7/c8y_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 15:28:44.000000 c8y_api-1.7/c8y_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-23 15:28:44.000000 c8y_api-1.7/c8y_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-23 15:28:44.000000 c8y_api-1.7/c8y_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.058104 c8y_api-1.7/c8y_tk/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_tk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.058104 c8y_api-1.7/c8y_tk/notification2/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_tk/notification2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-03-23 15:28:25.000000 c8y_api-1.7/c8y_tk/notification2/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.058104 c8y_api-1.7/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_audits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_binaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_device_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_devicegroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_global_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_inventoryroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_tenant_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-03-23 15:28:25.000000 c8y_api-1.7/integration_tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-03-23 15:28:25.000000 c8y_api-1.7/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-23 15:28:25.000000 c8y_api-1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-23 15:28:25.000000 c8y_api-1.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.062104 c8y_api-1.7/samples/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/cumulocity-tenant_options.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/cumulocity.json
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/handling_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/multi_tenant_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/notification2_asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/notification2_synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/simple_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/simple_tenant_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/tenant_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/user_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-23 15:28:25.000000 c8y_api-1.7/samples/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-23 15:28:44.066104 c8y_api-1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-03-23 15:28:25.000000 c8y_api-1.7/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.062104 c8y_api-1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.066104 c8y_api-1.7/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/alarm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/application.json
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/audit_records.json
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/bulk_operations.json
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/event.json
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/global_role.json
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/inventoryrole.json
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/managed_object.json
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/operation.json
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/subscriptions.json
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/tenant_option.json
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_bulk_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_inventoryrole.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_managedobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_tenant_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    42314 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/model/user.json
--rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/test_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/test_device_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-03-23 15:28:25.000000 c8y_api-1.7/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:28:44.066104 c8y_api-1.7/util/
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-03-23 15:28:25.000000 c8y_api-1.7/util/microservice_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.355218 c8y_api-1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.331217 c8y_api-1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.335217 c8y_api-1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-14 14:19:56.000000 c8y_api-1.8/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 14:19:56.000000 c8y_api-1.8/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-14 14:19:56.000000 c8y_api-1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 14:19:56.000000 c8y_api-1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-14 14:19:56.000000 c8y_api-1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 14:19:56.000000 c8y_api-1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-14 14:20:08.355218 c8y_api-1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-14 14:19:56.000000 c8y_api-1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.335217 c8y_api-1.8/c8y_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_main_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.335217 c8y_api-1.8/c8y_api/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.339218 c8y_api-1.8/c8y_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/administration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/binaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17926 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22887 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/managedobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/notification2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/tenant_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.335217 c8y_api-1.8/c8y_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.339218 c8y_api-1.8/c8y_tk/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_tk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.339218 c8y_api-1.8/c8y_tk/notification2/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_tk/notification2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_tk/notification2/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.343218 c8y_api-1.8/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_audits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_device_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_devicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_global_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_inventoryroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_tenant_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-04-14 14:19:56.000000 c8y_api-1.8/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 14:19:56.000000 c8y_api-1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 14:19:56.000000 c8y_api-1.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.347218 c8y_api-1.8/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/cumulocity-tenant_options.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/cumulocity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/dealing_with_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/handling_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/multi_tenant_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/notification2_asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/notification2_synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/simple_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/simple_tenant_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/tenant_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/user_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-14 14:20:08.355218 c8y_api-1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-14 14:19:56.000000 c8y_api-1.8/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.347218 c8y_api-1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.355218 c8y_api-1.8/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/alarm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/audit_records.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/bulk_operations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/global_role.json
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/inventoryrole.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/managed_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/operation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/series.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/subscriptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/tenant_option.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_bulk_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_inventoryrole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_managedobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_tenant_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42314 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/user.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_device_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.355218 c8y_api-1.8/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-14 14:19:56.000000 c8y_api-1.8/util/microservice_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-14 14:19:56.000000 c8y_api-1.8/util/testing_util.py
```

### Comparing `c8y_api-1.7/.github/workflows/codeql-analysis.yml` & `c8y_api-1.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/.github/workflows/python-publish.yml` & `c8y_api-1.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/CHANGELOG.md` & `c8y_api-1.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## Version 1.8
+
+* Adding support for measurement series queries.
+
 ## Version 1.7
 
 * Adding support for the Audit API.
 
 * Added support for event attachment handling.
 
 * Adding support for bulk operations.
```

### Comparing `c8y_api-1.7/LICENSE` & `c8y_api-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/PKG-INFO` & `c8y_api-1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c8y_api
-Version: 1.7
+Version: 1.8
 Summary: Python client for the Cumulocity REST API
 Home-page: https://github.com/SoftwareAG/cumulocity-python-api
 Author: Christoph Souris
 Author-email: christoph.souris@softwareag.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `c8y_api-1.7/README.md` & `c8y_api-1.8/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-
-![GitHub](https://img.shields.io/github/license/SoftwareAG/cumulocity-python-api)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/SoftwareAG/cumulocity-python-api)
-![GitHub Release Date](https://img.shields.io/github/release-date/SoftwareAG/cumulocity-python-api)
-
-# cumulocity-python-api
-
-This project is a Python client for the Cumulocity REST API to make it easier to develop programs, scripts, device agents or microservices in Python.
-
-## Installation
-
-### Prerequisites
-
-Before installing the module (or any module for that matter) consider creating
-a virtual environment for your project. This is generally preferred over 
-installing modules and dependencies globally:
-
-```shell
-cd <project-root>
-python3 -m venv venv
-source venv/bin/activate
-``` 
-
-### Installation from PyPI
-
-The recommended way is to install the lastest distribution package directly from the Python Package Index (PyPI).
-You can either add _c8y_api_ as a dependency to your project using _setup.cfg_, or install it manually:
-
-```shell
-pip install c8y_api
-```
-
-### Installation using pip
-
-Releases are also archived within the GitHub releases page. The module is released as standard Python wheel (_.whl_ file).
-It can be ownloaded and installed using pip using the following command:
-
-```shell
-pip install <release wheel file>
-```
-
-Like installing from PyPI, this will install all necessary dependencies automatically.  For your
-reference, the module's dependencies are also listed in file _requirements.txt_.
- 
-### Manual installation
-
-Alternatively, you can clone the repository. The module sources can be used directly within your Python 3 project.
-Simply copy the _c8y_api_ folder to your sources root and install the requirements by running the following command:
-
-```shell
-pip3 install -r requirements.txt
-```
-
-The _requirements.txt_ file is part of the sources.
-
-If the _c8y_api_ folder is in your sources root folder all imports should
-work right away. Alternatively you can add _c8y_api_ to your _PYHTONPATH_:
-
-```shell
-export PYTHONPATH=<project-root>/c8y_api; $PYTHONPATH
-```
-
-## Licensing
-
-This project is licensed under the Apache 2.0 license - see <https://www.apache.org/licenses/LICENSE-2.0>
-
-______________________
-
-These tools are provided as-is and without warranty or support. They do not constitute part of the Software AG product suite. Users are free to use, fork and modify them, subject to the license agreement. While Software AG welcomes contributions, we cannot guarantee to include every contribution in the master project.
-
-______________________
-
-You can find additional information in the [Software AG TECHcommunity](https://tech.forums.softwareag.com/tag/Cumulocity-IoT). There is also a introductory article ([Getting started with the Cumulocity Python API](https://tech.forums.softwareag.com/t/getting-started-with-the-cumulocity-python-api/264700)) available.
-
-Contact us at [TECHcommunity](mailto:technologycommunity@softwareag.com?subject=Github/SoftwareAG) if you have any questions.
-
+
+![GitHub](https://img.shields.io/github/license/SoftwareAG/cumulocity-python-api)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/SoftwareAG/cumulocity-python-api)
+![GitHub Release Date](https://img.shields.io/github/release-date/SoftwareAG/cumulocity-python-api)
+
+# cumulocity-python-api
+
+This project is a Python client for the Cumulocity REST API to make it easier to develop programs, scripts, device agents or microservices in Python.
+
+## Installation
+
+### Prerequisites
+
+Before installing the module (or any module for that matter) consider creating
+a virtual environment for your project. This is generally preferred over 
+installing modules and dependencies globally:
+
+```shell
+cd <project-root>
+python3 -m venv venv
+source venv/bin/activate
+``` 
+
+### Installation from PyPI
+
+The recommended way is to install the lastest distribution package directly from the Python Package Index (PyPI).
+You can either add _c8y_api_ as a dependency to your project using _setup.cfg_, or install it manually:
+
+```shell
+pip install c8y_api
+```
+
+### Installation using pip
+
+Releases are also archived within the GitHub releases page. The module is released as standard Python wheel (_.whl_ file).
+It can be ownloaded and installed using pip using the following command:
+
+```shell
+pip install <release wheel file>
+```
+
+Like installing from PyPI, this will install all necessary dependencies automatically.  For your
+reference, the module's dependencies are also listed in file _requirements.txt_.
+ 
+### Manual installation
+
+Alternatively, you can clone the repository. The module sources can be used directly within your Python 3 project.
+Simply copy the _c8y_api_ folder to your sources root and install the requirements by running the following command:
+
+```shell
+pip3 install -r requirements.txt
+```
+
+The _requirements.txt_ file is part of the sources.
+
+If the _c8y_api_ folder is in your sources root folder all imports should
+work right away. Alternatively you can add _c8y_api_ to your _PYHTONPATH_:
+
+```shell
+export PYTHONPATH=<project-root>/c8y_api; $PYTHONPATH
+```
+
+## Licensing
+
+This project is licensed under the Apache 2.0 license - see <https://www.apache.org/licenses/LICENSE-2.0>
+
+______________________
+
+These tools are provided as-is and without warranty or support. They do not constitute part of the Software AG product suite. Users are free to use, fork and modify them, subject to the license agreement. While Software AG welcomes contributions, we cannot guarantee to include every contribution in the master project.
+
+______________________
+
+You can find additional information in the [Software AG TECHcommunity](https://tech.forums.softwareag.com/tag/Cumulocity-IoT). There is also a introductory article ([Getting started with the Cumulocity Python API](https://tech.forums.softwareag.com/t/getting-started-with-the-cumulocity-python-api/264700)) available.
+
+Contact us at [TECHcommunity](mailto:technologycommunity@softwareag.com?subject=Github/SoftwareAG) if you have any questions.
+
```

### Comparing `c8y_api-1.7/c8y_api/_auth.py` & `c8y_api-1.8/c8y_api/_auth.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/_base_api.py` & `c8y_api-1.8/c8y_api/_base_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/_jwt.py` & `c8y_api-1.8/c8y_api/_jwt.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/_main_api.py` & `c8y_api-1.8/c8y_api/_main_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/_registry_api.py` & `c8y_api-1.8/c8y_api/_registry_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/_util.py` & `c8y_api-1.8/c8y_api/_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/app/__init__.py` & `c8y_api-1.8/c8y_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/__init__.py` & `c8y_api-1.8/c8y_api/model/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,11 +22,11 @@
            'Permission', 'ReadPermission', 'WritePermission', 'AnyPermission',
            'Application',
            'AuditRecord', 'AuditRecords',
            'Operation', 'BulkOperation', 'Operations', 'BulkOperations',
            'ManagedObject', 'Device', 'DeviceGroup', 'Fragment', 'NamedObject',
            'Inventory', 'DeviceInventory', 'DeviceGroupInventory',
            'Identity', 'ExternalId', 'Binary', 'Binaries',
-           'Measurement', 'Measurements', 'Value', 'Count', 'Grams', 'Kilograms', 'Kelvin', 'Celsius',
+           'Measurement', 'Measurements', 'Series', 'Value', 'Count', 'Grams', 'Kilograms', 'Kelvin', 'Celsius',
            'Event', 'Events', 'Alarm', 'Alarms',
            'Subscription', 'Subscriptions', 'Tokens',
            'Meters', 'Centimeters', 'Liters', 'CubicMeters']
```

### Comparing `c8y_api-1.7/c8y_api/model/_base.py` & `c8y_api-1.8/c8y_api/model/_base.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/_parser.py` & `c8y_api-1.8/c8y_api/model/_parser.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/_util.py` & `c8y_api-1.8/c8y_api/model/_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/administration.py` & `c8y_api-1.8/c8y_api/model/administration.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/alarms.py` & `c8y_api-1.8/c8y_api/model/alarms.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/applications.py` & `c8y_api-1.8/c8y_api/model/applications.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/audit.py` & `c8y_api-1.8/c8y_api/model/audit.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/binaries.py` & `c8y_api-1.8/c8y_api/model/binaries.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/events.py` & `c8y_api-1.8/c8y_api/model/events.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/identity.py` & `c8y_api-1.8/c8y_api/model/identity.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/inventory.py` & `c8y_api-1.8/c8y_api/model/inventory.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/managedobjects.py` & `c8y_api-1.8/c8y_api/model/managedobjects.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/notification2.py` & `c8y_api-1.8/c8y_api/model/notification2.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/c8y_api/model/operations.py` & `c8y_api-1.8/c8y_api/model/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,14 +341,15 @@
     group_id = SimpleObject.UpdatableProperty('_u_group_id')
     failed_parent_id = SimpleObject.UpdatableProperty('_u_failed_parent_id')
     start_time = SimpleObject.UpdatableProperty('_u_start_time')
     creation_ramp = SimpleObject.UpdatableProperty('_u_creation_ramp')
 
     @property
     def operation_prototype(self) -> _DictWrapper:
+        # pylint: disable=missing-function-docstring
         return self.operationPrototype
 
     @operation_prototype.setter
     def operation_prototype(self, fragment):
         self.__setitem__('operationPrototype', fragment)
 
     @property
```

### Comparing `c8y_api-1.7/c8y_api.egg-info/PKG-INFO` & `c8y_api-1.8/c8y_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c8y-api
-Version: 1.7
+Version: 1.8
 Summary: Python client for the Cumulocity REST API
 Home-page: https://github.com/SoftwareAG/cumulocity-python-api
 Author: Christoph Souris
 Author-email: christoph.souris@softwareag.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `c8y_api-1.7/c8y_api.egg-info/SOURCES.txt` & `c8y_api-1.8/c8y_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 integration_tests/test_operations.py
 integration_tests/test_tenant_options.py
 integration_tests/test_users.py
 samples/Dockerfile
 samples/build.sh
 samples/cumulocity-tenant_options.json
 samples/cumulocity.json
+samples/dealing_with_measurements.py
 samples/handling_events.py
 samples/multi_tenant_app.py
 samples/notification2_asynchronous.py
 samples/notification2_synchronous.py
 samples/simple_agent.py
 samples/simple_tenant_app.py
 samples/tenant_options.py
@@ -87,14 +88,15 @@
 tests/model/bulk_operations.json
 tests/model/device.json
 tests/model/event.json
 tests/model/global_role.json
 tests/model/inventoryrole.json
 tests/model/managed_object.json
 tests/model/operation.json
+tests/model/series.json
 tests/model/subscriptions.json
 tests/model/tenant_option.json
 tests/model/test_alarm.py
 tests/model/test_application.py
 tests/model/test_audit.py
 tests/model/test_base.py
 tests/model/test_bulk_operation.py
@@ -108,8 +110,9 @@
 tests/model/test_operation.py
 tests/model/test_parser.py
 tests/model/test_resource.py
 tests/model/test_subscription.py
 tests/model/test_tenant_option.py
 tests/model/test_user.py
 tests/model/user.json
-util/microservice_util.py
+util/microservice_util.py
+util/testing_util.py
```

### Comparing `c8y_api-1.7/c8y_tk/notification2/listener.py` & `c8y_api-1.8/c8y_tk/notification2/listener.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/conftest.py` & `c8y_api-1.8/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_alarms.py` & `c8y_api-1.8/integration_tests/test_alarms.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_applications.py` & `c8y_api-1.8/integration_tests/test_applications.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_audits.py` & `c8y_api-1.8/integration_tests/test_audits.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_binaries.py` & `c8y_api-1.8/integration_tests/test_binaries.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_bulk_operations.py` & `c8y_api-1.8/integration_tests/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_device_registry.py` & `c8y_api-1.8/integration_tests/test_device_registry.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_devicegroups.py` & `c8y_api-1.8/integration_tests/test_devicegroups.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_events.py` & `c8y_api-1.8/integration_tests/test_events.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_global_roles.py` & `c8y_api-1.8/integration_tests/test_global_roles.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_identity.py` & `c8y_api-1.8/integration_tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_inventory.py` & `c8y_api-1.8/integration_tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_inventoryroles.py` & `c8y_api-1.8/integration_tests/test_inventoryroles.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_operations.py` & `c8y_api-1.8/integration_tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_tenant_options.py` & `c8y_api-1.8/integration_tests/test_tenant_options.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/integration_tests/test_users.py` & `c8y_api-1.8/integration_tests/test_users.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/pylintrc` & `c8y_api-1.8/pylintrc`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/samples/build.sh` & `c8y_api-1.8/samples/build.sh`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 [[ -d "$DIST_DIR" ]] && rm -rf "$DIST_DIR"
 mkdir -p "$DIST_DIR"
 
 # copy & render sources
 cp ./requirements.txt "$BUILD_DIR"
 cp ./samples/util.py "$BUILD_DIR"
 cp "./samples/$NAME.py" "$BUILD_DIR"
+cp "./util/testing_util.py" "$BUILD_DIR"
 cp -r "./c8y_api" "$BUILD_DIR"
+cp -r "./c8y_tk" "$BUILD_DIR"
 sed -e "s/{VERSION}/$VERSION/g" ./samples/cumulocity.json > "$BUILD_DIR/cumulocity.json"
 sed -e "s/{SAMPLE}/$NAME/g" ./samples/Dockerfile > "$BUILD_DIR/Dockerfile"
 # extend cumulocity.json is defined
 if [[ -r ./samples/cumulocity-$NAME.json ]]; then
   echo -n "Found custom extension at './samples/cumulocity-$NAME.json'. Applying ..."
   tmp=`tempfile`
   jq -s '.[0] + .[1]' "$BUILD_DIR/cumulocity.json" ./samples/cumulocity-$NAME.json > $tmp
```

### Comparing `c8y_api-1.7/samples/handling_events.py` & `c8y_api-1.8/samples/handling_events.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/samples/multi_tenant_app.py` & `c8y_api-1.8/samples/multi_tenant_app.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/samples/notification2_asynchronous.py` & `c8y_api-1.8/samples/notification2_asynchronous.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 # as specifically provided for in your License Agreement with Software AG.
 
 # pylint: disable=missing-function-docstring
 
 import asyncio
 
 from c8y_api.app import SimpleCumulocityApp
-from c8y_api.model import ManagedObject
+from c8y_api.model import ManagedObject, Subscription
 from c8y_tk.notification2 import AsyncListener
-from model.notification2 import Subscription
 
-from tests import RandomNameGenerator
+from testing_util import RandomNameGenerator
 from util import load_dotenv
 
 
 async def main():
 
     c8y = SimpleCumulocityApp()
     print("CumulocityApp initialized.")
```

### Comparing `c8y_api-1.7/samples/notification2_synchronous.py` & `c8y_api-1.8/samples/notification2_synchronous.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import threading
 import time
 
 from c8y_api.app import SimpleCumulocityApp
 from c8y_api.model import ManagedObject, Subscription
 from c8y_tk.notification2 import Listener
 
-from tests import RandomNameGenerator
+from testing_util import RandomNameGenerator
 from util import load_dotenv
 
 
 # load environment from a .env if present
 load_dotenv()
 
 # initialize Cumulocity connection
```

### Comparing `c8y_api-1.7/samples/simple_agent.py` & `c8y_api-1.8/samples/simple_agent.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/samples/simple_tenant_app.py` & `c8y_api-1.8/samples/simple_tenant_app.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/samples/tenant_options.py` & `c8y_api-1.8/samples/tenant_options.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/samples/user_sessions.py` & `c8y_api-1.8/samples/user_sessions.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/samples/util.py` & `c8y_api-1.8/samples/util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/setup.cfg` & `c8y_api-1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tasks.py` & `c8y_api-1.8/tasks.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/alarm.json` & `c8y_api-1.8/tests/model/alarm.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/application.json` & `c8y_api-1.8/tests/model/application.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/audit_records.json` & `c8y_api-1.8/tests/model/audit_records.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/bulk_operations.json` & `c8y_api-1.8/tests/model/bulk_operations.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/device.json` & `c8y_api-1.8/tests/model/device.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/event.json` & `c8y_api-1.8/tests/model/event.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/global_role.json` & `c8y_api-1.8/tests/model/global_role.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/inventoryrole.json` & `c8y_api-1.8/tests/model/inventoryrole.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/managed_object.json` & `c8y_api-1.8/tests/model/managed_object.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/subscriptions.json` & `c8y_api-1.8/tests/model/subscriptions.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/tenant_option.json` & `c8y_api-1.8/tests/model/tenant_option.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 7% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-00000000: 7b0d 0a20 2020 2022 7365 6c66 223a 2022  {..    "self": "
-00000010: 6874 7470 733a 2f2f 7431 3233 3435 2e63  https://t12345.c
-00000020: 756d 756c 6f63 6974 792e 636f 6d2f 7465  umulocity.com/te
-00000030: 6e61 6e74 2f6f 7074 696f 6e73 2f6a 7774  nant/options/jwt
-00000040: 2f63 7265 6465 6e74 6961 6c73 2e6b 6579  /credentials.key
-00000050: 2e70 7269 7661 7465 222c 0d0a 2020 2020  .private",..    
-00000060: 2263 6174 6567 6f72 7922 3a20 226a 7774  "category": "jwt
-00000070: 222c 0d0a 2020 2020 2276 616c 7565 223a  ",..    "value":
-00000080: 2022 6336 6338 3463 3333 6139 3739 3038   "c6c84c33a97908
-00000090: 3632 6233 6265 3630 3635 3536 3539 6237  62b3be60655659b7
-000000a0: 6435 3861 3939 3931 6263 3935 6433 3766  d58a9991bc95d37f
-000000b0: 3566 6331 3738 3932 6334 3135 3862 3333  5fc17892c4158b33
-000000c0: 3835 6332 3066 3136 3363 6537 3432 3463  85c20f163ce7424c
-000000d0: 3363 6135 6434 3731 3836 3761 3364 3463  3ca5d471867a3d4c
-000000e0: 6161 3333 3939 3565 6338 3236 3938 3731  aa33995ec8269871
-000000f0: 6533 3066 3564 3130 3537 3966 6238 6630  e30f5d10579fb8f0
-00000100: 3662 3762 3938 6237 3734 6461 6563 3965  6b7b98b774daec9e
-00000110: 6162 3239 3764 6231 3636 6433 3662 3534  ab297db166d36b54
-00000120: 6263 6438 3438 6132 3635 6262 3136 3239  bcd848a265bb1629
-00000130: 6333 3431 3465 3739 3435 3461 3665 6461  c3414e79454a6eda
-00000140: 6663 3165 3535 6230 3730 3332 3364 3439  fc1e55b070323d49
-00000150: 3635 6139 6537 3639 6562 3662 6666 6332  65a9e769eb6bffc2
-00000160: 6231 6461 3964 3334 3861 3538 3761 6531  b1da9d348a587ae1
-00000170: 3366 3135 3565 3035 6635 6432 6539 6466  3f155e05f5d2e9df
-00000180: 6262 6136 6363 3338 6439 3563 6630 3037  bba6cc38d95cf007
-00000190: 3638 6565 6261 3264 3134 3838 6237 6630  68eeba2d1488b7f0
-000001a0: 6430 3364 3436 3432 6564 3530 6264 3135  d03d4642ed50bd15
-000001b0: 3436 3263 6430 6533 3937 3865 3439 3365  462cd0e3978e493e
-000001c0: 6534 6635 3832 3637 3635 3635 6639 3930  e4f582676565f990
-000001d0: 3537 6465 3139 3362 3864 3831 3963 6239  57de193b8d819cb9
-000001e0: 3039 3662 3438 3831 3263 3239 3666 3035  096b48812c296f05
-000001f0: 3262 3032 6332 3965 3463 3130 3630 6161  2b02c29e4c1060aa
-00000200: 6133 3665 3862 6263 3161 3837 3131 3465  a36e8bbc1a87114e
-00000210: 6664 3936 6632 6631 6334 3263 6263 6630  fd96f2f1c42cbcf0
-00000220: 3239 3735 3531 3563 6438 3634 3362 6534  2975515cd8643be4
-00000230: 3364 6332 3931 3634 6531 3537 3862 6132  3dc29164e1578ba2
-00000240: 3233 6165 3162 6165 3634 3737 3032 6161  23ae1bae647702aa
-00000250: 6363 6534 3637 3838 3933 6335 6436 6334  cce4678893c5d6c4
-00000260: 3933 3566 6238 6462 6565 3235 6334 3038  935fb8dbee25c408
-00000270: 3165 3937 6139 3763 6539 3736 3462 3136  1e97a97ce9764b16
-00000280: 3064 3366 3863 3037 3130 3736 6637 6564  0d3f8c071076f7ed
-00000290: 6230 3137 3737 3539 6330 6134 3036 3333  b0177759c0a40633
-000002a0: 3366 3237 3337 3633 3136 3964 6434 3935  3f273763169dd495
-000002b0: 6132 3535 6639 3438 3861 6534 3565 3562  a255f9488ae45e5b
-000002c0: 3739 6533 3338 3866 3337 3863 6433 6162  79e3388f378cd3ab
-000002d0: 6363 3933 3233 3532 3062 3662 3633 3839  cc9323520b6b6389
-000002e0: 6664 3063 6562 6161 6563 3533 6361 3232  fd0cebaaec53ca22
-000002f0: 3661 3137 3038 6264 3339 3566 3561 3261  6a1708bd395f5a2a
-00000300: 3339 3436 3266 3664 3533 3230 3736 6130  39462f6d532076a0
-00000310: 6135 3064 6466 3761 3736 3035 3935 6136  a50ddf7a760595a6
-00000320: 6236 3066 3661 6438 3236 3461 6261 3237  b60f6ad8264aba27
-00000330: 3863 3138 3933 3431 6166 6231 3761 3838  8c189341afb17a88
-00000340: 3739 3534 6534 3165 3664 3738 3661 3735  7954e41e6d786a75
-00000350: 3064 3031 3664 3839 6663 3435 6338 3438  0d016d89fc45c848
-00000360: 3665 3835 6161 3061 3062 6364 6636 3866  6e85aa0a0bcdf68f
-00000370: 3131 3964 6330 3539 6162 3334 3237 3662  119dc059ab34276b
-00000380: 3033 3837 3664 3134 3761 3964 3565 3663  03876d147a9d5e6c
-00000390: 3538 6332 6262 3262 6234 6630 3534 6438  58c2bb2bb4f054d8
-000003a0: 6234 3636 3665 3162 6231 3866 3935 3430  b4666e1bb18f9540
-000003b0: 3839 6266 3434 6536 3164 3162 3366 6365  89bf44e61d1b3fce
-000003c0: 6664 3233 3638 3038 3065 3233 3036 3036  fd2368080e230606
-000003d0: 3539 3439 3463 3062 3965 6563 3630 3038  59494c0b9eec6008
-000003e0: 3263 3866 3435 3739 3465 3134 3935 3130  2c8f45794e149510
-000003f0: 3734 6131 6433 3462 3865 6564 3666 3737  74a1d34b8eed6f77
-00000400: 3132 6364 6466 3462 6439 3434 3563 3563  12cddf4bd9445c5c
-00000410: 3663 6334 6137 6330 3964 3735 3936 3263  6cc4a7c09d75962c
-00000420: 6137 3831 3232 3834 3230 6563 3966 3639  a781228420ec9f69
-00000430: 3539 3065 3839 6238 3137 3335 3438 3532  590e89b817354852
-00000440: 6631 6464 6433 3737 6564 3463 6266 6131  f1ddd377ed4cbfa1
-00000450: 3738 3662 3139 3734 3135 3833 6166 6633  786b19741583aff3
-00000460: 6363 3436 6165 3565 3463 6332 6430 6530  cc46ae5e4cc2d0e0
-00000470: 3835 3135 3333 3665 3834 3266 3664 6431  8515336e842f6dd1
-00000480: 3063 6662 3161 6332 6337 6664 6534 6466  0cfb1ac2c7fde4df
-00000490: 6666 3066 6534 3938 6339 6136 6632 3664  ff0fe498c9a6f26d
-000004a0: 3161 3538 6238 6161 6535 6266 3265 6336  1a58b8aae5bf2ec6
-000004b0: 3139 6139 6334 3561 6134 6233 6664 3139  19a9c45aa4b3fd19
-000004c0: 3739 3762 3137 3230 3762 3833 6534 6263  797b17207b83e4bc
-000004d0: 3535 3531 3033 6264 6634 3732 3738 3762  555103bdf472787b
-000004e0: 3961 3464 3239 3331 3235 3363 3662 3533  9a4d2931253c6b53
-000004f0: 3536 3466 3538 3735 3761 3762 6133 6438  564f58757a7ba3d8
-00000500: 6662 3730 3739 3130 3736 3736 3461 6437  fb70791076764ad7
-00000510: 6231 6331 3939 3562 3662 3038 3138 3036  b1c1995b6b081806
-00000520: 3663 6162 3338 6630 3738 6131 3435 6130  6cab38f078a145a0
-00000530: 3663 6362 3561 6163 3836 3962 3666 3162  6ccb5aac869b6f1b
-00000540: 3836 3038 6638 3866 6361 3138 3766 3533  8608f88fca187f53
-00000550: 6338 3138 6137 6238 3236 6463 3030 6539  c818a7b826dc00e9
-00000560: 6262 6632 3163 3261 3239 6337 6435 3939  bbf21c2a29c7d599
-00000570: 3431 6663 6537 6530 6663 3964 3536 3830  41fce7e0fc9d5680
-00000580: 6564 3937 6633 6261 6532 6533 6535 3166  ed97f3bae2e3e51f
-00000590: 6463 3732 3239 6536 6138 6535 3164 3938  dc7229e6a8e51d98
-000005a0: 3430 3839 3332 3832 3966 3364 3661 3834  408932829f3d6a84
-000005b0: 6264 3565 6538 3361 3839 6332 6436 3366  bd5ee83a89c2d63f
-000005c0: 6634 6133 3436 6634 3233 6362 6566 3362  f4a346f423cbef3b
-000005d0: 6436 6334 3932 3565 3232 3563 3239 6561  d6c4925e225c29ea
-000005e0: 3039 3938 6437 3661 3964 6663 6465 3264  0998d76a9dfcde2d
-000005f0: 3632 3261 3332 6238 6261 3532 3562 3032  622a32b8ba525b02
-00000600: 3435 6438 6436 6232 6664 6131 3030 3030  45d8d6b2fda10000
-00000610: 3263 6531 6637 3837 3233 3734 3938 3930  2ce1f78723749890
-00000620: 3966 3339 3838 3832 3531 3831 3930 6363  9f398882518190cc
-00000630: 3336 6430 3264 6633 6335 3064 3132 3330  36d02df3c50d1230
-00000640: 3063 3236 3764 6638 6363 6439 3366 6362  0c267df8ccd93fcb
-00000650: 6639 6261 6330 3733 3032 6439 3464 3137  f9bac07302d94d17
-00000660: 3366 3636 6530 3039 3736 6634 6161 6133  3f66e00976f4aaa3
-00000670: 3834 6664 3838 3362 6465 6136 3836 3930  84fd883bdea68690
-00000680: 3433 3162 3761 6630 3361 3639 6133 3861  431b7af03a69a38a
-00000690: 6334 3238 3835 3332 3162 3966 3430 3233  c42885321b9f4023
-000006a0: 3261 3831 3839 3839 6535 3634 3065 3033  2a818989e5640e03
-000006b0: 3133 3239 6232 3564 6166 3638 6635 3431  1329b25daf68f541
-000006c0: 6632 3238 3566 6339 6330 3661 6637 3234  f2285fc9c06af724
-000006d0: 6236 3630 3230 3532 6637 3063 6234 3130  b6602052f70cb410
-000006e0: 3130 6433 6432 3838 3162 3530 3938 3434  10d3d2881b509844
-000006f0: 6435 3735 3138 6662 6432 3665 3631 3531  d57518fbd26e6151
-00000700: 3635 3039 3936 6166 6433 6432 6230 3232  650996afd3d2b022
-00000710: 6133 6362 3262 3933 6135 3662 3962 3362  a3cb2b93a56b9b3b
-00000720: 3763 6134 6330 3832 3133 6133 3064 6561  7ca4c08213a30dea
-00000730: 3764 3132 3265 3662 6432 3866 6639 3634  7d122e6bd28ff964
-00000740: 6662 3265 6631 6530 6562 6235 6135 6538  fb2ef1e0ebb5a5e8
-00000750: 6265 6332 3434 3134 3365 3432 3362 3238  bec244143e423b28
-00000760: 6166 3761 3135 3366 6438 6136 3363 6363  af7a153fd8a63ccc
-00000770: 3038 3061 6664 3866 6237 6230 6338 3839  080afd8fb7b0c889
-00000780: 3539 3034 3561 6336 6539 3232 3234 6663  59045ac6e92224fc
-00000790: 3262 3238 6163 3163 6231 3061 3366 3934  2b28ac1cb10a3f94
-000007a0: 3233 3932 6131 3234 6433 6134 3735 3661  2392a124d3a4756a
-000007b0: 3964 3533 6661 3138 6334 3166 3638 3233  9d53fa18c41f6823
-000007c0: 3535 6630 3731 6538 3330 3331 6632 6333  55f071e83031f2c3
-000007d0: 3137 6439 3566 3364 6534 6537 6433 3935  17d95f3de4e7d395
-000007e0: 6136 6166 3935 6639 3933 6465 3835 6132  a6af95f993de85a2
-000007f0: 3838 6433 6165 3636 3938 3865 6661 3662  88d3ae66988efa6b
-00000800: 3736 6439 3737 3264 6266 6333 6239 3637  76d9772dbfc3b967
-00000810: 3437 6139 3535 3266 6662 6363 6238 6236  47a9552ffbccb8b6
-00000820: 3039 3831 3830 6264 6438 3264 6638 3561  098180bdd82df85a
-00000830: 6265 3939 6435 3766 3633 3839 3532 3330  be99d57f63895230
-00000840: 3632 6136 3438 3438 3638 6665 3662 3133  62a6484868fe6b13
-00000850: 6639 6435 3537 3964 6164 3861 3831 3436  f9d5579dad8a8146
-00000860: 6531 3737 3362 3862 3865 6163 3561 3761  e1773b8b8eac5a7a
-00000870: 6565 3261 6363 6330 6531 3934 3465 3563  ee2accc0e1944e5c
-00000880: 3737 3961 3231 3663 6437 3439 6666 3262  779a216cd749ff2b
-00000890: 6333 3261 3535 6464 3737 3363 3735 3066  c32a55dd773c750f
-000008a0: 6664 6536 3630 3535 6134 6133 3938 6630  fde66055a4a398f0
-000008b0: 6331 3035 6361 3163 3237 6630 3464 3139  c105ca1c27f04d19
-000008c0: 6234 3161 6362 6139 3637 3762 3961 6137  b41acba9677b9aa7
-000008d0: 6466 3163 3737 6237 3262 6336 3431 6361  df1c77b72bc641ca
-000008e0: 3333 6631 6262 6333 6539 6161 6437 3431  33f1bbc3e9aad741
-000008f0: 6364 3736 3834 3262 3536 3564 3434 6530  cd76842b565d44e0
-00000900: 3731 3763 6431 6431 6463 3030 3464 3462  717cd1d1dc004d4b
-00000910: 3932 3635 3531 3364 3566 6662 6365 3030  9265513d5ffbce00
-00000920: 6139 3635 6438 6232 3339 6534 3665 6336  a965d8b239e46ec6
-00000930: 3261 6264 3063 3138 3638 3936 3338 6534  2abd0c18689638e4
-00000940: 6564 3831 3861 3566 6661 3534 3230 3037  ed818a5ffa542007
-00000950: 6130 3638 3835 6538 3262 3639 3934 3764  a06885e82b69947d
-00000960: 6562 3762 3336 3634 6162 3437 3633 3535  eb7b3664ab476355
-00000970: 3831 6139 6264 6561 3766 3834 3939 3638  81a9bdea7f849968
-00000980: 3766 3362 3634 6533 3535 6137 3533 3630  7f3b64e355a75360
-00000990: 6236 3037 3564 6234 3363 6633 3839 6539  b6075db43cf389e9
-000009a0: 3634 3639 3166 6638 3338 3735 6235 3636  64691ff83875b566
-000009b0: 3135 3265 3162 3939 6437 3538 3530 3133  152e1b99d7585013
-000009c0: 3263 3465 3133 3432 6461 3232 3164 3038  2c4e1342da221d08
-000009d0: 3137 3862 3964 6236 6666 6362 3961 6332  178b9db6ffcb9ac2
-000009e0: 3065 6432 6239 3566 3937 6565 3633 3261  0ed2b95f97ee632a
-000009f0: 3264 3039 3434 6463 6336 3632 3934 3964  2d0944dcc662949d
-00000a00: 3531 6131 3435 6239 3438 3036 3532 6665  51a145b9480652fe
-00000a10: 3365 6439 6531 3736 3866 6334 6139 3464  3ed9e1768fc4a94d
-00000a20: 3466 6434 3763 6262 6630 3534 3265 6561  4fd47cbbf0542eea
-00000a30: 3531 3033 3263 6438 3664 3235 3831 3232  51032cd86d258122
-00000a40: 3435 6363 6239 3964 3666 3563 6564 3637  45ccb99d6f5ced67
-00000a50: 3937 3337 3962 6665 3736 6236 3832 6361  97379bfe76b682ca
-00000a60: 3562 6237 3537 6131 3532 3963 3733 3764  5bb757a1529c737d
-00000a70: 6166 3530 6434 3533 3532 6235 3630 3962  af50d45352b5609b
-00000a80: 6632 3664 6562 3331 3536 3738 3463 3836  f26deb3156784c86
-00000a90: 3566 6534 3564 6465 6564 3738 3235 3238  5fe45ddeed782528
-00000aa0: 3736 6264 6535 3836 6261 3836 3566 6532  76bde586ba865fe2
-00000ab0: 3835 3938 3230 3166 6136 3837 3461 3034  8598201fa6874a04
-00000ac0: 6363 3363 3661 3137 6261 6131 3762 3234  cc3c6a17baa17b24
-00000ad0: 6462 6565 6638 3139 3438 6637 6563 3762  dbeef81948f7ec7b
-00000ae0: 3630 3331 6434 6335 3836 3165 3436 3039  6031d4c5861e4609
-00000af0: 3762 3935 3638 3836 3632 3532 6139 3335  7b9568866252a935
-00000b00: 3632 3534 6431 3036 3338 3732 3639 6337  6254d106387269c7
-00000b10: 3032 3338 3931 6465 3636 6633 3638 6261  023891de66f368ba
-00000b20: 3531 6131 6263 3037 6634 3436 3334 3735  51a1bc07f4463475
-00000b30: 3933 3463 3839 3330 3165 6436 6433 6538  934c89301ed6d3e8
-00000b40: 6538 3265 3835 6432 3763 3964 6563 6234  e82e85d27c9decb4
-00000b50: 6637 3762 3830 3639 3138 3061 6639 3466  f77b8069180af94f
-00000b60: 6636 3065 3363 6662 6563 3137 6361 6537  f60e3cfbec17cae7
-00000b70: 3130 3165 6461 3064 6163 3135 3036 6466  101eda0dac1506df
-00000b80: 6231 3662 3738 3531 6663 3561 3864 3662  b16b7851fc5a8d6b
-00000b90: 6539 6130 6536 3764 3462 3333 6566 6334  e9a0e67d4b33efc4
-00000ba0: 6635 3137 3566 3131 3533 3764 6537 6338  f5175f11537de7c8
-00000bb0: 3366 6330 3339 3635 3966 6661 6466 3266  3fc039659ffadf2f
-00000bc0: 3362 3430 3566 3531 3664 6233 3261 6535  3b405f516db32ae5
-00000bd0: 6161 3466 3135 3031 6662 3365 3262 3762  aa4f1501fb3e2b7b
-00000be0: 3430 3334 6431 3937 6130 6335 3766 3132  4034d197a0c57f12
-00000bf0: 3938 3333 3365 6265 3432 6238 6534 3239  98333ebe42b8e429
-00000c00: 3839 3038 6133 6663 3230 6135 6164 3934  8908a3fc20a5ad94
-00000c10: 3262 3830 6364 6131 3337 3361 3935 3033  2b80cda1373a9503
-00000c20: 3665 3733 6139 3835 3536 3030 3934 3234  6e73a98556009424
-00000c30: 3764 6536 3435 3833 3731 6636 3135 3865  7de6458371f6158e
-00000c40: 6263 6461 6437 3964 3335 3866 3032 3238  bcdad79d358f0228
-00000c50: 3963 3134 3732 3834 3435 3332 6631 3237  9c1472844532f127
-00000c60: 3664 3764 3762 6235 3662 6661 3336 6339  6d7d7bb56bfa36c9
-00000c70: 3535 6632 3930 6162 3664 6134 3263 6338  55f290ab6da42cc8
-00000c80: 3863 6531 3563 6663 3733 3336 3162 3233  8ce15cfc73361b23
-00000c90: 6630 3230 3138 3163 3430 3436 3535 3865  f020181c4046558e
-00000ca0: 3663 3534 6539 6333 3739 6464 6132 6639  6c54e9c379dda2f9
-00000cb0: 6439 3062 6237 3065 6136 6163 3835 6561  d90bb70ea6ac85ea
-00000cc0: 3331 3831 3833 6666 6166 3638 6133 6134  318183ffaf68a3a4
-00000cd0: 3336 3330 3336 6364 3163 6363 3934 6331  363036cd1ccc94c1
-00000ce0: 3064 3865 6461 3134 3039 3330 3563 6639  0d8eda1409305cf9
-00000cf0: 6663 3630 3335 3434 3030 6465 3438 6465  fc60354400de48de
-00000d00: 3035 3936 6233 6633 3564 3936 3131 3464  0596b3f35d96114d
-00000d10: 3962 3836 6630 3138 6135 6563 6264 3233  9b86f018a5ecbd23
-00000d20: 3035 6136 3631 6666 6565 6533 3165 6565  05a661ffeee31eee
-00000d30: 3530 3537 6337 3762 3561 3762 3765 6561  5057c77b5a7b7eea
-00000d40: 3833 3933 3831 6236 3763 3636 3165 6434  839381b67c661ed4
-00000d50: 3665 3837 6430 6232 3137 3564 6163 6131  6e87d0b2175daca1
-00000d60: 3935 3766 6622 2c0d 0a20 2020 2022 6b65  957ff",..    "ke
-00000d70: 7922 3a20 2263 7265 6465 6e74 6961 6c73  y": "credentials
-00000d80: 2e6b 6579 2e70 7269 7661 7465 220d 0a7d  .key.private"..}
+00000000: 7b0a 2020 2020 2273 656c 6622 3a20 2268  {.    "self": "h
+00000010: 7474 7073 3a2f 2f74 3132 3334 352e 6375  ttps://t12345.cu
+00000020: 6d75 6c6f 6369 7479 2e63 6f6d 2f74 656e  mulocity.com/ten
+00000030: 616e 742f 6f70 7469 6f6e 732f 6a77 742f  ant/options/jwt/
+00000040: 6372 6564 656e 7469 616c 732e 6b65 792e  credentials.key.
+00000050: 7072 6976 6174 6522 2c0a 2020 2020 2263  private",.    "c
+00000060: 6174 6567 6f72 7922 3a20 226a 7774 222c  ategory": "jwt",
+00000070: 0a20 2020 2022 7661 6c75 6522 3a20 2263  .    "value": "c
+00000080: 3663 3834 6333 3361 3937 3930 3836 3262  6c84c33a9790862b
+00000090: 3362 6536 3036 3535 3635 3962 3764 3538  3be60655659b7d58
+000000a0: 6139 3939 3162 6339 3564 3337 6635 6663  a9991bc95d37f5fc
+000000b0: 3137 3839 3263 3431 3538 6233 3338 3563  17892c4158b3385c
+000000c0: 3230 6631 3633 6365 3734 3234 6333 6361  20f163ce7424c3ca
+000000d0: 3564 3437 3138 3637 6133 6434 6361 6133  5d471867a3d4caa3
+000000e0: 3339 3935 6563 3832 3639 3837 3165 3330  3995ec8269871e30
+000000f0: 6635 6431 3035 3739 6662 3866 3036 6237  f5d10579fb8f06b7
+00000100: 6239 3862 3737 3464 6165 6339 6561 6232  b98b774daec9eab2
+00000110: 3937 6462 3136 3664 3336 6235 3462 6364  97db166d36b54bcd
+00000120: 3834 3861 3236 3562 6231 3632 3963 3334  848a265bb1629c34
+00000130: 3134 6537 3934 3534 6136 6564 6166 6331  14e79454a6edafc1
+00000140: 6535 3562 3037 3033 3233 6434 3936 3561  e55b070323d4965a
+00000150: 3965 3736 3965 6236 6266 6663 3262 3164  9e769eb6bffc2b1d
+00000160: 6139 6433 3438 6135 3837 6165 3133 6631  a9d348a587ae13f1
+00000170: 3535 6530 3566 3564 3265 3964 6662 6261  55e05f5d2e9dfbba
+00000180: 3663 6333 3864 3935 6366 3030 3736 3865  6cc38d95cf00768e
+00000190: 6562 6132 6431 3438 3862 3766 3064 3033  eba2d1488b7f0d03
+000001a0: 6434 3634 3265 6435 3062 6431 3534 3632  d4642ed50bd15462
+000001b0: 6364 3065 3339 3738 6534 3933 6565 3466  cd0e3978e493ee4f
+000001c0: 3538 3236 3736 3536 3566 3939 3035 3764  582676565f99057d
+000001d0: 6531 3933 6238 6438 3139 6362 3930 3936  e193b8d819cb9096
+000001e0: 6234 3838 3132 6332 3936 6630 3532 6230  b48812c296f052b0
+000001f0: 3263 3239 6534 6331 3036 3061 6161 3336  2c29e4c1060aaa36
+00000200: 6538 6262 6331 6138 3731 3134 6566 6439  e8bbc1a87114efd9
+00000210: 3666 3266 3163 3432 6362 6366 3032 3937  6f2f1c42cbcf0297
+00000220: 3535 3135 6364 3836 3433 6265 3433 6463  5515cd8643be43dc
+00000230: 3239 3136 3465 3135 3738 6261 3232 3361  29164e1578ba223a
+00000240: 6531 6261 6536 3437 3730 3261 6163 6365  e1bae647702aacce
+00000250: 3436 3738 3839 3363 3564 3663 3439 3335  4678893c5d6c4935
+00000260: 6662 3864 6265 6532 3563 3430 3831 6539  fb8dbee25c4081e9
+00000270: 3761 3937 6365 3937 3634 6231 3630 6433  7a97ce9764b160d3
+00000280: 6638 6330 3731 3037 3666 3765 6462 3031  f8c071076f7edb01
+00000290: 3737 3735 3963 3061 3430 3633 3333 6632  77759c0a406333f2
+000002a0: 3733 3736 3331 3639 6464 3439 3561 3235  73763169dd495a25
+000002b0: 3566 3934 3838 6165 3435 6535 6237 3965  5f9488ae45e5b79e
+000002c0: 3333 3838 6633 3738 6364 3361 6263 6339  3388f378cd3abcc9
+000002d0: 3332 3335 3230 6236 6236 3338 3966 6430  323520b6b6389fd0
+000002e0: 6365 6261 6165 6335 3363 6132 3236 6131  cebaaec53ca226a1
+000002f0: 3730 3862 6433 3935 6635 6132 6133 3934  708bd395f5a2a394
+00000300: 3632 6636 6435 3332 3037 3661 3061 3530  62f6d532076a0a50
+00000310: 6464 6637 6137 3630 3539 3561 3662 3630  ddf7a760595a6b60
+00000320: 6636 6164 3832 3634 6162 6132 3738 6331  f6ad8264aba278c1
+00000330: 3839 3334 3161 6662 3137 6138 3837 3935  89341afb17a88795
+00000340: 3465 3431 6536 6437 3836 6137 3530 6430  4e41e6d786a750d0
+00000350: 3136 6438 3966 6334 3563 3834 3836 6538  16d89fc45c8486e8
+00000360: 3561 6130 6130 6263 6466 3638 6631 3139  5aa0a0bcdf68f119
+00000370: 6463 3035 3961 6233 3432 3736 6230 3338  dc059ab34276b038
+00000380: 3736 6431 3437 6139 6435 6536 6335 3863  76d147a9d5e6c58c
+00000390: 3262 6232 6262 3466 3035 3464 3862 3436  2bb2bb4f054d8b46
+000003a0: 3636 6531 6262 3138 6639 3534 3038 3962  66e1bb18f954089b
+000003b0: 6634 3465 3631 6431 6233 6663 6566 6432  f44e61d1b3fcefd2
+000003c0: 3336 3830 3830 6532 3330 3630 3635 3934  368080e230606594
+000003d0: 3934 6330 6239 6565 6336 3030 3832 6338  94c0b9eec60082c8
+000003e0: 6634 3537 3934 6531 3439 3531 3037 3461  f45794e14951074a
+000003f0: 3164 3334 6238 6565 6436 6637 3731 3263  1d34b8eed6f7712c
+00000400: 6464 6634 6264 3934 3435 6335 6336 6363  ddf4bd9445c5c6cc
+00000410: 3461 3763 3039 6437 3539 3632 6361 3738  4a7c09d75962ca78
+00000420: 3132 3238 3432 3065 6339 6636 3935 3930  1228420ec9f69590
+00000430: 6538 3962 3831 3733 3534 3835 3266 3164  e89b817354852f1d
+00000440: 6464 3337 3765 6434 6362 6661 3137 3836  dd377ed4cbfa1786
+00000450: 6231 3937 3431 3538 3361 6666 3363 6334  b19741583aff3cc4
+00000460: 3661 6535 6534 6363 3264 3065 3038 3531  6ae5e4cc2d0e0851
+00000470: 3533 3336 6538 3432 6636 6464 3130 6366  5336e842f6dd10cf
+00000480: 6231 6163 3263 3766 6465 3464 6666 6630  b1ac2c7fde4dfff0
+00000490: 6665 3439 3863 3961 3666 3236 6431 6135  fe498c9a6f26d1a5
+000004a0: 3862 3861 6165 3562 6632 6563 3631 3961  8b8aae5bf2ec619a
+000004b0: 3963 3435 6161 3462 3366 6431 3937 3937  9c45aa4b3fd19797
+000004c0: 6231 3732 3037 6238 3365 3462 6335 3535  b17207b83e4bc555
+000004d0: 3130 3362 6466 3437 3237 3837 6239 6134  103bdf472787b9a4
+000004e0: 6432 3933 3132 3533 6336 6235 3335 3634  d2931253c6b53564
+000004f0: 6635 3837 3537 6137 6261 3364 3866 6237  f58757a7ba3d8fb7
+00000500: 3037 3931 3037 3637 3634 6164 3762 3163  0791076764ad7b1c
+00000510: 3139 3935 6236 6230 3831 3830 3636 6361  1995b6b0818066ca
+00000520: 6233 3866 3037 3861 3134 3561 3036 6363  b38f078a145a06cc
+00000530: 6235 6161 6338 3639 6236 6631 6238 3630  b5aac869b6f1b860
+00000540: 3866 3838 6663 6131 3837 6635 3363 3831  8f88fca187f53c81
+00000550: 3861 3762 3832 3664 6330 3065 3962 6266  8a7b826dc00e9bbf
+00000560: 3231 6332 6132 3963 3764 3539 3934 3166  21c2a29c7d59941f
+00000570: 6365 3765 3066 6339 6435 3638 3065 6439  ce7e0fc9d5680ed9
+00000580: 3766 3362 6165 3265 3365 3531 6664 6337  7f3bae2e3e51fdc7
+00000590: 3232 3965 3661 3865 3531 6439 3834 3038  229e6a8e51d98408
+000005a0: 3933 3238 3239 6633 6436 6138 3462 6435  932829f3d6a84bd5
+000005b0: 6565 3833 6138 3963 3264 3633 6666 3461  ee83a89c2d63ff4a
+000005c0: 3334 3666 3432 3363 6265 6633 6264 3663  346f423cbef3bd6c
+000005d0: 3439 3235 6532 3235 6332 3965 6130 3939  4925e225c29ea099
+000005e0: 3864 3736 6139 6466 6364 6532 6436 3232  8d76a9dfcde2d622
+000005f0: 6133 3262 3862 6135 3235 6230 3234 3564  a32b8ba525b0245d
+00000600: 3864 3662 3266 6461 3130 3030 3032 6365  8d6b2fda100002ce
+00000610: 3166 3738 3732 3337 3439 3839 3039 6633  1f787237498909f3
+00000620: 3938 3838 3235 3138 3139 3063 6333 3664  98882518190cc36d
+00000630: 3032 6466 3363 3530 6431 3233 3030 6332  02df3c50d12300c2
+00000640: 3637 6466 3863 6364 3933 6663 6266 3962  67df8ccd93fcbf9b
+00000650: 6163 3037 3330 3264 3934 6431 3733 6636  ac07302d94d173f6
+00000660: 3665 3030 3937 3666 3461 6161 3338 3466  6e00976f4aaa384f
+00000670: 6438 3833 6264 6561 3638 3639 3034 3331  d883bdea68690431
+00000680: 6237 6166 3033 6136 3961 3338 6163 3432  b7af03a69a38ac42
+00000690: 3838 3533 3231 6239 6634 3032 3332 6138  885321b9f40232a8
+000006a0: 3138 3938 3965 3536 3430 6530 3331 3332  18989e5640e03132
+000006b0: 3962 3235 6461 6636 3866 3534 3166 3232  9b25daf68f541f22
+000006c0: 3835 6663 3963 3036 6166 3732 3462 3636  85fc9c06af724b66
+000006d0: 3032 3035 3266 3730 6362 3431 3031 3064  02052f70cb41010d
+000006e0: 3364 3238 3831 6235 3039 3834 3464 3537  3d2881b509844d57
+000006f0: 3531 3866 6264 3236 6536 3135 3136 3530  518fbd26e6151650
+00000700: 3939 3661 6664 3364 3262 3032 3261 3363  996afd3d2b022a3c
+00000710: 6232 6239 3361 3536 6239 6233 6237 6361  b2b93a56b9b3b7ca
+00000720: 3463 3038 3231 3361 3330 6465 6137 6431  4c08213a30dea7d1
+00000730: 3232 6536 6264 3238 6666 3936 3466 6232  22e6bd28ff964fb2
+00000740: 6566 3165 3065 6262 3561 3565 3862 6563  ef1e0ebb5a5e8bec
+00000750: 3234 3431 3433 6534 3233 6232 3861 6637  244143e423b28af7
+00000760: 6131 3533 6664 3861 3633 6363 6330 3830  a153fd8a63ccc080
+00000770: 6166 6438 6662 3762 3063 3838 3935 3930  afd8fb7b0c889590
+00000780: 3435 6163 3665 3932 3232 3466 6332 6232  45ac6e92224fc2b2
+00000790: 3861 6331 6362 3130 6133 6639 3432 3339  8ac1cb10a3f94239
+000007a0: 3261 3132 3464 3361 3437 3536 6139 6435  2a124d3a4756a9d5
+000007b0: 3366 6131 3863 3431 6636 3832 3335 3566  3fa18c41f682355f
+000007c0: 3037 3165 3833 3033 3166 3263 3331 3764  071e83031f2c317d
+000007d0: 3935 6633 6465 3465 3764 3339 3561 3661  95f3de4e7d395a6a
+000007e0: 6639 3566 3939 3364 6538 3561 3238 3864  f95f993de85a288d
+000007f0: 3361 6536 3639 3838 6566 6136 6237 3664  3ae66988efa6b76d
+00000800: 3937 3732 6462 6663 3362 3936 3734 3761  9772dbfc3b96747a
+00000810: 3935 3532 6666 6263 6362 3862 3630 3938  9552ffbccb8b6098
+00000820: 3138 3062 6464 3832 6466 3835 6162 6539  180bdd82df85abe9
+00000830: 3964 3537 6636 3338 3935 3233 3036 3261  9d57f6389523062a
+00000840: 3634 3834 3836 3866 6536 6231 3366 3964  6484868fe6b13f9d
+00000850: 3535 3739 6461 6438 6138 3134 3665 3137  5579dad8a8146e17
+00000860: 3733 6238 6238 6561 6335 6137 6165 6532  73b8b8eac5a7aee2
+00000870: 6163 6363 3065 3139 3434 6535 6337 3739  accc0e1944e5c779
+00000880: 6132 3136 6364 3734 3966 6632 6263 3332  a216cd749ff2bc32
+00000890: 6135 3564 6437 3733 6337 3530 6666 6465  a55dd773c750ffde
+000008a0: 3636 3035 3561 3461 3339 3866 3063 3130  66055a4a398f0c10
+000008b0: 3563 6131 6332 3766 3034 6431 3962 3431  5ca1c27f04d19b41
+000008c0: 6163 6261 3936 3737 6239 6161 3764 6631  acba9677b9aa7df1
+000008d0: 6337 3762 3732 6263 3634 3163 6133 3366  c77b72bc641ca33f
+000008e0: 3162 6263 3365 3961 6164 3734 3163 6437  1bbc3e9aad741cd7
+000008f0: 3638 3432 6235 3635 6434 3465 3037 3137  6842b565d44e0717
+00000900: 6364 3164 3164 6330 3034 6434 6239 3236  cd1d1dc004d4b926
+00000910: 3535 3133 6435 6666 6263 6530 3061 3936  5513d5ffbce00a96
+00000920: 3564 3862 3233 3965 3436 6563 3632 6162  5d8b239e46ec62ab
+00000930: 6430 6331 3836 3839 3633 3865 3465 6438  d0c18689638e4ed8
+00000940: 3138 6135 6666 6135 3432 3030 3761 3036  18a5ffa542007a06
+00000950: 3838 3565 3832 6236 3939 3437 6465 6237  885e82b69947deb7
+00000960: 6233 3636 3461 6234 3736 3335 3538 3161  b3664ab47635581a
+00000970: 3962 6465 6137 6638 3439 3936 3837 6633  9bdea7f8499687f3
+00000980: 6236 3465 3335 3561 3735 3336 3062 3630  b64e355a75360b60
+00000990: 3735 6462 3433 6366 3338 3965 3936 3436  75db43cf389e9646
+000009a0: 3931 6666 3833 3837 3562 3536 3631 3532  91ff83875b566152
+000009b0: 6531 6239 3964 3735 3835 3031 3332 6334  e1b99d75850132c4
+000009c0: 6531 3334 3264 6132 3231 6430 3831 3738  e1342da221d08178
+000009d0: 6239 6462 3666 6663 6239 6163 3230 6564  b9db6ffcb9ac20ed
+000009e0: 3262 3935 6639 3765 6536 3332 6132 6430  2b95f97ee632a2d0
+000009f0: 3934 3464 6363 3636 3239 3439 6435 3161  944dcc662949d51a
+00000a00: 3134 3562 3934 3830 3635 3266 6533 6564  145b9480652fe3ed
+00000a10: 3965 3137 3638 6663 3461 3934 6434 6664  9e1768fc4a94d4fd
+00000a20: 3437 6362 6266 3035 3432 6565 6135 3130  47cbbf0542eea510
+00000a30: 3332 6364 3836 6432 3538 3132 3234 3563  32cd86d25812245c
+00000a40: 6362 3939 6436 6635 6365 6436 3739 3733  cb99d6f5ced67973
+00000a50: 3739 6266 6537 3662 3638 3263 6135 6262  79bfe76b682ca5bb
+00000a60: 3735 3761 3135 3239 6337 3337 6461 6635  757a1529c737daf5
+00000a70: 3064 3435 3335 3262 3536 3039 6266 3236  0d45352b5609bf26
+00000a80: 6465 6233 3135 3637 3834 6338 3635 6665  deb3156784c865fe
+00000a90: 3435 6464 6565 6437 3832 3532 3837 3662  45ddeed78252876b
+00000aa0: 6465 3538 3662 6138 3635 6665 3238 3539  de586ba865fe2859
+00000ab0: 3832 3031 6661 3638 3734 6130 3463 6333  8201fa6874a04cc3
+00000ac0: 6336 6131 3762 6161 3137 6232 3464 6265  c6a17baa17b24dbe
+00000ad0: 6566 3831 3934 3866 3765 6337 6236 3033  ef81948f7ec7b603
+00000ae0: 3164 3463 3538 3631 6534 3630 3937 6239  1d4c5861e46097b9
+00000af0: 3536 3838 3636 3235 3261 3933 3536 3235  568866252a935625
+00000b00: 3464 3130 3633 3837 3236 3963 3730 3233  4d106387269c7023
+00000b10: 3839 3164 6536 3666 3336 3862 6135 3161  891de66f368ba51a
+00000b20: 3162 6330 3766 3434 3633 3437 3539 3334  1bc07f4463475934
+00000b30: 6338 3933 3031 6564 3664 3365 3865 3832  c89301ed6d3e8e82
+00000b40: 6538 3564 3237 6339 6465 6362 3466 3737  e85d27c9decb4f77
+00000b50: 6238 3036 3931 3830 6166 3934 6666 3630  b8069180af94ff60
+00000b60: 6533 6366 6265 6331 3763 6165 3731 3031  e3cfbec17cae7101
+00000b70: 6564 6130 6461 6331 3530 3664 6662 3136  eda0dac1506dfb16
+00000b80: 6237 3835 3166 6335 6138 6436 6265 3961  b7851fc5a8d6be9a
+00000b90: 3065 3637 6434 6233 3365 6663 3466 3531  0e67d4b33efc4f51
+00000ba0: 3735 6631 3135 3337 6465 3763 3833 6663  75f11537de7c83fc
+00000bb0: 3033 3936 3539 6666 6164 6632 6633 6234  039659ffadf2f3b4
+00000bc0: 3035 6635 3136 6462 3332 6165 3561 6134  05f516db32ae5aa4
+00000bd0: 6631 3530 3166 6233 6532 6237 6234 3033  f1501fb3e2b7b403
+00000be0: 3464 3139 3761 3063 3537 6631 3239 3833  4d197a0c57f12983
+00000bf0: 3333 6562 6534 3262 3865 3432 3938 3930  33ebe42b8e429890
+00000c00: 3861 3366 6332 3061 3561 6439 3432 6238  8a3fc20a5ad942b8
+00000c10: 3063 6461 3133 3733 6139 3530 3336 6537  0cda1373a95036e7
+00000c20: 3361 3938 3535 3630 3039 3432 3437 6465  3a985560094247de
+00000c30: 3634 3538 3337 3166 3631 3538 6562 6364  6458371f6158ebcd
+00000c40: 6164 3739 6433 3538 6630 3232 3839 6331  ad79d358f02289c1
+00000c50: 3437 3238 3434 3533 3266 3132 3736 6437  472844532f1276d7
+00000c60: 6437 6262 3536 6266 6133 3663 3935 3566  d7bb56bfa36c955f
+00000c70: 3239 3061 6236 6461 3432 6363 3838 6365  290ab6da42cc88ce
+00000c80: 3135 6366 6337 3333 3631 6232 3366 3032  15cfc73361b23f02
+00000c90: 3031 3831 6334 3034 3635 3538 6536 6335  0181c4046558e6c5
+00000ca0: 3465 3963 3337 3964 6461 3266 3964 3930  4e9c379dda2f9d90
+00000cb0: 6262 3730 6561 3661 6338 3565 6133 3138  bb70ea6ac85ea318
+00000cc0: 3138 3366 6661 6636 3861 3361 3433 3633  183ffaf68a3a4363
+00000cd0: 3033 3663 6431 6363 6339 3463 3130 6438  036cd1ccc94c10d8
+00000ce0: 6564 6131 3430 3933 3035 6366 3966 6336  eda1409305cf9fc6
+00000cf0: 3033 3534 3430 3064 6534 3864 6530 3539  0354400de48de059
+00000d00: 3662 3366 3335 6439 3631 3134 6439 6238  6b3f35d96114d9b8
+00000d10: 3666 3031 3861 3565 6362 6432 3330 3561  6f018a5ecbd2305a
+00000d20: 3636 3166 6665 6565 3331 6565 6535 3035  661ffeee31eee505
+00000d30: 3763 3737 6235 6137 6237 6565 6138 3339  7c77b5a7b7eea839
+00000d40: 3338 3162 3637 6336 3631 6564 3436 6538  381b67c661ed46e8
+00000d50: 3764 3062 3231 3735 6461 6361 3139 3537  7d0b2175daca1957
+00000d60: 6666 222c 0a20 2020 2022 6b65 7922 3a20  ff",.    "key": 
+00000d70: 2263 7265 6465 6e74 6961 6c73 2e6b 6579  "credentials.key
+00000d80: 2e70 7269 7661 7465 220a 7d              .private".}
```

### Comparing `c8y_api-1.7/tests/model/test_alarm.py` & `c8y_api-1.8/tests/model/test_alarm.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_application.py` & `c8y_api-1.8/tests/model/test_application.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_audit.py` & `c8y_api-1.8/tests/model/test_audit.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_base.py` & `c8y_api-1.8/tests/model/test_base.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_bulk_operation.py` & `c8y_api-1.8/tests/model/test_bulk_operation.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_device.py` & `c8y_api-1.8/tests/model/test_device.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_event.py` & `c8y_api-1.8/tests/model/test_event.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_global_role.py` & `c8y_api-1.8/tests/model/test_global_role.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_inventory.py` & `c8y_api-1.8/tests/model/test_inventory.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_inventoryrole.py` & `c8y_api-1.8/tests/model/test_inventoryrole.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_managedobject.py` & `c8y_api-1.8/tests/model/test_managedobject.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_operation.py` & `c8y_api-1.8/tests/model/test_operation.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_parser.py` & `c8y_api-1.8/tests/model/test_parser.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_resource.py` & `c8y_api-1.8/tests/model/test_resource.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/test_subscription.py` & `c8y_api-1.8/tests/model/test_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     updated_subscription = subscription.create()
 
     # 1) to_json should have been called
     assert subscription.to_json.call_count == 1
     # 2) the given resource path should be correct
     resource = isolate_last_call_arg(c8y.post, 'resource', 0)
-    assert resource == f'notification2/subscriptions'
+    assert resource == f'/notification2/subscriptions'
     # 3) the given payload should match what to_json returned
     payload = isolate_last_call_arg(c8y.post, 'json', 1)
     assert set(payload.keys()) == {'expected'}
     # 4) the return should be parsed properly
     assert updated_subscription.name == sample_json['subscription']
     assert updated_subscription.context == sample_json['context']
     assert updated_subscription.source_id == sample_json['source']['id']
@@ -102,9 +102,9 @@
     subscription.id = 'subscription-id'
 
     subscription.delete()
 
     assert c8y.delete.call_count == 1
     # 2) the given resource path should be correct
     resource = isolate_last_call_arg(c8y.delete, 'resource', 0)
-    assert resource == f'notification2/subscriptions/{subscription.id}'
+    assert resource == f'/notification2/subscriptions/{subscription.id}'
```

### Comparing `c8y_api-1.7/tests/model/test_tenant_option.py` & `c8y_api-1.8/tests/model/test_tenant_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     updated_option = sample_option.create()
 
     # 1) to_json should have been called
     assert sample_option.to_json.call_count == 1
     # 2) the given resource path should be correct
     resource = isolate_last_call_arg(c8y.post, 'resource', 0)
-    assert resource == f'tenant/options'
+    assert resource == f'/tenant/options'
     # 3) the given payload should match what to_json returned
     payload = isolate_last_call_arg(c8y.post, 'json', 1)
     assert set(payload.keys()) == {'expected'}
     # 4) the return should be parsed properly
     assert updated_option.key == sample_json['key']
     assert updated_option.category == sample_json['category']
     assert updated_option.value == sample_json['value']
@@ -118,15 +118,15 @@
 
     # 1) to_json should have been called
     assert sample_option.to_json.call_count == 1
     only_updated = isolate_last_call_arg(sample_option.to_json, 'only_updated', 0)
     assert only_updated
     # 2) the given resource path should be correct
     resource = isolate_last_call_arg(c8y.put, 'resource', 0)
-    assert resource == f'tenant/options/{sample_option.category}/{sample_option.key}'
+    assert resource == f'/tenant/options/{sample_option.category}/{sample_option.key}'
     # 3) the given payload should match what to_json returned
     payload = isolate_last_call_arg(c8y.put, 'json', 1)
     assert set(payload.keys()) == {'expected'}
     # 4) the response should be parsed
     assert result.key == sample_json['key']
     assert result.category == sample_json['category']
     assert result.value == sample_json['value']
```

### Comparing `c8y_api-1.7/tests/model/test_user.py` & `c8y_api-1.8/tests/model/test_user.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/model/user.json` & `c8y_api-1.8/tests/model/user.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/test_app.py` & `c8y_api-1.8/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/test_auth.py` & `c8y_api-1.8/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/test_base_api.py` & `c8y_api-1.8/tests/test_base_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/test_device_registry.py` & `c8y_api-1.8/tests/test_device_registry.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/test_util.py` & `c8y_api-1.8/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.7/tests/utils.py` & `c8y_api-1.8/tests/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 # and/or its subsidiaries and/or its affiliates and/or their licensors.
 # Use, reproduction, transfer, publication or disclosure is prohibited except
 # as specifically provided for in your License Agreement with Software AG.
 
 from __future__ import annotations
 
 import base64
-import random
-import re
 from typing import List, Set, Any
 from unittest.mock import Mock
 
 import jwt
 import pytest
-from requests import request
 
 from c8y_api.model._base import CumulocityObject
 
+from testing_util import RandomNameGenerator
+
 
 def get_ids(objs: List[CumulocityObject]) -> Set[str]:
     """Isolate the ID from a list of database objects."""
     return {o.id for o in objs}
 
 
 def isolate_last_call_arg(mock: Mock, name: str, pos: int = None) -> Any:
@@ -82,51 +81,14 @@
 
 @pytest.fixture(scope='function')
 def random_name() -> str:
     """Provide a random name."""
     return RandomNameGenerator.random_name()
 
 
-def read_webcontent(source_url, target_path):
-    """Read web content to a local file."""
-    response = request('get', source_url)
-    if 200 <= response.status_code <= 299:
-        with open(target_path, 'wt', encoding='utf-8') as file:
-            file.write(response.text)
-    else:
-        raise RuntimeError('Unable to read web content. Unexpected response from web site: '
-                           f'HTTP {response.status_code} {response.text}')
-
-
-class RandomNameGenerator:
-    """Provides randomly generated names using a public service."""
-
-    wordlist_path = 'wordlist.txt'
-    read_webcontent('https://raw.githubusercontent.com/mike-hearn/useapassphrase/master/js/wordlist.js',
-                    wordlist_path)
-    with open(wordlist_path, 'rt', encoding='utf-8') as file:
-        file.readline()  # skip first line
-        lines = file.readlines()
-    words = [re.sub('[^\\w]', '', line) for line in lines]
-
-    @classmethod
-    def random_name(cls, num: int = 3, sep: str = '_') -> str:
-        """Generate a readable random name from joined random words.
-
-        Args:
-            num (int):  number of random words to concactenate
-            sep (str):  concatenation separator
-
-        Returns:
-            The generated name
-        """
-        words = [random.choice(cls.words) for _ in range(0, num)]
-        return sep.join(words)
-
-
 def b64encode(auth_string: str) -> str:
     """Encode a string with base64. This uses UTF-8 encoding."""
     return base64.b64encode(auth_string.encode('utf-8')).decode('utf-8')
 
 
 def build_auth_string(auth_value: str) -> str:
     """Build a complete auth string from an base64 encoded auth value.
```

### Comparing `c8y_api-1.7/util/microservice_util.py` & `c8y_api-1.8/util/microservice_util.py`

 * *Files identical despite different names*

