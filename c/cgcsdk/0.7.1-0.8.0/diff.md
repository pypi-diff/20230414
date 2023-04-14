# Comparing `tmp/cgcsdk-0.7.1.tar.gz` & `tmp/cgcsdk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-0.7.1.tar", last modified: Thu Mar 23 11:27:00 2023, max compression
+gzip compressed data, was "cgcsdk-0.8.0.tar", last modified: Fri Apr 14 14:29:17 2023, max compression
```

## Comparing `cgcsdk-0.7.1.tar` & `cgcsdk-0.8.0.tar`

### file list

```diff
@@ -1,87 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 11:27:00.000431 cgcsdk-0.7.1/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.7.1/LICENSE
--rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2023-03-23 11:26:59.998427 cgcsdk-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.762540 cgcsdk-0.7.1/cgc/
--rw-rw-rw-   0        0        0      234 2023-03-23 10:58:35.000000 cgcsdk-0.7.1/cgc/.env
--rw-rw-rw-   0        0        0     2806 2023-03-23 11:23:45.000000 cgcsdk-0.7.1/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      324 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/__init__.py
--rw-rw-rw-   0        0        0     1089 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.781998 cgcsdk-0.7.1/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.7.1/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.805698 cgcsdk-0.7.1/cgc/commands/auth/
--rw-rw-rw-   0        0        0      265 2023-02-17 10:02:49.000000 cgcsdk-0.7.1/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     2428 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1202 2023-02-17 10:49:54.000000 cgcsdk-0.7.1/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     3922 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.826089 cgcsdk-0.7.1/cgc/commands/billing/
--rw-rw-rw-   0        0        0      751 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     3444 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1946 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4695 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     1347 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     2121 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/cgc_cmd_responses.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.849818 cgcsdk-0.7.1/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0     7539 2023-03-08 16:34:19.000000 cgcsdk-0.7.1/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0      678 2023-03-09 13:37:16.000000 cgcsdk-0.7.1/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     4501 2023-02-17 10:02:49.000000 cgcsdk-0.7.1/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     3290 2023-03-09 09:10:46.000000 cgcsdk-0.7.1/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.857230 cgcsdk-0.7.1/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      381 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.871478 cgcsdk-0.7.1/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.7.1/cgc/config.py
--rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.876625 cgcsdk-0.7.1/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.7.1/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     2956 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.881419 cgcsdk-0.7.1/cgc/tests/
--rw-rw-rw-   0        0        0   102691 2023-03-22 14:29:23.000000 cgcsdk-0.7.1/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.909198 cgcsdk-0.7.1/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.7.1/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.7.1/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.7.1/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.7.1/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.7.1/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.7.1/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.7.1/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9172 2023-03-22 11:24:32.000000 cgcsdk-0.7.1/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.933397 cgcsdk-0.7.1/cgc/utils/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.7.1/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.7.1/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2560 2023-02-17 10:02:49.000000 cgcsdk-0.7.1/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.941857 cgcsdk-0.7.1/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.7.1/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1318 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1122 2023-03-23 11:15:14.000000 cgcsdk-0.7.1/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.960219 cgcsdk-0.7.1/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.7.1/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.7.1/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.7.1/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.7.1/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.7.1/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.7.1/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.7.1/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     1973 2023-02-15 11:40:43.000000 cgcsdk-0.7.1/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     4727 2023-03-23 11:24:38.000000 cgcsdk-0.7.1/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.7.1/cgc/utils/update.py
--rw-rw-rw-   0        0        0     2958 2023-03-08 10:41:28.000000 cgcsdk-0.7.1/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2023-03-23 11:26:59.993643 cgcsdk-0.7.1/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1101 2023-03-23 11:26:59.000000 cgcsdk-0.7.1/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2194 2023-03-23 11:26:59.000000 cgcsdk-0.7.1/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 11:26:59.000000 cgcsdk-0.7.1/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-03-23 11:26:59.000000 cgcsdk-0.7.1/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       94 2023-03-23 11:26:59.000000 cgcsdk-0.7.1/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-23 11:26:59.000000 cgcsdk-0.7.1/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-23 11:27:00.000878 cgcsdk-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     2061 2023-02-15 12:56:02.000000 cgcsdk-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.576294 cgcsdk-0.8.0/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2023-04-14 14:29:17.574677 cgcsdk-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.314630 cgcsdk-0.8.0/cgc/
+-rw-rw-rw-   0        0        0      234 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/.env
+-rw-rw-rw-   0        0        0     3021 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      435 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1253 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.323543 cgcsdk-0.8.0/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.334739 cgcsdk-0.8.0/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      265 2023-02-17 10:02:49.000000 cgcsdk-0.8.0/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     2371 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1202 2023-02-17 10:49:54.000000 cgcsdk-0.8.0/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     3922 2023-03-22 14:29:23.000000 cgcsdk-0.8.0/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.343461 cgcsdk-0.8.0/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     1353 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     1995 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/cgc_cmd_responses.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.372502 cgcsdk-0.8.0/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0     4275 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      883 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5189 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.379463 cgcsdk-0.8.0/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     2592 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.386932 cgcsdk-0.8.0/cgc/commands/debug/
+-rw-rw-rw-   0        0        0        0 2023-03-22 14:29:23.000000 cgcsdk-0.8.0/cgc/commands/debug/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.393573 cgcsdk-0.8.0/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     4413 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/commands/resource/resource_cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.412750 cgcsdk-0.8.0/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.0/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.0/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/config.py
+-rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.420110 cgcsdk-0.8.0/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3187 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.429987 cgcsdk-0.8.0/cgc/tests/
+-rw-rw-rw-   0        0        0   102745 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.470327 cgcsdk-0.8.0/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.0/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.0/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.512619 cgcsdk-0.8.0/cgc/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.0/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2560 2023-02-17 10:02:49.000000 cgcsdk-0.8.0/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.526651 cgcsdk-0.8.0/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1122 2023-03-23 11:15:14.000000 cgcsdk-0.8.0/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.546520 cgcsdk-0.8.0/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.0/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.0/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.0/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.0/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     1973 2023-02-15 11:40:43.000000 cgcsdk-0.8.0/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     4727 2023-03-23 11:24:38.000000 cgcsdk-0.8.0/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.0/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     2958 2023-03-08 10:41:28.000000 cgcsdk-0.8.0/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:29:17.570329 cgcsdk-0.8.0/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     1101 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2320 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       94 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 14:29:17.000000 cgcsdk-0.8.0/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:29:17.576800 cgcsdk-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     2061 2023-02-15 12:56:02.000000 cgcsdk-0.8.0/setup.py
```

### Comparing `cgcsdk-0.7.1/PKG-INFO` & `cgcsdk-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.7.1
+Version: 0.8.0
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.7.1/cgc/CHANGELOG.md` & `cgcsdk-0.8.0/cgc/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Change Log
 
+## 0.8.0
+
+Release on Apr 14, 2023.
+
+* cgc db - new commands for managing databases
+* cgc compute - refactor commands for compute template management
+* cgc resource - new command to control db and compute resources
+
 ## 0.7.1
 
 Released on Mar 23, 2023.
 
 * endpoints can be disabled on server, client correctly understand error code 302
 * api-keys management endpoints are temporary disabled (list, delete)
```

### Comparing `cgcsdk-0.7.1/cgc/cgc.py` & `cgcsdk-0.8.0/cgc/cgc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import click
 from cgc.commands.volume.volume_cmd import volume_group
 from cgc.commands.compute.compute_cmd import compute_group
 from cgc.commands.billing.billing_cmd import billing_group
+from cgc.commands.db.db_cmd import db_group
+from cgc.commands.resource.resource_cmd import resource_group
 from cgc.commands.auth.auth_cmd import (
     api_keys_group,
     auth_register,
 )
 from cgc.commands.debug.debug_cmd import debug_group
 from cgc.commands.cgc_cmd import cgc_rm, cgc_status, sending_telemetry_permission
 from cgc.utils.version_control import check_version, get_version
@@ -19,14 +21,16 @@
     check_version()
 
 
 cli.add_command(auth_register)
 cli.add_command(api_keys_group)
 cli.add_command(volume_group)
 cli.add_command(compute_group)
+cli.add_command(db_group)
+cli.add_command(resource_group)
 cli.add_command(billing_group)
 cli.add_command(cgc_rm)
 cli.add_command(cgc_status)
 cli.add_command(debug_group)
 cli.add_command(sending_telemetry_permission)
```

### Comparing `cgcsdk-0.7.1/cgc/commands/auth/auth_cmd.py` & `cgcsdk-0.8.0/cgc/commands/auth/auth_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 )
 
 from cgc.utils.prepare_headers import get_url_and_prepare_headers_register
 from cgc.utils.cryptography import rsa_crypto
 from cgc.utils.click_group import CustomCommand, CustomGroup
 from cgc.utils.requests_helper import call_api, EndpointTypes
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
-from cgc.telemetry.basic import telemetry_permission_set
 
 
 @click.group("api-keys", cls=CustomGroup)
 def api_keys_group():
     """
     Management of API keys.
     """
```

### Comparing `cgcsdk-0.7.1/cgc/commands/auth/auth_responses.py` & `cgcsdk-0.8.0/cgc/commands/auth/auth_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/commands/auth/auth_utils.py` & `cgcsdk-0.8.0/cgc/commands/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/commands/billing/__init__.py` & `cgcsdk-0.8.0/cgc/commands/billing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 
 class NoVolumeStopEvents(BillingCommandException):
     def __init__(self) -> None:
         super().__init__("No volume stop events to list.")
 
 
-class NoComputeStopEvents(BillingCommandException):
+class NoResourceStopEvents(BillingCommandException):
     def __init__(self) -> None:
-        super().__init__("No compute stop events to list.")
+        super().__init__("No resource stop events to list.")
```

### Comparing `cgcsdk-0.7.1/cgc/commands/billing/billing_cmd.py` & `cgcsdk-0.8.0/cgc/commands/billing/billing_cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 
 from cgc.commands.billing.billing_utils import verify_input_datetime
 from cgc.commands.billing.billing_responses import (
     billing_status_response,
     billing_invoice_response,
-    stop_events_compute_response,
+    stop_events_resource_response,
     stop_events_volume_response,
 )
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.utils.click_group import CustomGroup, CustomCommand
 from cgc.utils.requests_helper import call_api, EndpointTypes
 
@@ -62,25 +62,25 @@
 def stop_events_group():
     """
     List stop events information.
     """
     pass
 
 
-@stop_events_group.command("compute")
+@stop_events_group.command("resource")
 @click.option("--date_from", "-f", "date_from", prompt="Date from (DD-MM-YYYY)")
 @click.option("--date_to", "-t", "date_to", prompt="Date to (DD-MM-YYYY)")
-def stop_events_compute(date_from, date_to):
+def stop_events_resource(date_from, date_to):
     verify_input_datetime(date_from, date_to)
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/billing/list_compute_stop_events?time_from={date_from}&time_till={date_to}"
-    metric = "billing.stop_events.compute"
+    url = f"{api_url}/v1/api/billing/list_resource_stop_events?time_from={date_from}&time_till={date_to}"
+    metric = "billing.stop_events.resource"
     __res = call_api(request=EndpointTypes.get, url=url, headers=headers)
     click.echo(
-        stop_events_compute_response(
+        stop_events_resource_response(
             retrieve_and_validate_response_send_metric(__res, metric)
         )
     )
 
 
 @stop_events_group.command("volume")
 @click.option("--date_from", "-f", "date_from", prompt="Date from (DD-MM-YYYY)")
```

### Comparing `cgcsdk-0.7.1/cgc/commands/billing/billing_responses.py` & `cgcsdk-0.8.0/cgc/commands/billing/billing_responses.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import calendar
 from cgc.commands.billing import (
     NoCostsFound,
     NoInvoiceFoundForSelectedMonth,
-    NoComputeStopEvents,
+    NoResourceStopEvents,
     NoVolumeStopEvents,
 )
 from cgc.commands.billing.billing_utils import (
     get_billing_status_message,
     get_table_compute_stop_events_message,
     get_table_volume_stop_events_message,
 )
@@ -36,18 +36,18 @@
         raise NoInvoiceFoundForSelectedMonth(year, month)
     message = get_billing_status_message(users_invoices_list)
     message += f"Total cost for namespace {namespace} in {calendar.month_name[month]} {year}: {total_cost:.2f} pln"
     return message
 
 
 @key_error_decorator_for_helpers
-def stop_events_compute_response(data: dict) -> str:
+def stop_events_resource_response(data: dict) -> str:
     event_list = data["details"]["event_list"]
     if not event_list:
-        raise NoComputeStopEvents()
+        raise NoResourceStopEvents()
     return get_table_compute_stop_events_message(event_list)
 
 
 @key_error_decorator_for_helpers
 def stop_events_volume_response(data: dict) -> str:
     event_list = data["details"]["event_list"]
     if not event_list:
```

### Comparing `cgcsdk-0.7.1/cgc/commands/billing/billing_utils.py` & `cgcsdk-0.8.0/cgc/commands/billing/billing_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         rent_start = cost["rent_start"]
         rent_end = cost["rent_end"]
         rent_time = f"{int(cost['rent_time'])} s"
         rent_cost = f"{float(cost['cost_total']):.2f} pln"
         resources = cost["resources"]
         name = resources["name"]
         rent_type = cost["type"]
-        if rent_type == "events_compute":
+        if rent_type == "events_resource":
             entity = resources["entity"]
         elif rent_type == "events_volume":
             entity = "volume"
         else:
             entity = "ERROR"
         total_user_cost += float(cost["cost_total"])
         row_list = [entity, name, rent_start, rent_end, rent_time, rent_cost]
```

### Comparing `cgcsdk-0.7.1/cgc/commands/cgc_cmd.py` & `cgcsdk-0.8.0/cgc/commands/cgc_cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import click
 from cgc.commands.cgc_cmd_responses import cgc_status_response
-from cgc.commands.compute.compute_cmd import compute_delete
+from cgc.commands.resource.resource_cmd import resource_delete
 from cgc.utils.requests_helper import call_api, EndpointTypes
 from cgc.utils.click_group import CustomCommand
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.telemetry.basic import telemetry_permission_set
 
 
 @click.command("rm", cls=CustomCommand)
 @click.argument("name", type=click.STRING)
 def cgc_rm(name: str):
     """
     Delete an app in user namespace
     """
-    compute_delete(name)
+    resource_delete(name)
 
 
 @click.command("status", cls=CustomCommand)
 def cgc_status():
     """Lists available and used resources"""
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/compute/status"
-    metric = "compute.status"
+    url = f"{api_url}/v1/api/resource/status"
+    metric = "resource.status"
     __res = call_api(
         request=EndpointTypes.get,
         url=url,
         headers=headers,
     )
     click.echo(
         cgc_status_response(retrieve_and_validate_response_send_metric(__res, metric))
```

### Comparing `cgcsdk-0.7.1/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-0.8.0/cgc/commands/cgc_cmd_responses.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,56 +17,53 @@
     list_headers = ["Resource", "Type", "Available", "Limit"]
     resource_names = [
         "CPU",
         "RAM",
         "GPU",
         "-",
         "-",
-        "-",
+        # "-",
         "Volume",
         "Storage",
         "-",
         "-",
-        "-",
     ]
     types = [
         "",
         "",
         "",
         "A100",
         "A5000",
         # "V100",
         "Count",
         "",
-        "cpu-nvme",
-        "cpu-ssd",
-        "gpu-nvme",
+        "nvme",
+        "ssd",
     ]
     resource_keys = [
         "limits.cpu",
         "limits.memory",
         "requests.nvidia.com/gpu",
         "comtegra.cloud/a100",
         "comtegra.cloud/a5000",
         # "comtegra.cloud/v100",
         "persistentvolumeclaims",
         "requests.storage",
-        "compute-nvme-rwx.storageclass.storage.k8s.io/requests.storage",
-        "compute-ssd-rwx.storageclass.storage.k8s.io/requests.storage",
-        "gpu-nvme-rwx.storageclass.storage.k8s.io/requests.storage",
+        "nvme-rwx.storageclass.storage.k8s.io/requests.storage",
+        "ssd-rwx.storageclass.storage.k8s.io/requests.storage",
     ]
 
     resources_available_list = []
     resources_limits_list = []
     for key in resource_keys:
         available = resources_available[key]
         limit = resources_limits[key]
         if "storage" in key or "memory" in key:
-            available = f"{available} GiB"
-            limit = f"{limit} GiB"
+            available = f"{available} Gb"
+            limit = f"{limit} Gb"
         else:
             available = int(available)
             limit = int(limit)
         resources_available_list.append(available)
         resources_limits_list.append(limit)
 
     return tabulate(
```

### Comparing `cgcsdk-0.7.1/cgc/commands/compute/compute_cmd.py` & `cgcsdk-0.8.0/cgc/commands/volume/volume_cmd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,279 +1,248 @@
 import json
+import sys
 import click
 
-from cgc.commands.compute.compute_models import EntityList, GPUsList
-from cgc.commands.compute.compute_responses import (
-    compute_create_filebrowser_response,
-    compute_create_response,
-    compute_delete_response,
-    compute_restart_response,
-    compute_list_response,
-    template_list_response,
-    template_get_start_path_response,
-)
-from cgc.commands.compute.compute_utills import (
-    compute_create_payload,
-    compute_delete_payload,
+from cgc.commands.volume.data_model import (
+    volume_create_payload_validator,
+    volume_delete_payload_validator,
+    volume_mount_payload_validator,
+    volume_umount_payload_validator,
+)
+from cgc.commands.volume.volume_responses import (
+    volume_list_response,
+    volume_mount_response,
+    volume_umount_response,
+    volume_create_response,
+    volume_delete_response,
 )
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.utils.click_group import CustomGroup, CustomCommand
 from cgc.utils.requests_helper import call_api, EndpointTypes
 
 
-@click.group(name="compute", cls=CustomGroup)
-@click.option("--debug", "debug", is_flag=True, default=False, hidden=True)
-@click.pass_context
-def compute_group(ctx, debug):
+@click.group("volume", cls=CustomGroup)
+def volume_group():
     """
-    Management of compute resources.
+    Management of volumes.
     """
-    ctx.ensure_object(dict)
-    ctx.obj["DEBUG"] = debug
+    pass
 
 
-@click.group(name="template", cls=CustomGroup)
-def template_group():
+@volume_group.command("list", cls=CustomCommand)
+def volume_list():
     """
-    Management of templates.
+    List all volumes for user namespace.
     """
-
-
-@template_group.command("list", cls=CustomCommand)
-def template_list():
-    """Lists all available templates"""
-    api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/compute/list_available_templates"
-    metric = "compute.template.list"
-    __res = call_api(request=EndpointTypes.get, url=url, headers=headers)
-    click.echo(
-        template_list_response(
-            retrieve_and_validate_response_send_metric(__res, metric)
-        )
-    )
-
-
-@template_group.command("get_start_path", cls=CustomCommand)
-@click.argument("template", type=click.Choice(EntityList.get_list()))
-def template_get_start_path(template: str):
-    """Displays start path of specified template"""
-    api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/compute/get_template_start_path?template_name={template}"
-    metric = "compute.template.get_start_path"
-    __res = call_api(request=EndpointTypes.get, url=url, headers=headers)
-    click.echo(
-        template_get_start_path_response(
-            retrieve_and_validate_response_send_metric(__res, metric)
-        )
-    )
-
-
-@click.group(name="filebrowser", cls=CustomGroup)
-def filebrowser_group():
-    """
-    Management of filebrowser.
-    """
-
-
-@filebrowser_group.command("create", cls=CustomCommand)
-def compute_filebrowser_create():
-    """Create a filebrowser service"""
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/compute/filebrowser_create"
-    metric = "compute.create_filebrowser"
-    __payload = {"puid": 0, "pgid": 0}
+    url = f"{api_url}/v1/api/storage/volume/list"
+    metric = "volume.list"
     __res = call_api(
-        request=EndpointTypes.post,
+        request=EndpointTypes.get,
         url=url,
         headers=headers,
-        data=json.dumps(__payload),
     )
     click.echo(
-        compute_create_filebrowser_response(
-            retrieve_and_validate_response_send_metric(__res, metric)
-        )
+        volume_list_response(retrieve_and_validate_response_send_metric(__res, metric))
     )
 
 
-@filebrowser_group.command("delete", cls=CustomCommand)
-def compute_filebrowser_delete():
-    """Delete a filebrowser service"""
-    compute_delete("filebrowser")
-
-
-@compute_group.command("create", cls=CustomCommand)
-@click.argument("entity", type=click.Choice(EntityList.get_list()))
-@click.option("-n", "--name", "name", type=click.STRING, required=True)
-@click.option(
-    "-g",
-    "--gpu",
-    "gpu",
-    type=click.INT,
-    default=0,
-    help="How much GPU cards app will use",
-)
-@click.option(
-    "-gt",
-    "--gpu-type",
-    "gpu_type",
-    type=click.Choice(GPUsList.get_list(), case_sensitive=False),
-    default="A5000",
-    help="Graphic card used by the app",
-)
+@volume_group.command("create", cls=CustomCommand)
+@click.argument("name")
+@click.option("-s", "--size", "size", type=click.IntRange(1, 1000), required=True)
 @click.option(
-    "-c",
-    "--cpu",
-    "cpu",
-    type=click.INT,
-    default=1,
-    help="How much CPU cores app can use",
+    "-t",
+    "--type",
+    "disk_type",
+    type=click.Choice(["ssd", "nvme"]),
+    default="ssd",
+    help="Type of disk",
 )
 @click.option(
-    "-m",
-    "--memory",
-    "memory",
-    type=click.INT,
-    default=2,
-    help="How much Gi RAM app can use",
+    "-a",
+    "--access",
+    "access",
+    type=click.Choice(["rwx", "rwo"]),
+    default="rwx",
+    help="Volume access mode",
 )
-@click.option(
-    "-v",
-    "--volume",
-    "volumes",
-    multiple=True,
-    help="List of volume names to be mounted with default mount path",
-)
-def compute_create(
-    entity: str,
-    gpu: int,
-    gpu_type: str,
-    cpu: int,
-    memory: int,
-    volumes: list[str],
-    name: str,
-):
-    """
-    Create an app in user namespace.
+def volume_create(name: str, size: int, disk_type: str, access: str):
+    """Create volume in user namespace.
     \f
-    :param entity: name of entity to create
-    :type entity: str
-    :param gpu: number of gpus to be used by app
-    :type gpu: int
-    :param cpu: number of cores to be used by app
-    :type cpu: int
-    :param memory: GB of memory to be used by app
-    :type memory: int
-    :param volumes: list of volumes to mount
-    :type volumes: list[str]
-    :param name: name of app
+    :param name: name of volume
     :type name: str
+    :param size: size of volume in GB
+    :type size: int
+    :param type: type of volume - HDD, SSD or NVMe
+    :type type: str
+    :param access: access type of volume - RWO or RWX
+    :type access: str
     """
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/compute/create"
-    metric = "compute.create"
-    __payload = compute_create_payload(
-        name=name,
-        entity=entity,
-        cpu=cpu,
-        memory=memory,
-        gpu=gpu,
-        volumes=volumes,
-        gpu_type=gpu_type,
+    url = f"{api_url}/v1/api/storage/volume/create"
+    metric = "volume.create"
+    __payload = volume_create_payload_validator(
+        name=name, access=access, size=size, disk_type=disk_type
     )
     __res = call_api(
         request=EndpointTypes.post,
         url=url,
-        headers=headers,
         data=json.dumps(__payload),
+        headers=headers,
     )
     click.echo(
-        compute_create_response(
+        volume_create_response(
             retrieve_and_validate_response_send_metric(__res, metric)
         )
     )
 
 
-@compute_group.command("delete", cls=CustomCommand)
-@click.argument("name", type=click.STRING)
-def compute_delete_cmd(name: str):
-    """
-    Delete an app from user namespace.
-    \f
-    :param name: name of app to delete
-    :type name: str
-    """
-    compute_delete(name)
-
-
-def compute_delete(name: str):
-    """
-    Delete an app using backend endpoint.
+@volume_group.command("delete", cls=CustomCommand)
+@click.argument("name")
+@click.option(
+    "-f",
+    "--force",
+    "force_delete",
+    is_flag=True,
+    default=False,
+    help="Force delete volume",
+)
+def volume_delete(name: str, force_delete: bool):
+    """Delete specific volume from user namespace.
     \f
-    :param name: name of app to delete
+    :param name: name of the volume to delete
     :type name: str
+    :param force_delete: delete volume even if it is still mounted
+    :type force_delete: bool
     """
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/compute/delete"
-    metric = "compute.delete"
-    __payload = compute_delete_payload(name=name)
+    url = f"{api_url}/v1/api/storage/volume/delete"
+    metric = "volume.delete"
+    __payload = volume_delete_payload_validator(
+        name=name,
+        force_delete=force_delete,
+    )
     __res = call_api(
         request=EndpointTypes.delete,
         url=url,
-        headers=headers,
         data=json.dumps(__payload),
+        headers=headers,
     )
     click.echo(
-        compute_delete_response(
+        volume_delete_response(
             retrieve_and_validate_response_send_metric(__res, metric)
         )
     )
 
 
-@compute_group.command("list", cls=CustomCommand)
+@volume_group.command("umount", cls=CustomCommand)
+@click.argument("name")
 @click.option(
-    "-d", "--detailed", "detailed", type=click.BOOL, is_flag=True, default=False
+    "-t",
+    "--target",
+    "target_template_names",
+    multiple=True,
+    default=None,
+    help="This template will have volume unmounted",
 )
-@click.pass_context
-def compute_list(ctx, detailed):
-    """
-    List all apps for user namespace.
+def volume_umount(name: str, target_template_names):
+    """Umount volume from compute resources.
+    \f
+    :param name: name of the volume to umount
+    :type name: str
     """
-    api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/compute/list"
-    metric = "compute.list"
+    while True:
+        if len(target_template_names) == 0:
+            click.echo(
+                "Unmounting a volume will reload all compute resources it was mounted to"
+            )
+        else:
+            click.echo(
+                f'Unmounting a volume will reload those resources: "{target_template_names}"'
+            )
+        answer = input("Do you want to continue? (Y/N): ").lower()
+        if answer in ("y", "yes"):
+            break
+        if answer in ("n", "no"):
+            sys.exit()
+
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/storage/volume/umount"
+    metric = "volume.umount"
+    __payload = volume_umount_payload_validator(
+        name=name, target_template_names=target_template_names
+    )
     __res = call_api(
-        request=EndpointTypes.get,
+        request=EndpointTypes.post,
         url=url,
+        data=json.dumps(__payload),
         headers=headers,
     )
-    table = compute_list_response(
-        detailed,
-        retrieve_and_validate_response_send_metric(__res, metric),
+    click.echo(
+        volume_umount_response(
+            retrieve_and_validate_response_send_metric(__res, metric)
+        )
     )
 
-    click.echo(table)
 
-
-@compute_group.command("restart", cls=CustomCommand)
-@click.argument("name", type=click.STRING)
-def compute_restart(name: str):
-    """Restarts the specified app"""
-    api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/compute/restart"
-    metric = "compute.restart"
-    __payload = {"name": name}
+@volume_group.command("mount", cls=CustomCommand)
+@click.argument("name")
+@click.option(
+    "-t",
+    "--target",
+    "target",
+    type=str,
+    required=True,
+    help="This template will have volume mounted",
+)
+@click.option(
+    "-p",
+    "--mount_path",
+    "mount_path",
+    type=str,
+    default=None,
+    help="Under this path (not default) will be volume mounted",
+)
+def volume_mount(
+    name: str,
+    target: str,
+    mount_path: str,
+):
+    """Mount volume to specific template.
+    \f
+    :param name: name of the volume to mount
+    :type name: str
+    :param target_template_type: type of template to mount volume to
+    :type target_template_type: str
+    :param target: name of the template to mount volume to
+    :type target: str
+    :param mount_path: path to mount volume to
+    :type mount_path: str
+    """
+    while True:
+        click.echo(
+            "Mounting a volume will reload the compute resources it will be mounted to."
+        )
+        answer = input("Do you want to continue? (Y/N): ").lower()
+        if answer in ("y", "yes"):
+            break
+        if answer in ("n", "no"):
+            sys.exit()
+
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/storage/volume/mount"
+    metric = "volume.mount"
+    __payload = volume_mount_payload_validator(
+        name=name,
+        target=target,
+        mount_path=mount_path,
+    )
     __res = call_api(
         request=EndpointTypes.post,
         url=url,
-        headers=headers,
         data=json.dumps(__payload),
+        headers=headers,
     )
     click.echo(
-        compute_restart_response(
-            retrieve_and_validate_response_send_metric(__res, metric)
-        )
+        volume_mount_response(retrieve_and_validate_response_send_metric(__res, metric))
     )
-
-
-compute_group.add_command(filebrowser_group)
-compute_group.add_command(template_group)
```

### Comparing `cgcsdk-0.7.1/cgc/commands/compute/compute_models.py` & `cgcsdk-0.8.0/cgc/commands/compute/compute_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 from enum import Enum
 
 
-class EntityList(Enum):
+class CGCEntityList(Enum):
+    """Base class for other lists"""
+
+    @classmethod
+    def get_list(cls) -> list[str]:
+        return [el.value for el in cls]
+
+
+class EntityList(CGCEntityList):
     """List of templates in cgc-server
 
     :param Enum: name of template
     :type Enum: str
     """
 
     NVIDIA_TENSORFLOW = "nvidia-tensorflow"
     NVIDIA_RAPIDS = "nvidia-rapids"
     NVIDIA_PYTORCH = "nvidia-pytorch"
     NVIDIA_TRITON = "nvidia-triton"
 
-    @classmethod
-    def get_list(cls) -> list[str]:
-        return [el.value for el in cls]
 
+class DatabasesList(CGCEntityList):
+    """List of templates in cgc-server
+
+    :param Enum: name of template
+    :type Enum: str
+    """
+
+    MONGODB = "mongodb"
+    POSTGRESQL = "postgresql"
+    REDIS = "redis"
 
-class GPUsList(Enum):
+
+class GPUsList(CGCEntityList):
     """List of templates in cgc-server
 
     :param Enum: name of template
     :type Enum: str
     """
 
     A100 = "A100"
     # V100 = "V100"
     A5000 = "A5000"
-
-    @classmethod
-    def get_list(cls) -> list[str]:
-        return [el.value for el in cls]
```

### Comparing `cgcsdk-0.7.1/cgc/commands/compute/compute_responses.py` & `cgcsdk-0.8.0/cgc/commands/compute/compute_responses.py`

 * *Files 11% similar despite different names*

```diff
@@ -85,21 +85,26 @@
     entity = data["details"]["created_service"]["labels"]["entity"]
     volume_list = data["details"].get("mounted_pvc_list")
     volumes = ",".join(volume_list) if volume_list else None
     try:
         app_token = data["details"]["created_template"]["app_token"]
     except KeyError:
         app_token = None
-    app_url = data["details"]["created_template"]["pod_url"]
 
     message = f"{entity} app {name} creation started!\n"
     if volumes:
         message += f" Volumes to mount: {volumes}\n"
         message += f"Container will be Ready after volumes can be see mounted.\n"
-    message += f"Will be accessible at: {app_url}\nApp token: {app_token}\nTo monitor the startup status use command: cgc compute list"
+
+    app_url = data["details"]["created_template"]["pod_url"]
+    if app_url == "None":
+        message += f"Will be accessible at: {app_url}\n"
+    else:
+        message += "This app is not exposed via HTTPS\n"
+    message += f"App token: {app_token}\nTo monitor the startup status use command: cgc resource list"
 
     return message
 
 
 @key_error_decorator_for_helpers
 def compute_delete_response(data: dict) -> str:
     """Create response string for compute delete command.
@@ -122,7 +127,29 @@
     :type response: requests.Response
     :return: Response string.
     :rtype: str
     """
 
     name = data["details"]["template_name"]
     return f"App {name} has been successfully restarted."
+
+
+@key_error_decorator_for_helpers
+def compute_logs_response(data: dict) -> str:
+    """prepare logs to print
+
+    :param data: _description_
+    :type data: dict
+    :return: _description_
+    :rtype: str
+    """
+    # converting dict o list
+    logs_list = []
+    for event in data["details"]["pod_event_list"]:
+        row = []
+        for key, value in event.items():
+            row.append((key, value))
+        logs_list.append(row)
+    if len(logs_list) > 0:
+        return tabulate_a_response(logs_list)
+    else:
+        return "No events to list for this app"
```

### Comparing `cgcsdk-0.7.1/cgc/commands/compute/compute_utills.py` & `cgcsdk-0.8.0/cgc/commands/compute/compute_utills.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,30 +72,33 @@
         except KeyError:
             pass
 
     return output_data
 
 
 def compute_create_payload(
-    name, entity, cpu, memory, volumes: list, gpu: int, gpu_type: str
+    name, entity, cpu, memory, volumes: list, gpu: int = 0, gpu_type: str = None
 ):
     """
     Create payload for app creation.
     """
 
     payload = {
         "name": name,
         "entity": entity,
         "cpu": cpu,
         "gpu": gpu,
         "memory": memory,
         "gpu_type": gpu_type,
     }
-    if len(volumes) != 0:
-        payload["pv_volume"] = volumes
+    try:
+        if len(volumes) != 0:
+            payload["pv_volume"] = volumes
+    except TypeError:
+        pass
     return payload
 
 
 def compute_delete_payload(name):
     """
     Create payload for app creation.
     """
```

### Comparing `cgcsdk-0.7.1/cgc/commands/volume/data_model.py` & `cgcsdk-0.8.0/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/commands/volume/volume_responses.py` & `cgcsdk-0.8.0/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/commands/volume/volume_utils.py` & `cgcsdk-0.8.0/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/server.crt` & `cgcsdk-0.8.0/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/telemetry/basic.py` & `cgcsdk-0.8.0/cgc/telemetry/basic.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,21 @@
     """Set telemetry permission to .env file
 
     :return: TELEMETRY_PERMISSION value
     :rtype: bool
     """
     while True:
         permission = input(
-            "Do you want to send telemetry info for application improvements purposes? [yes/no]:\n"
+            "We would like to make your experience with CGC even better! :)\n\
+            We would like to know which commands are utilized most often and if they have finished properly. Nothing else is collected. Only raw numbers.\n\
+Would you agree to send us these numbers? (YES/no) [YES]: \n"
         )
-        if permission in ["yes", "no"]:
+        if permission.lower() in ["yes", "no", ""]:
             break
-    permission = True if permission == "yes" else False
+    permission = True if permission == "" or permission == "yes" else False
 
     f = open(file=ENV_FILE_PATH, mode="r")
     replaced_content = f.read()
     replaced_content = replaced_content.splitlines()
     f.close()
     for i, line in enumerate(replaced_content):
         splitted = line.split(" ")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cgcsdk-0.7.1/cgc/tests/__init__.py` & `cgcsdk-0.8.0/cgc/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                         {
                             "rent_start": "2023-02-03 16:25:17",
                             "rent_end": "2023-02-09 10:15:24",
                             "rent_time": 496207.06346,
                             "rent_start_cost": "2023-02-03 16:25:17",
                             "rent_end_cost": "2023-02-09 10:15:24",
                             "rent_time_cost": 496207.06346,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 1,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -49,15 +49,15 @@
                         {
                             "rent_start": "2023-02-07 14:33:57",
                             "rent_end": "2023-02-09 10:15:24",
                             "rent_time": 157287.06558,
                             "rent_start_cost": "2023-02-07 14:33:57",
                             "rent_end_cost": "2023-02-09 10:15:24",
                             "rent_time_cost": 157287.06558,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 2,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -69,15 +69,15 @@
                         {
                             "rent_start": "2023-02-08 13:57:02",
                             "rent_end": "2023-02-09 10:15:24",
                             "rent_time": 73102.066748,
                             "rent_start_cost": "2023-02-08 13:57:02",
                             "rent_end_cost": "2023-02-09 10:15:24",
                             "rent_time_cost": 73102.066748,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test2",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 2,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -89,15 +89,15 @@
                         {
                             "rent_start": "2023-02-08 14:00:13",
                             "rent_end": "2023-02-09 10:15:24",
                             "rent_time": 72911.068128,
                             "rent_start_cost": "2023-02-08 14:00:13",
                             "rent_end_cost": "2023-02-09 10:15:24",
                             "rent_time_cost": 72911.068128,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test2",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 2,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -109,15 +109,15 @@
                         {
                             "rent_start": "2023-02-08 15:28:08",
                             "rent_end": "2023-02-09 10:15:24",
                             "rent_time": 67636.069558,
                             "rent_start_cost": "2023-02-08 15:28:08",
                             "rent_end_cost": "2023-02-09 10:15:24",
                             "rent_time_cost": 67636.069558,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test2",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 2,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -163,15 +163,15 @@
                         {
                             "rent_start": "2023-02-02 15:32:50",
                             "rent_end": "2023-02-03 15:38:32",
                             "rent_time": 86742,
                             "rent_start_cost": "2023-02-02 15:32:50",
                             "rent_end_cost": "2023-02-03 15:38:32",
                             "rent_time_cost": 86742,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 1,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -183,15 +183,15 @@
                         {
                             "rent_start": "2023-02-03 15:38:53",
                             "rent_end": "2023-02-03 16:06:05",
                             "rent_time": 1632,
                             "rent_start_cost": "2023-02-03 15:38:53",
                             "rent_end_cost": "2023-02-03 16:06:05",
                             "rent_time_cost": 1632,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 2,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -203,15 +203,15 @@
                         {
                             "rent_start": "2023-02-03 16:06:13",
                             "rent_end": "2023-02-03 16:18:49",
                             "rent_time": 756,
                             "rent_start_cost": "2023-02-03 16:06:13",
                             "rent_end_cost": "2023-02-03 16:18:49",
                             "rent_time_cost": 756,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "filebrowser",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 1,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -223,15 +223,15 @@
                         {
                             "rent_start": "2023-02-03 16:30:11",
                             "rent_end": "2023-02-03 16:33:25",
                             "rent_time": 194,
                             "rent_start_cost": "2023-02-03 16:30:11",
                             "rent_end_cost": "2023-02-03 16:33:25",
                             "rent_time_cost": 194,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test3",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 1,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -260,15 +260,15 @@
                         {
                             "rent_start": "2023-02-02 14:03:20",
                             "rent_end": "2023-02-08 14:00:06",
                             "rent_time": 518206,
                             "rent_start_cost": "2023-02-02 14:03:20",
                             "rent_end_cost": "2023-02-08 14:00:06",
                             "rent_time_cost": 518206,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test2",
                                 "entity": "nvidia-pytorch",
                                 "cpu": 1,
                                 "memory": 1,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -280,15 +280,15 @@
                         {
                             "rent_start": "2023-02-03 16:30:03",
                             "rent_end": "2023-02-08 15:27:22",
                             "rent_time": 428239,
                             "rent_start_cost": "2023-02-03 16:30:03",
                             "rent_end_cost": "2023-02-08 15:27:22",
                             "rent_time_cost": 428239,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test2",
                                 "entity": "tensorflow-jupyter",
                                 "cpu": 1,
                                 "memory": 1,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -339,15 +339,15 @@
                         {
                             "rent_start": "2023-02-05 14:50:48",
                             "rent_end": "2023-02-05 14:52:26",
                             "rent_time": 98,
                             "rent_start_cost": "2023-02-05 14:50:48",
                             "rent_end_cost": "2023-02-05 14:52:26",
                             "rent_time_cost": 98,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test1",
                                 "entity": "nvidia-pytorch",
                                 "cpu": 1,
                                 "memory": 2,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -359,15 +359,15 @@
                         {
                             "rent_start": "2023-02-05 14:54:49",
                             "rent_end": "2023-02-07 14:13:51",
                             "rent_time": 170342,
                             "rent_start_cost": "2023-02-05 14:54:49",
                             "rent_end_cost": "2023-02-07 14:13:51",
                             "rent_time_cost": 170342,
-                            "type": "events_compute",
+                            "type": "events_resource",
                             "resources": {
                                 "name": "test1",
                                 "entity": "nvidia-pytorch",
                                 "cpu": 1,
                                 "memory": 2,
                                 "gpu": 0,
                                 "gpu_type": None,
@@ -376,15 +376,15 @@
                             "tid_end": "63e25c9fc037717bc2322083",
                             "cost_total": 42585,
                         },
                     ],
                 },
             ],
         },
-        "message": "{'namespace': 'pytest', 'cost_total': 75665.4, 'details': [{'user_id': 'e57c8668-6bc3-47c7-85de-903bfc3772b7', 'details': [{'rent_start': '2023-02-03 16:25:17', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 496207.06346, 'rent_start_cost': '2023-02-03 16:25:17', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 496207.06346, 'type': 'events_compute', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd356cc037717bc2322053', 'tid_end': None, 'cost_total': 1654.0}, {'rent_start': '2023-02-03 16:58:38', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 494206.064514, 'rent_start_cost': '2023-02-03 16:58:38', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 494206.064514, 'type': 'events_volume', 'resources': {'name': 'test2', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63dd3d3dc037717bc2322069', 'tid_end': None, 'cost_total': 823.7}, {'rent_start': '2023-02-07 14:33:57', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 157287.06558, 'rent_start_cost': '2023-02-07 14:33:57', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 157287.06558, 'type': 'events_compute', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63e26155c037717bc232208b', 'tid_end': None, 'cost_total': 786.3000000000001}, {'rent_start': '2023-02-08 13:57:02', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 73102.066748, 'rent_start_cost': '2023-02-08 13:57:02', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 73102.066748, 'type': 'events_compute', 'resources': {'name': 'test2', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63e3aa2dc037717bc2322097', 'tid_end': None, 'cost_total': 365.40000000000003}, {'rent_start': '2023-02-08 14:00:13', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 72911.068128, 'rent_start_cost': '2023-02-08 14:00:13', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 72911.068128, 'type': 'events_compute', 'resources': {'name': 'test2', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63e3aaecc037717bc232209c', 'tid_end': None, 'cost_total': 364.5}, {'rent_start': '2023-02-08 15:28:08', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 67636.069558, 'rent_start_cost': '2023-02-08 15:28:08', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 67636.069558, 'type': 'events_compute', 'resources': {'name': 'test2', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63e3bf88c037717bc23220a1', 'tid_end': None, 'cost_total': 338.1}, {'rent_start': '2023-02-02 15:24:01', 'rent_end': '2023-02-02 15:26:23', 'rent_time': 142.0, 'rent_start_cost': '2023-02-02 15:24:01', 'rent_end_cost': '2023-02-02 15:26:23', 'rent_time_cost': 142.0, 'type': 'events_volume', 'resources': {'name': 'duzy', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63dbd597c037717bc232200a', 'tid_end': '63dbd61fc037717bc232200d', 'cost_total': 0.2}, {'rent_start': '2023-02-02 15:40:52', 'rent_end': '2023-02-02 15:44:50', 'rent_time': 238.0, 'rent_start_cost': '2023-02-02 15:40:52', 'rent_end_cost': '2023-02-02 15:44:50', 'rent_time_cost': 238.0, 'type': 'events_volume', 'resources': {'name': 'duzy', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63dbd983c037717bc2322015', 'tid_end': '63dbda71c037717bc2322019', 'cost_total': 0.4}, {'rent_start': '2023-02-02 15:32:50', 'rent_end': '2023-02-03 15:38:32', 'rent_time': 86742.0, 'rent_start_cost': '2023-02-02 15:32:50', 'rent_end_cost': '2023-02-03 15:38:32', 'rent_time_cost': 86742.0, 'type': 'events_compute', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dbd7a1c037717bc232200f', 'tid_end': '63dd2a77c037717bc2322041', 'cost_total': 289.2}, {'rent_start': '2023-02-03 15:38:53', 'rent_end': '2023-02-03 16:06:05', 'rent_time': 1632.0, 'rent_start_cost': '2023-02-03 15:38:53', 'rent_end_cost': '2023-02-03 16:06:05', 'rent_time_cost': 1632.0, 'type': 'events_compute', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd2a8dc037717bc2322043', 'tid_end': '63dd30edc037717bc232204b', 'cost_total': 8.100000000000001}, {'rent_start': '2023-02-03 16:06:13', 'rent_end': '2023-02-03 16:18:49', 'rent_time': 756.0, 'rent_start_cost': '2023-02-03 16:06:13', 'rent_end_cost': '2023-02-03 16:18:49', 'rent_time_cost': 756.0, 'type': 'events_compute', 'resources': {'name': 'filebrowser', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd30f4c037717bc232204d', 'tid_end': '63dd33e8c037717bc2322050', 'cost_total': 2.6}, {'rent_start': '2023-02-03 16:30:11', 'rent_end': '2023-02-03 16:33:25', 'rent_time': 194.0, 'rent_start_cost': '2023-02-03 16:30:11', 'rent_end_cost': '2023-02-03 16:33:25', 'rent_time_cost': 194.0, 'type': 'events_compute', 'resources': {'name': 'test3', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd3692c037717bc232205b', 'tid_end': '63dd3754c037717bc232205e', 'cost_total': 0.6000000000000001}, {'rent_start': '2023-02-03 16:53:52', 'rent_end': '2023-02-03 16:58:32', 'rent_time': 280.0, 'rent_start_cost': '2023-02-03 16:53:52', 'rent_end_cost': '2023-02-03 16:58:32', 'rent_time_cost': 280.0, 'type': 'events_volume', 'resources': {'name': 'test2', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63dd3c20c037717bc2322063', 'tid_end': '63dd3d38c037717bc2322067', 'cost_total': 0.5}, {'rent_start': '2023-02-02 14:03:20', 'rent_end': '2023-02-08 14:00:06', 'rent_time': 518206.0, 'rent_start_cost': '2023-02-02 14:03:20', 'rent_end_cost': '2023-02-08 14:00:06', 'rent_time_cost': 518206.0, 'type': 'events_compute', 'resources': {'name': 'test2', 'entity': 'nvidia-pytorch', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dbc2a8c037717bc2322001', 'tid_end': '63e3aae6c037717bc232209a', 'cost_total': 1727.4}, {'rent_start': '2023-02-03 16:30:03', 'rent_end': '2023-02-08 15:27:22', 'rent_time': 428239.0, 'rent_start_cost': '2023-02-03 16:30:03', 'rent_end_cost': '2023-02-08 15:27:22', 'rent_time_cost': 428239.0, 'type': 'events_compute', 'resources': {'name': 'test2', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd368ac037717bc2322058', 'tid_end': '63e3bf59c037717bc232209f', 'cost_total': 1427.4}]}, {'user_id': '9a8b327c-1f27-4d79-a387-071cd0954cf9', 'details': [{'rent_start': '2023-01-03 12:40:08', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 3188116.118518, 'rent_start_cost': '2023-02-01 00:00:00', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 728124.118518, 'type': 'events_volume', 'resources': {'name': 'test', 'disks_type': 'ssd', 'size': 1}, 'tid_start': '63dd00a8c037717bc232201d', 'tid_end': None, 'cost_total': 24270}, {'rent_start': '2023-02-04 09:08:29', 'rent_end': '2023-02-04 17:24:09', 'rent_time': 29740.0, 'rent_start_cost': '2023-02-04 09:08:29', 'rent_end_cost': '2023-02-04 17:24:09', 'rent_time_cost': 29740.0, 'type': 'events_volume', 'resources': {'name': 'test1', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63de208cc037717bc232206c', 'tid_end': '63de94b9c037717bc232206f', 'cost_total': 992.0}, {'rent_start': '2023-02-05 14:50:48', 'rent_end': '2023-02-05 14:52:26', 'rent_time': 98.0, 'rent_start_cost': '2023-02-05 14:50:48', 'rent_end_cost': '2023-02-05 14:52:26', 'rent_time_cost': 98.0, 'type': 'events_compute', 'resources': {'name': 'test1', 'entity': 'nvidia-pytorch', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dfc248c037717bc2322079', 'tid_end': '63dfc2a9c037717bc232207c', 'cost_total': 30}, {'rent_start': '2023-02-05 14:54:49', 'rent_end': '2023-02-07 14:13:51', 'rent_time': 170342.0, 'rent_start_cost': '2023-02-05 14:54:49', 'rent_end_cost': '2023-02-07 14:13:51', 'rent_time_cost': 170342.0, 'type': 'events_compute', 'resources': {'name': 'test1', 'entity': 'nvidia-pytorch', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dfc338c037717bc232207e', 'tid_end': '63e25c9fc037717bc2322083', 'cost_total': 42585}]}]}",
+        "message": "{'namespace': 'pytest', 'cost_total': 75665.4, 'details': [{'user_id': 'e57c8668-6bc3-47c7-85de-903bfc3772b7', 'details': [{'rent_start': '2023-02-03 16:25:17', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 496207.06346, 'rent_start_cost': '2023-02-03 16:25:17', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 496207.06346, 'type': 'events_resource', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd356cc037717bc2322053', 'tid_end': None, 'cost_total': 1654.0}, {'rent_start': '2023-02-03 16:58:38', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 494206.064514, 'rent_start_cost': '2023-02-03 16:58:38', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 494206.064514, 'type': 'events_volume', 'resources': {'name': 'test2', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63dd3d3dc037717bc2322069', 'tid_end': None, 'cost_total': 823.7}, {'rent_start': '2023-02-07 14:33:57', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 157287.06558, 'rent_start_cost': '2023-02-07 14:33:57', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 157287.06558, 'type': 'events_resource', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63e26155c037717bc232208b', 'tid_end': None, 'cost_total': 786.3000000000001}, {'rent_start': '2023-02-08 13:57:02', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 73102.066748, 'rent_start_cost': '2023-02-08 13:57:02', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 73102.066748, 'type': 'events_resource', 'resources': {'name': 'test2', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63e3aa2dc037717bc2322097', 'tid_end': None, 'cost_total': 365.40000000000003}, {'rent_start': '2023-02-08 14:00:13', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 72911.068128, 'rent_start_cost': '2023-02-08 14:00:13', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 72911.068128, 'type': 'events_resource', 'resources': {'name': 'test2', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63e3aaecc037717bc232209c', 'tid_end': None, 'cost_total': 364.5}, {'rent_start': '2023-02-08 15:28:08', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 67636.069558, 'rent_start_cost': '2023-02-08 15:28:08', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 67636.069558, 'type': 'events_resource', 'resources': {'name': 'test2', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63e3bf88c037717bc23220a1', 'tid_end': None, 'cost_total': 338.1}, {'rent_start': '2023-02-02 15:24:01', 'rent_end': '2023-02-02 15:26:23', 'rent_time': 142.0, 'rent_start_cost': '2023-02-02 15:24:01', 'rent_end_cost': '2023-02-02 15:26:23', 'rent_time_cost': 142.0, 'type': 'events_volume', 'resources': {'name': 'duzy', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63dbd597c037717bc232200a', 'tid_end': '63dbd61fc037717bc232200d', 'cost_total': 0.2}, {'rent_start': '2023-02-02 15:40:52', 'rent_end': '2023-02-02 15:44:50', 'rent_time': 238.0, 'rent_start_cost': '2023-02-02 15:40:52', 'rent_end_cost': '2023-02-02 15:44:50', 'rent_time_cost': 238.0, 'type': 'events_volume', 'resources': {'name': 'duzy', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63dbd983c037717bc2322015', 'tid_end': '63dbda71c037717bc2322019', 'cost_total': 0.4}, {'rent_start': '2023-02-02 15:32:50', 'rent_end': '2023-02-03 15:38:32', 'rent_time': 86742.0, 'rent_start_cost': '2023-02-02 15:32:50', 'rent_end_cost': '2023-02-03 15:38:32', 'rent_time_cost': 86742.0, 'type': 'events_resource', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dbd7a1c037717bc232200f', 'tid_end': '63dd2a77c037717bc2322041', 'cost_total': 289.2}, {'rent_start': '2023-02-03 15:38:53', 'rent_end': '2023-02-03 16:06:05', 'rent_time': 1632.0, 'rent_start_cost': '2023-02-03 15:38:53', 'rent_end_cost': '2023-02-03 16:06:05', 'rent_time_cost': 1632.0, 'type': 'events_resource', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd2a8dc037717bc2322043', 'tid_end': '63dd30edc037717bc232204b', 'cost_total': 8.100000000000001}, {'rent_start': '2023-02-03 16:06:13', 'rent_end': '2023-02-03 16:18:49', 'rent_time': 756.0, 'rent_start_cost': '2023-02-03 16:06:13', 'rent_end_cost': '2023-02-03 16:18:49', 'rent_time_cost': 756.0, 'type': 'events_resource', 'resources': {'name': 'filebrowser', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd30f4c037717bc232204d', 'tid_end': '63dd33e8c037717bc2322050', 'cost_total': 2.6}, {'rent_start': '2023-02-03 16:30:11', 'rent_end': '2023-02-03 16:33:25', 'rent_time': 194.0, 'rent_start_cost': '2023-02-03 16:30:11', 'rent_end_cost': '2023-02-03 16:33:25', 'rent_time_cost': 194.0, 'type': 'events_resource', 'resources': {'name': 'test3', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd3692c037717bc232205b', 'tid_end': '63dd3754c037717bc232205e', 'cost_total': 0.6000000000000001}, {'rent_start': '2023-02-03 16:53:52', 'rent_end': '2023-02-03 16:58:32', 'rent_time': 280.0, 'rent_start_cost': '2023-02-03 16:53:52', 'rent_end_cost': '2023-02-03 16:58:32', 'rent_time_cost': 280.0, 'type': 'events_volume', 'resources': {'name': 'test2', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63dd3c20c037717bc2322063', 'tid_end': '63dd3d38c037717bc2322067', 'cost_total': 0.5}, {'rent_start': '2023-02-02 14:03:20', 'rent_end': '2023-02-08 14:00:06', 'rent_time': 518206.0, 'rent_start_cost': '2023-02-02 14:03:20', 'rent_end_cost': '2023-02-08 14:00:06', 'rent_time_cost': 518206.0, 'type': 'events_resource', 'resources': {'name': 'test2', 'entity': 'nvidia-pytorch', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dbc2a8c037717bc2322001', 'tid_end': '63e3aae6c037717bc232209a', 'cost_total': 1727.4}, {'rent_start': '2023-02-03 16:30:03', 'rent_end': '2023-02-08 15:27:22', 'rent_time': 428239.0, 'rent_start_cost': '2023-02-03 16:30:03', 'rent_end_cost': '2023-02-08 15:27:22', 'rent_time_cost': 428239.0, 'type': 'events_resource', 'resources': {'name': 'test2', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 1, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dd368ac037717bc2322058', 'tid_end': '63e3bf59c037717bc232209f', 'cost_total': 1427.4}]}, {'user_id': '9a8b327c-1f27-4d79-a387-071cd0954cf9', 'details': [{'rent_start': '2023-01-03 12:40:08', 'rent_end': '2023-02-09 10:15:24', 'rent_time': 3188116.118518, 'rent_start_cost': '2023-02-01 00:00:00', 'rent_end_cost': '2023-02-09 10:15:24', 'rent_time_cost': 728124.118518, 'type': 'events_volume', 'resources': {'name': 'test', 'disks_type': 'ssd', 'size': 1}, 'tid_start': '63dd00a8c037717bc232201d', 'tid_end': None, 'cost_total': 24270}, {'rent_start': '2023-02-04 09:08:29', 'rent_end': '2023-02-04 17:24:09', 'rent_time': 29740.0, 'rent_start_cost': '2023-02-04 09:08:29', 'rent_end_cost': '2023-02-04 17:24:09', 'rent_time_cost': 29740.0, 'type': 'events_volume', 'resources': {'name': 'test1', 'disks_type': 'ssd', 'size': 1.0}, 'tid_start': '63de208cc037717bc232206c', 'tid_end': '63de94b9c037717bc232206f', 'cost_total': 992.0}, {'rent_start': '2023-02-05 14:50:48', 'rent_end': '2023-02-05 14:52:26', 'rent_time': 98.0, 'rent_start_cost': '2023-02-05 14:50:48', 'rent_end_cost': '2023-02-05 14:52:26', 'rent_time_cost': 98.0, 'type': 'events_resource', 'resources': {'name': 'test1', 'entity': 'nvidia-pytorch', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dfc248c037717bc2322079', 'tid_end': '63dfc2a9c037717bc232207c', 'cost_total': 30}, {'rent_start': '2023-02-05 14:54:49', 'rent_end': '2023-02-07 14:13:51', 'rent_time': 170342.0, 'rent_start_cost': '2023-02-05 14:54:49', 'rent_end_cost': '2023-02-07 14:13:51', 'rent_time_cost': 170342.0, 'type': 'events_resource', 'resources': {'name': 'test1', 'entity': 'nvidia-pytorch', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63dfc338c037717bc232207e', 'tid_end': '63e25c9fc037717bc2322083', 'cost_total': 42585}]}]}",
         "code": 200,
         "time_stamp": "2023-02-09 12:28:28 ",
     }
     test_billing_invoice = (
         2023,
         1,
         {
@@ -403,15 +403,15 @@
                             {
                                 "rent_start": "2022-12-09 10:23:04",
                                 "rent_end": "2023-01-13 11:50:18",
                                 "rent_time": 3029234,
                                 "rent_start_cost": "2023-01-01 00:00:00",
                                 "rent_end_cost": "2023-01-13 11:50:18",
                                 "rent_time_cost": 1079418,
-                                "type": "events_compute",
+                                "type": "events_resource",
                                 "resources": {
                                     "name": "test",
                                     "entity": "tensorflow-jupyter",
                                     "cpu": 1,
                                     "memory": 2,
                                     "gpu": 0,
                                     "gpu_type": None,
@@ -423,15 +423,15 @@
                             {
                                 "rent_start": "2023-01-16 12:01:17",
                                 "rent_end": "2023-01-16 13:09:10",
                                 "rent_time": 4073,
                                 "rent_start_cost": "2023-01-16 12:01:17",
                                 "rent_end_cost": "2023-01-16 13:09:10",
                                 "rent_time_cost": 4073,
-                                "type": "events_compute",
+                                "type": "events_resource",
                                 "resources": {
                                     "name": "test1",
                                     "entity": "datascience-jupyter",
                                     "cpu": 1,
                                     "memory": 2,
                                     "gpu": 0,
                                     "gpu_type": None,
@@ -443,15 +443,15 @@
                             {
                                 "rent_start": "2023-01-16 11:59:47",
                                 "rent_end": "2023-01-16 13:16:21",
                                 "rent_time": 4594,
                                 "rent_start_cost": "2023-01-16 11:59:47",
                                 "rent_end_cost": "2023-01-16 13:16:21",
                                 "rent_time_cost": 4594,
-                                "type": "events_compute",
+                                "type": "events_resource",
                                 "resources": {
                                     "name": "test12",
                                     "entity": "datascience-jupyter",
                                     "cpu": 1,
                                     "memory": 2,
                                     "gpu": 0,
                                     "gpu_type": None,
@@ -463,15 +463,15 @@
                             {
                                 "rent_start": "2023-01-16 12:49:05",
                                 "rent_end": "2023-01-16 13:16:30",
                                 "rent_time": 1645,
                                 "rent_start_cost": "2023-01-16 12:49:05",
                                 "rent_end_cost": "2023-01-16 13:16:30",
                                 "rent_time_cost": 1645,
-                                "type": "events_compute",
+                                "type": "events_resource",
                                 "resources": {
                                     "name": "test12324",
                                     "entity": "datascience-jupyter",
                                     "cpu": 1,
                                     "memory": 2,
                                     "gpu": 0,
                                     "gpu_type": None,
@@ -483,15 +483,15 @@
                             {
                                 "rent_start": "2023-01-16 13:09:59",
                                 "rent_end": "2023-01-16 13:16:41",
                                 "rent_time": 402,
                                 "rent_start_cost": "2023-01-16 13:09:59",
                                 "rent_end_cost": "2023-01-16 13:16:41",
                                 "rent_time_cost": 402,
-                                "type": "events_compute",
+                                "type": "events_resource",
                                 "resources": {
                                     "name": "test123243222",
                                     "entity": "datascience-jupyter",
                                     "cpu": 1,
                                     "memory": 2,
                                     "gpu": 0,
                                     "gpu_type": None,
@@ -503,15 +503,15 @@
                             {
                                 "rent_start": "2023-01-16 13:17:57",
                                 "rent_end": "2023-01-16 13:40:29",
                                 "rent_time": 1352,
                                 "rent_start_cost": "2023-01-16 13:17:57",
                                 "rent_end_cost": "2023-01-16 13:40:29",
                                 "rent_time_cost": 1352,
-                                "type": "events_compute",
+                                "type": "events_resource",
                                 "resources": {
                                     "name": "test5",
                                     "entity": "datascience-jupyter",
                                     "cpu": 1,
                                     "memory": 2,
                                     "gpu": 0,
                                     "gpu_type": None,
@@ -523,15 +523,15 @@
                             {
                                 "rent_start": "2023-01-16 13:28:41",
                                 "rent_end": "2023-01-16 13:40:32",
                                 "rent_time": 711,
                                 "rent_start_cost": "2023-01-16 13:28:41",
                                 "rent_end_cost": "2023-01-16 13:40:32",
                                 "rent_time_cost": 711,
-                                "type": "events_compute",
+                                "type": "events_resource",
                                 "resources": {
                                     "name": "test6",
                                     "entity": "datascience-jupyter",
                                     "cpu": 1,
                                     "memory": 2,
                                     "gpu": 0,
                                     "gpu_type": None,
@@ -543,15 +543,15 @@
                             {
                                 "rent_start": "2023-01-16 13:38:10",
                                 "rent_end": "2023-01-16 13:40:35",
                                 "rent_time": 145,
                                 "rent_start_cost": "2023-01-16 13:38:10",
                                 "rent_end_cost": "2023-01-16 13:40:35",
                                 "rent_time_cost": 145,
-                                "type": "events_compute",
+                                "type": "events_resource",
                                 "resources": {
                                     "name": "test7",
                                     "entity": "datascience-jupyter",
                                     "cpu": 1,
                                     "memory": 2,
                                     "gpu": 0,
                                     "gpu_type": None,
@@ -563,15 +563,15 @@
                             {
                                 "rent_start": "2023-01-16 11:06:03",
                                 "rent_end": "2023-01-16 13:40:46",
                                 "rent_time": 9283,
                                 "rent_start_cost": "2023-01-16 11:06:03",
                                 "rent_end_cost": "2023-01-16 13:40:46",
                                 "rent_time_cost": 9283,
-                                "type": "events_compute",
+                                "type": "events_resource",
                                 "resources": {
                                     "name": "test",
                                     "entity": "datascience-jupyter",
                                     "cpu": 1,
                                     "memory": 2,
                                     "gpu": 0,
                                     "gpu_type": None,
@@ -606,15 +606,15 @@
                                 "cost_total": 82000,
                             }
                         ],
                     },
                 ],
                 "date_requested": {"year": 2023, "month": 1},
             },
-            "message": "{'namespace': 'pytest', 'cost_total': 87508.3, 'invoice': [{'user_id': 'e57c8668-6bc3-47c7-85de-903bfc3772b7', 'month': 1, 'year': 2023, 'cost_total': 5508.300000000001, 'details': [{'rent_start': '2022-12-09 10:23:04', 'rent_end': '2023-01-13 11:50:18', 'rent_time': 3029234.0, 'rent_start_cost': '2023-01-01 00:00:00', 'rent_end_cost': '2023-01-13 11:50:18', 'rent_time_cost': 1079418.0, 'type': 'events_compute', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63930c8a0fd5a2fe98fe5d51', 'tid_end': '63c14579c037717bc2321fad', 'cost_total': 5397.0}, {'rent_start': '2023-01-16 12:01:17', 'rent_end': '2023-01-16 13:09:10', 'rent_time': 4073.0, 'rent_start_cost': '2023-01-16 12:01:17', 'rent_end_cost': '2023-01-16 13:09:10', 'rent_time_cost': 4073.0, 'type': 'events_compute', 'resources': {'name': 'test1', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c53c8cc037717bc2321fc6', 'tid_end': '63c54c75c037717bc2321fd5', 'cost_total': 20.400000000000002}, {'rent_start': '2023-01-16 11:59:47', 'rent_end': '2023-01-16 13:16:21', 'rent_time': 4594.0, 'rent_start_cost': '2023-01-16 11:59:47', 'rent_end_cost': '2023-01-16 13:16:21', 'rent_time_cost': 4594.0, 'type': 'events_compute', 'resources': {'name': 'test12', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c53c32c037717bc2321fc4', 'tid_end': '63c54e25c037717bc2321fe0', 'cost_total': 23.1}, {'rent_start': '2023-01-16 12:49:05', 'rent_end': '2023-01-16 13:16:30', 'rent_time': 1645.0, 'rent_start_cost': '2023-01-16 12:49:05', 'rent_end_cost': '2023-01-16 13:16:30', 'rent_time_cost': 1645.0, 'type': 'events_compute', 'resources': {'name': 'test12324', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c547c1c037717bc2321fcb', 'tid_end': '63c54e2dc037717bc2321fe4', 'cost_total': 8.100000000000001}, {'rent_start': '2023-01-16 13:09:59', 'rent_end': '2023-01-16 13:16:41', 'rent_time': 402.0, 'rent_start_cost': '2023-01-16 13:09:59', 'rent_end_cost': '2023-01-16 13:16:41', 'rent_time_cost': 402.0, 'type': 'events_compute', 'resources': {'name': 'test123243222', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c54ca6c037717bc2321fd6', 'tid_end': '63c54e38c037717bc2321fe6', 'cost_total': 2.1}, {'rent_start': '2023-01-16 13:17:57', 'rent_end': '2023-01-16 13:40:29', 'rent_time': 1352.0, 'rent_start_cost': '2023-01-16 13:17:57', 'rent_end_cost': '2023-01-16 13:40:29', 'rent_time_cost': 1352.0, 'type': 'events_compute', 'resources': {'name': 'test5', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c54e85c037717bc2321fe8', 'tid_end': '63c553ccc037717bc2321ff5', 'cost_total': 6.9}, {'rent_start': '2023-01-16 13:28:41', 'rent_end': '2023-01-16 13:40:32', 'rent_time': 711.0, 'rent_start_cost': '2023-01-16 13:28:41', 'rent_end_cost': '2023-01-16 13:40:32', 'rent_time_cost': 711.0, 'type': 'events_compute', 'resources': {'name': 'test6', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c55109c037717bc2321feb', 'tid_end': '63c553d0c037717bc2321ff7', 'cost_total': 3.6000000000000005}, {'rent_start': '2023-01-16 13:38:10', 'rent_end': '2023-01-16 13:40:35', 'rent_time': 145.0, 'rent_start_cost': '2023-01-16 13:38:10', 'rent_end_cost': '2023-01-16 13:40:35', 'rent_time_cost': 145.0, 'type': 'events_compute', 'resources': {'name': 'test7', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c55341c037717bc2321ff2', 'tid_end': '63c553d3c037717bc2321ff9', 'cost_total': 0.6000000000000001}, {'rent_start': '2023-01-16 11:06:03', 'rent_end': '2023-01-16 13:40:46', 'rent_time': 9283.0, 'rent_start_cost': '2023-01-16 11:06:03', 'rent_end_cost': '2023-01-16 13:40:46', 'rent_time_cost': 9283.0, 'type': 'events_compute', 'resources': {'name': 'test', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c52f9bc037717bc2321fb5', 'tid_end': '63c553ddc037717bc2321ffb', 'cost_total': 46.5}]}, {'user_id': '9a8b327c-1f27-4d79-a387-071cd0954cf9', 'month': 1, 'year': 2023, 'cost_total': 82000, 'details': [{'rent_start': '2023-01-03 12:40:08', 'rent_end': '2023-02-09 10:19:06', 'rent_time': 3188338.545678, 'rent_start_cost': '2023-01-03 12:40:08', 'rent_end_cost': '2023-01-31 23:59:59', 'rent_time_cost': 2459991.0, 'type': 'events_volume', 'resources': {'name': 'test', 'disks_type': 'ssd', 'size': 1}, 'tid_start': '63dd00a8c037717bc232201d', 'tid_end': None, 'cost_total': 82000}]}], 'date_requested': {'year': 2023, 'month': 1}}",
+            "message": "{'namespace': 'pytest', 'cost_total': 87508.3, 'invoice': [{'user_id': 'e57c8668-6bc3-47c7-85de-903bfc3772b7', 'month': 1, 'year': 2023, 'cost_total': 5508.300000000001, 'details': [{'rent_start': '2022-12-09 10:23:04', 'rent_end': '2023-01-13 11:50:18', 'rent_time': 3029234.0, 'rent_start_cost': '2023-01-01 00:00:00', 'rent_end_cost': '2023-01-13 11:50:18', 'rent_time_cost': 1079418.0, 'type': 'events_resource', 'resources': {'name': 'test', 'entity': 'tensorflow-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63930c8a0fd5a2fe98fe5d51', 'tid_end': '63c14579c037717bc2321fad', 'cost_total': 5397.0}, {'rent_start': '2023-01-16 12:01:17', 'rent_end': '2023-01-16 13:09:10', 'rent_time': 4073.0, 'rent_start_cost': '2023-01-16 12:01:17', 'rent_end_cost': '2023-01-16 13:09:10', 'rent_time_cost': 4073.0, 'type': 'events_resource', 'resources': {'name': 'test1', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c53c8cc037717bc2321fc6', 'tid_end': '63c54c75c037717bc2321fd5', 'cost_total': 20.400000000000002}, {'rent_start': '2023-01-16 11:59:47', 'rent_end': '2023-01-16 13:16:21', 'rent_time': 4594.0, 'rent_start_cost': '2023-01-16 11:59:47', 'rent_end_cost': '2023-01-16 13:16:21', 'rent_time_cost': 4594.0, 'type': 'events_resource', 'resources': {'name': 'test12', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c53c32c037717bc2321fc4', 'tid_end': '63c54e25c037717bc2321fe0', 'cost_total': 23.1}, {'rent_start': '2023-01-16 12:49:05', 'rent_end': '2023-01-16 13:16:30', 'rent_time': 1645.0, 'rent_start_cost': '2023-01-16 12:49:05', 'rent_end_cost': '2023-01-16 13:16:30', 'rent_time_cost': 1645.0, 'type': 'events_resource', 'resources': {'name': 'test12324', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c547c1c037717bc2321fcb', 'tid_end': '63c54e2dc037717bc2321fe4', 'cost_total': 8.100000000000001}, {'rent_start': '2023-01-16 13:09:59', 'rent_end': '2023-01-16 13:16:41', 'rent_time': 402.0, 'rent_start_cost': '2023-01-16 13:09:59', 'rent_end_cost': '2023-01-16 13:16:41', 'rent_time_cost': 402.0, 'type': 'events_resource', 'resources': {'name': 'test123243222', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c54ca6c037717bc2321fd6', 'tid_end': '63c54e38c037717bc2321fe6', 'cost_total': 2.1}, {'rent_start': '2023-01-16 13:17:57', 'rent_end': '2023-01-16 13:40:29', 'rent_time': 1352.0, 'rent_start_cost': '2023-01-16 13:17:57', 'rent_end_cost': '2023-01-16 13:40:29', 'rent_time_cost': 1352.0, 'type': 'events_resource', 'resources': {'name': 'test5', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c54e85c037717bc2321fe8', 'tid_end': '63c553ccc037717bc2321ff5', 'cost_total': 6.9}, {'rent_start': '2023-01-16 13:28:41', 'rent_end': '2023-01-16 13:40:32', 'rent_time': 711.0, 'rent_start_cost': '2023-01-16 13:28:41', 'rent_end_cost': '2023-01-16 13:40:32', 'rent_time_cost': 711.0, 'type': 'events_resource', 'resources': {'name': 'test6', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c55109c037717bc2321feb', 'tid_end': '63c553d0c037717bc2321ff7', 'cost_total': 3.6000000000000005}, {'rent_start': '2023-01-16 13:38:10', 'rent_end': '2023-01-16 13:40:35', 'rent_time': 145.0, 'rent_start_cost': '2023-01-16 13:38:10', 'rent_end_cost': '2023-01-16 13:40:35', 'rent_time_cost': 145.0, 'type': 'events_resource', 'resources': {'name': 'test7', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c55341c037717bc2321ff2', 'tid_end': '63c553d3c037717bc2321ff9', 'cost_total': 0.6000000000000001}, {'rent_start': '2023-01-16 11:06:03', 'rent_end': '2023-01-16 13:40:46', 'rent_time': 9283.0, 'rent_start_cost': '2023-01-16 11:06:03', 'rent_end_cost': '2023-01-16 13:40:46', 'rent_time_cost': 9283.0, 'type': 'events_resource', 'resources': {'name': 'test', 'entity': 'datascience-jupyter', 'cpu': 1, 'memory': 2, 'gpu': 0, 'gpu_type': None}, 'tid_start': '63c52f9bc037717bc2321fb5', 'tid_end': '63c553ddc037717bc2321ffb', 'cost_total': 46.5}]}, {'user_id': '9a8b327c-1f27-4d79-a387-071cd0954cf9', 'month': 1, 'year': 2023, 'cost_total': 82000, 'details': [{'rent_start': '2023-01-03 12:40:08', 'rent_end': '2023-02-09 10:19:06', 'rent_time': 3188338.545678, 'rent_start_cost': '2023-01-03 12:40:08', 'rent_end_cost': '2023-01-31 23:59:59', 'rent_time_cost': 2459991.0, 'type': 'events_volume', 'resources': {'name': 'test', 'disks_type': 'ssd', 'size': 1}, 'tid_start': '63dd00a8c037717bc232201d', 'tid_end': None, 'cost_total': 82000}]}], 'date_requested': {'year': 2023, 'month': 1}}",
             "code": 200,
             "time_stamp": "2023-02-10 10:58:38 ",
         },
     )
     test_billing_invoice_empty = (
         2022,
         11,
@@ -636,15 +636,15 @@
                 "date_requested": {"year": 2022, "month": 11},
             },
             "message": "{'namespace': 'pytest', 'cost_total': 0, 'invoice': [{'user_id': 'e57c8668-6bc3-47c7-85de-903bfc3772b7', 'month': 11, 'year': 2022, 'cost_total': 0, 'details': []}], 'date_requested': {'year': 2022, 'month': 11}}",
             "code": 200,
             "time_stamp": "2023-02-10 11:01:44 ",
         },
     )
-    test_billing_stop_events_compute = {
+    test_billing_stop_events_resource = {
         "status": "Success",
         "reason": "LIST_COMPUTE_STOP_EVENTS",
         "details": {
             "event_list": [
                 {
                     "event_id": "634e539ee2dc201119f13f97",
                     "date_created": "2022-10-18 07:19:59",
@@ -680,15 +680,15 @@
         "status": "Success",
         "reason": "LIST_STORAGE_STOP_EVENTS",
         "details": {"event_list": []},
         "message": "{'event_list': []}",
         "code": 200,
         "time_stamp": "2023-02-06 13:28:39 ",
     }
-    test_billing_no_stop_events_compute = {
+    test_billing_no_stop_events_resource = {
         "status": "Success",
         "reason": "LIST_COMPUTE_STOP_EVENTS",
         "details": {"event_list": []},
         "message": "{'event_list': []}",
         "code": 200,
         "time_stamp": "2023-02-06 13:28:39 ",
     }
@@ -839,15 +839,15 @@
         },
         "message": "{'namespace': 'pytest', 'created_template': {'name': 'test', 'labels': {'entity': 'tensorflow-jupyter'}, 'pod_url': 'https://test.pytest.dev.quantdevlabs.com', 'replicas': 1, 'app_token': '2da1723c002f467881aabd10c66e54cf'}, 'mount_start_path': '/tf', 'mounted_pvc_list': [], 'status': 'PVC NOT FOUND', 'created_service': {'name': 'test', 'labels': {'entity': 'tensorflow-jupyter'}, 'ports': [{'port': 8888, 'protocol': 'TCP'}]}, 'modified_certificate': {'warning': 'running in development mode, not managing certificate'}, 'modified_ingress': {'name': 'pytest-ingress', 'labels': None, 'rules': ['filebrowser.pytest.dev.quantdevlabs.com', 'test.pytest.dev.quantdevlabs.com']}}",
         "code": 200,
         "time_stamp": "2023-02-06 13:28:39 ",
     }
     test_compute_template_list = {
         "status": "Success",
-        "reason": "COMPUTE_LIST_AVAILABLE_TEMPLATES",
+        "reason": "RESOURCE_LIST_AVAILABLE_TEMPLATES",
         "details": {
             "namespace": "pytest",
             "available_templates_list": [
                 "tensorflow-jupyter",
                 "datascience-jupyter",
                 "nvidia-rapids",
                 "nvidia-pytorch",
@@ -933,26 +933,26 @@
             'modified_ingress': {'name': 'pytest-ingress', 'labels': None,\
             'rules': ['test2.pytest.dev.quantdevlabs.com', 'filebrowser.pytest.dev.quantdevlabs.com']}}",
         "code": 200,
         "time_stamp": "2023-02-03 16:24:59 ",
     }
     test_compute_list_empty = {
         "status": "Success",
-        "reason": "COMPUTE_LIST",
+        "reason": "RESOURCE_LIST",
         "details": {
             "namespace": "pytest",
             "pods_list": [],
         },
         "message": "{'namespace': 'pytest', 'pods_list': []]}",
         "code": 200,
         "time_stamp": "2023-02-03 16:24:59 ",
     }
     test_compute_list_no_labels = {
         "status": "Success",
-        "reason": "COMPUTE_LIST",
+        "reason": "RESOURCE_LIST",
         "details": {
             "namespace": "comtegra",
             "pods_list": [
                 {
                     "labels": {"gpu-count": "2", "gpu-label": "A100"},
                     "name": "roberta-5476f5bcb7-cqnq8",
                     "status": "Running",
@@ -1517,15 +1517,15 @@
                     ],
                 },
             ],
         },
     ]
     test_compute_list = {
         "status": "Success",
-        "reason": "COMPUTE_LIST",
+        "reason": "RESOURCE_LIST",
         "details": {
             "namespace": "pytest",
             "pods_list": [
                 {
                     "labels": {
                         "app-name": "filebrowser",
                         "app-token": "9bb9c88f8fc14eadba5c5fbdafc06275",
@@ -1781,22 +1781,22 @@
         return f.read()
 
 
 class DesiredResponsesData:
     test_billing_status = get_desired_response_data("test_billing_status.txt")
     test_billing_invoice = get_desired_response_data("test_billing_invoice.txt")
     test_billing_invoice_empty = "[33mNo invoice found for 11.2022.[0m"
-    test_billing_stop_events_compute = get_desired_response_data(
-        "test_billing_stop_events_compute.txt"
+    test_billing_stop_events_resource = get_desired_response_data(
+        "test_billing_stop_events_resource.txt"
     )
     test_billing_stop_events_volume = get_desired_response_data(
         "test_billing_stop_events_volume.txt"
     )
     test_billing_no_stop_events_volume = "[33mNo volume stop events to list.[0m"
-    test_billing_no_stop_events_compute = "[33mNo compute stop events to list.[0m"
+    test_billing_no_stop_events_resource = "[33mNo compute stop events to list.[0m"
     test_volume_list = get_desired_response_data("test_volume_list.txt")
     test_volume_list_empty = "[33mNo volumes to list.[0m"
     test_volume_create = (
         "Volume test1 of size 1.0 GB on SSD created. Volume is ReadWriteMany."
     )
     test_volume_delete = "Volume test1 deleted."
     test_volume_unmount = "Volume test1 successfully unmounted from selected apps."
@@ -1812,15 +1812,15 @@
         "Username: pytest\n"
         "Password: 9bb9c88f8fc14eadba5c5fbdafc06275"
     )
     test_compute_create = (
         "nvidia-pytorch app test1 creation started!\n"
         "Will be accessible at: https://test1.pytest.dev.quantdevlabs.com\n"
         "App token: 1ce03c31ab9c40df8594d97b301eaaea\n"
-        "To monitor the startup status use command: cgc compute list"
+        "To monitor the startup status use command: cgc resource list"
     )
     test_compute_create_no_volume_found = "[33mVolume name not found in namespace.[0m"
     test_compute_delete = "App test1 and its service successfully deleted."
     test_compute_restart = "App test1 has been successfully restarted."
     test_compute_list = get_desired_response_data("test_compute_list.txt")
     test_compute_template_list = "Available templates: tensorflow-jupyter, datascience-jupyter, nvidia-rapids, nvidia-pytorch, nvidia-tensorflow"
     test_tabulate_a_response = get_desired_response_data("test_tabulate_response.txt")
```

### Comparing `cgcsdk-0.7.1/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-0.8.0/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-0.8.0/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-0.8.0/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/tests/responses_tests.py` & `cgcsdk-0.8.0/cgc/tests/responses_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     compute_list_response,
     template_list_response,
     template_get_start_path_response,
 )
 from cgc.commands.billing.billing_responses import (
     billing_status_response,
     billing_invoice_response,
-    stop_events_compute_response,
+    stop_events_resource_response,
     stop_events_volume_response,
 )
 from cgc.utils.response_utils import (
     tabulate_a_response,
     fill_missing_values_in_a_response,
 )
 from cgc.commands.compute.compute_utills import get_app_list
@@ -126,19 +126,19 @@
         result = billing_invoice_response(*ResponsesData.test_billing_invoice)
         self.assertEqual(result, DesiredResponsesData.test_billing_invoice)
 
     def test_billing_invoice_empty(self):
         result = billing_invoice_response(*ResponsesData.test_billing_invoice_empty)
         self.assertEqual(result, DesiredResponsesData.test_billing_invoice_empty)
 
-    def test_billing_stop_events_compute(self):
-        result = stop_events_compute_response(
-            ResponsesData.test_billing_stop_events_compute
+    def test_billing_stop_events_resource(self):
+        result = stop_events_resource_response(
+            ResponsesData.test_billing_stop_events_resource
         )
-        self.assertEqual(result, DesiredResponsesData.test_billing_stop_events_compute)
+        self.assertEqual(result, DesiredResponsesData.test_billing_stop_events_resource)
 
     def test_billing_stop_events_volume(self):
         result = stop_events_volume_response(
             ResponsesData.test_billing_stop_events_volume
         )
         self.assertEqual(result, DesiredResponsesData.test_billing_stop_events_volume)
 
@@ -146,20 +146,20 @@
         result = stop_events_volume_response(
             ResponsesData.test_billing_no_stop_events_volume
         )
         self.assertEqual(
             result, DesiredResponsesData.test_billing_no_stop_events_volume
         )
 
-    def test_billing_no_stop_events_compute(self):
-        result = stop_events_compute_response(
-            ResponsesData.test_billing_no_stop_events_compute
+    def test_billing_no_stop_events_resource(self):
+        result = stop_events_resource_response(
+            ResponsesData.test_billing_no_stop_events_resource
         )
         self.assertEqual(
-            result, DesiredResponsesData.test_billing_no_stop_events_compute
+            result, DesiredResponsesData.test_billing_no_stop_events_resource
         )
 
 
 # WIP
 class TestUtils(unittest.TestCase):
     def test_fill_missing_values_in_response(self):
         result = fill_missing_values_in_a_response(
```

### Comparing `cgcsdk-0.7.1/cgc/utils/click_group.py` & `cgcsdk-0.8.0/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/config_utils.py` & `cgcsdk-0.8.0/cgc/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/consts/env_consts.py` & `cgcsdk-0.8.0/cgc/utils/consts/env_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/consts/message_consts.py` & `cgcsdk-0.8.0/cgc/utils/consts/message_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-0.8.0/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-0.8.0/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-0.8.0/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/custom_exceptions.py` & `cgcsdk-0.8.0/cgc/utils/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/message_utils.py` & `cgcsdk-0.8.0/cgc/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/prepare_headers.py` & `cgcsdk-0.8.0/cgc/utils/prepare_headers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/requests_helper.py` & `cgcsdk-0.8.0/cgc/utils/requests_helper.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/response_utils.py` & `cgcsdk-0.8.0/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgc/utils/version_control.py` & `cgcsdk-0.8.0/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.7.1/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-0.8.0/cgcsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.7.1
+Version: 0.8.0
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.7.1/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-0.8.0/cgcsdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,20 @@
 cgc/commands/billing/billing_responses.py
 cgc/commands/billing/billing_utils.py
 cgc/commands/compute/__init__.py
 cgc/commands/compute/compute_cmd.py
 cgc/commands/compute/compute_models.py
 cgc/commands/compute/compute_responses.py
 cgc/commands/compute/compute_utills.py
+cgc/commands/db/__init__.py
+cgc/commands/db/db_cmd.py
 cgc/commands/debug/__init__.py
 cgc/commands/debug/debug_cmd.py
+cgc/commands/resource/__init__.py
+cgc/commands/resource/resource_cmd.py
 cgc/commands/volume/__init__.py
 cgc/commands/volume/data_model.py
 cgc/commands/volume/volume_cmd.py
 cgc/commands/volume/volume_responses.py
 cgc/commands/volume/volume_utils.py
 cgc/telemetry/__init__.py
 cgc/telemetry/basic.py
```

### Comparing `cgcsdk-0.7.1/setup.py` & `cgcsdk-0.8.0/setup.py`

 * *Files identical despite different names*

