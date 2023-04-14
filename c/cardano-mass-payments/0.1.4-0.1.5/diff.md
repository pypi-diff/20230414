# Comparing `tmp/cardano-mass-payments-0.1.4.tar.gz` & `tmp/cardano-mass-payments-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardano-mass-payments-0.1.4.tar", last modified: Fri Mar 31 09:01:55 2023, max compression
+gzip compressed data, was "cardano-mass-payments-0.1.5.tar", last modified: Fri Apr 14 05:30:32 2023, max compression
```

## Comparing `cardano-mass-payments-0.1.4.tar` & `cardano-mass-payments-0.1.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.207505 cardano-mass-payments-0.1.4/
--rw-rw-r--   0 francis   (1000) francis   (1000)    35149 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/LICENSE
--rw-rw-r--   0 francis   (1000) francis   (1000)    21186 2023-03-31 09:01:55.207505 cardano-mass-payments-0.1.4/PKG-INFO
--rw-rw-r--   0 francis   (1000) francis   (1000)    20397 2023-03-13 14:14:31.000000 cardano-mass-payments-0.1.4/README.md
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.199505 cardano-mass-payments-0.1.4/cardano_mass_payments/
--rw-rw-r--   0 francis   (1000) francis   (1000)       77 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)       96 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/cache.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    14775 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/classes.py
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.203505 cardano-mass-payments-0.1.4/cardano_mass_payments/commands/
--rw-rw-r--   0 francis   (1000) francis   (1000)       28 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/commands/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    26315 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/commands/mass_payments.py
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.203505 cardano-mass-payments-0.1.4/cardano_mass_payments/constants/
--rw-rw-r--   0 francis   (1000) francis   (1000)       47 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/constants/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     7228 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/constants/commands.py
--rw-rw-r--   0 francis   (1000) francis   (1000)      981 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/constants/common.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     2983 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/constants/exceptions.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     1541 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/settings.py
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.203505 cardano-mass-payments-0.1.4/cardano_mass_payments/utils/
--rw-rw-r--   0 francis   (1000) francis   (1000)       69 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/utils/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    52965 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/utils/cli_utils.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     2394 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/utils/common.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     5287 2023-03-14 11:07:49.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/utils/pycardano_utils.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    66406 2023-03-31 08:50:15.000000 cardano-mass-payments-0.1.4/cardano_mass_payments/utils/script_utils.py
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.203505 cardano-mass-payments-0.1.4/cardano_mass_payments.egg-info/
--rw-rw-r--   0 francis   (1000) francis   (1000)    21186 2023-03-31 09:01:55.000000 cardano-mass-payments-0.1.4/cardano_mass_payments.egg-info/PKG-INFO
--rw-rw-r--   0 francis   (1000) francis   (1000)     2276 2023-03-31 09:01:55.000000 cardano-mass-payments-0.1.4/cardano_mass_payments.egg-info/SOURCES.txt
--rw-rw-r--   0 francis   (1000) francis   (1000)        1 2023-03-31 09:01:55.000000 cardano-mass-payments-0.1.4/cardano_mass_payments.egg-info/dependency_links.txt
--rw-rw-r--   0 francis   (1000) francis   (1000)      101 2023-03-31 09:01:55.000000 cardano-mass-payments-0.1.4/cardano_mass_payments.egg-info/entry_points.txt
--rw-rw-r--   0 francis   (1000) francis   (1000)       17 2023-03-31 09:01:55.000000 cardano-mass-payments-0.1.4/cardano_mass_payments.egg-info/requires.txt
--rw-rw-r--   0 francis   (1000) francis   (1000)       28 2023-03-31 09:01:55.000000 cardano-mass-payments-0.1.4/cardano_mass_payments.egg-info/top_level.txt
--rw-rw-r--   0 francis   (1000) francis   (1000)      140 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/pyproject.toml
--rw-rw-r--   0 francis   (1000) francis   (1000)     1680 2023-03-31 09:01:55.207505 cardano-mass-payments-0.1.4/setup.cfg
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.203505 cardano-mass-payments-0.1.4/tests/
--rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     1069 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/tests/mock_responses.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    13201 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/tests/mock_utils.py
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.207505 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/
--rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    10717 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_create_transaction_command.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     9017 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_create_transaction_file.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     3151 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_latest_slot_number.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     3526 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_protocol_parameters.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     3140 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_stake_address_balance.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     3487 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_staking_address.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    13976 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_total_amount_plus_fee.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    26908 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_transaction_byte_size.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     7129 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_transaction_fee.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     3702 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_utxo_hash.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     8175 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_wallet_utxo.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     7405 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_sign_tx_file.py
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.207505 cardano-mass-payments-0.1.4/tests/test_process/
--rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_process/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    61880 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.4/tests/test_process/test_script_process.py
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-03-31 09:01:55.207505 cardano-mass-payments-0.1.4/tests/test_script_function_tests/
--rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_script_function_tests/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    31364 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_adjust_utxos.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    28933 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_dust_collect.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    33235 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_generate_bash_script.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     8694 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_group_output_utxo.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     2341 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_parse_payment_utxo_file.py
--rw-rw-r--   0 francis   (1000) francis   (1000)     2850 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_parse_sources_csv_file.py
--rw-rw-r--   0 francis   (1000) francis   (1000)    22424 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_preparation_step.py
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.912939 cardano-mass-payments-0.1.5/
+-rw-rw-r--   0 francis   (1000) francis   (1000)    35149 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/LICENSE
+-rw-rw-r--   0 francis   (1000) francis   (1000)    21607 2023-04-14 05:30:32.912939 cardano-mass-payments-0.1.5/PKG-INFO
+-rw-rw-r--   0 francis   (1000) francis   (1000)    20818 2023-04-07 15:16:44.000000 cardano-mass-payments-0.1.5/README.md
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.900933 cardano-mass-payments-0.1.5/cardano_mass_payments/
+-rw-rw-r--   0 francis   (1000) francis   (1000)       77 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/__init__.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)       96 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/cache.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    14775 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/classes.py
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.904935 cardano-mass-payments-0.1.5/cardano_mass_payments/commands/
+-rw-rw-r--   0 francis   (1000) francis   (1000)       28 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/commands/__init__.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    26713 2023-04-03 12:53:22.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/commands/mass_payments.py
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.904935 cardano-mass-payments-0.1.5/cardano_mass_payments/constants/
+-rw-rw-r--   0 francis   (1000) francis   (1000)       47 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/constants/__init__.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     7228 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/constants/commands.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)      981 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/constants/common.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     2983 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/constants/exceptions.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     1541 2023-04-07 15:19:13.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/settings.py
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.904935 cardano-mass-payments-0.1.5/cardano_mass_payments/utils/
+-rw-rw-r--   0 francis   (1000) francis   (1000)       69 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/utils/__init__.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    52965 2023-04-03 13:26:27.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/utils/cli_utils.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     2394 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/utils/common.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     5287 2023-04-03 11:21:31.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/utils/pycardano_utils.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    66665 2023-04-03 15:12:07.000000 cardano-mass-payments-0.1.5/cardano_mass_payments/utils/script_utils.py
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.904935 cardano-mass-payments-0.1.5/cardano_mass_payments.egg-info/
+-rw-rw-r--   0 francis   (1000) francis   (1000)    21607 2023-04-14 05:30:32.000000 cardano-mass-payments-0.1.5/cardano_mass_payments.egg-info/PKG-INFO
+-rw-rw-r--   0 francis   (1000) francis   (1000)     2276 2023-04-14 05:30:32.000000 cardano-mass-payments-0.1.5/cardano_mass_payments.egg-info/SOURCES.txt
+-rw-rw-r--   0 francis   (1000) francis   (1000)        1 2023-04-14 05:30:32.000000 cardano-mass-payments-0.1.5/cardano_mass_payments.egg-info/dependency_links.txt
+-rw-rw-r--   0 francis   (1000) francis   (1000)      101 2023-04-14 05:30:32.000000 cardano-mass-payments-0.1.5/cardano_mass_payments.egg-info/entry_points.txt
+-rw-rw-r--   0 francis   (1000) francis   (1000)       17 2023-04-14 05:30:32.000000 cardano-mass-payments-0.1.5/cardano_mass_payments.egg-info/requires.txt
+-rw-rw-r--   0 francis   (1000) francis   (1000)       28 2023-04-14 05:30:32.000000 cardano-mass-payments-0.1.5/cardano_mass_payments.egg-info/top_level.txt
+-rw-rw-r--   0 francis   (1000) francis   (1000)      140 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/pyproject.toml
+-rw-rw-r--   0 francis   (1000) francis   (1000)     1680 2023-04-14 05:30:32.912939 cardano-mass-payments-0.1.5/setup.cfg
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.904935 cardano-mass-payments-0.1.5/tests/
+-rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/__init__.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     1069 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/tests/mock_responses.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    13201 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/tests/mock_utils.py
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.904935 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/
+-rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/__init__.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    10717 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_create_transaction_command.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     9017 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_create_transaction_file.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     3151 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_latest_slot_number.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     3526 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_protocol_parameters.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     3140 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_stake_address_balance.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     3487 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_staking_address.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    13976 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_total_amount_plus_fee.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    26908 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_transaction_byte_size.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     7129 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_transaction_fee.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     3702 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_utxo_hash.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     8175 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_wallet_utxo.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     7405 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_sign_tx_file.py
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.912939 cardano-mass-payments-0.1.5/tests/test_process/
+-rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_process/__init__.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    64251 2023-04-07 15:19:08.000000 cardano-mass-payments-0.1.5/tests/test_process/test_script_process.py
+drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-04-14 05:30:32.912939 cardano-mass-payments-0.1.5/tests/test_script_function_tests/
+-rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_script_function_tests/__init__.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    31364 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_adjust_utxos.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    28933 2023-03-13 14:11:24.000000 cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_dust_collect.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    33235 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_generate_bash_script.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     8694 2023-03-13 14:11:21.000000 cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_group_output_utxo.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     2341 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_parse_payment_utxo_file.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)     2850 2023-02-17 09:56:27.000000 cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_parse_sources_csv_file.py
+-rw-rw-r--   0 francis   (1000) francis   (1000)    24545 2023-04-03 15:04:24.000000 cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_preparation_step.py
```

### Comparing `cardano-mass-payments-0.1.4/LICENSE` & `cardano-mass-payments-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/PKG-INFO` & `cardano-mass-payments-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-mass-payments
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool for handling mass payments for Cardano (ADA)
 Home-page: https://github.com/adaplus/cardano-mass-payments
 Author: ADAPlus
 Author-email: hello@adaplus.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -109,15 +109,15 @@
 | `--source-address`            | Primary Source Address (should be in the `--sources-csv` file). If not provided, will use the first address in the `--sources-csv` file.                                                                                                                                                                                                                                                          |
 | `--source-signing-key-file`   | Signing Key File of Primary Source Address. If not provided, will use the corresponding signing key file of the primary source address in the `--sources-csv` file.                                                                                                                                                                                                                               |
 | `--metadata-json-file`        | JSON File containing the metadata template that will be included in the cardano transaction.                                                                                                                                                                                                                                                                                                      |
 | `--metadata-message-file`     | TXT File containing the message that will be added in the transaction metadata.                                                                                                                                                                                                                                                                                                                   |
 | `--transaction-plan-file`     | TXT Transaction Plan File which can be used to generate the script.                                                                                                                                                                                                                                                                                                                               |
 | `--magic-number`              | Cardano Network Magic Number where the python script will connect to.                                                                                                                                                                                                                                                                                                                             |
 | `--cardano-node-docker-image` | Docker Image name of the Cardano node.                                                                                                                                                                                                                                                                                                                                                            |
-
+| `--reward-withdrawal-amount`  | Amount of lovelace that will be withdrawn from the source's rewards                                                                                                                                                                                                                                                                                                                               |
 
 #### Flag Details
 
 
 
 | **Flag**                         | **Description**                                                                                                         |
 |----------------------------------|-------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `cardano-mass-payments-0.1.4/README.md` & `cardano-mass-payments-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 | `--source-address`            | Primary Source Address (should be in the `--sources-csv` file). If not provided, will use the first address in the `--sources-csv` file.                                                                                                                                                                                                                                                          |
 | `--source-signing-key-file`   | Signing Key File of Primary Source Address. If not provided, will use the corresponding signing key file of the primary source address in the `--sources-csv` file.                                                                                                                                                                                                                               |
 | `--metadata-json-file`        | JSON File containing the metadata template that will be included in the cardano transaction.                                                                                                                                                                                                                                                                                                      |
 | `--metadata-message-file`     | TXT File containing the message that will be added in the transaction metadata.                                                                                                                                                                                                                                                                                                                   |
 | `--transaction-plan-file`     | TXT Transaction Plan File which can be used to generate the script.                                                                                                                                                                                                                                                                                                                               |
 | `--magic-number`              | Cardano Network Magic Number where the python script will connect to.                                                                                                                                                                                                                                                                                                                             |
 | `--cardano-node-docker-image` | Docker Image name of the Cardano node.                                                                                                                                                                                                                                                                                                                                                            |
-
+| `--reward-withdrawal-amount`  | Amount of lovelace that will be withdrawn from the source's rewards                                                                                                                                                                                                                                                                                                                               |
 
 #### Flag Details
 
 
 
 | **Flag**                         | **Description**                                                                                                         |
 |----------------------------------|-------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/classes.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/classes.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/commands/mass_payments.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/commands/mass_payments.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,14 +355,15 @@
         "payments_csv_file": args.payments_csv,
         "transaction_plan_file": transaction_plan,
         "dust_collection_method": dust_collection_method,
         "dust_collection_threshold": dust_collection_threshold,
         "enable_dust_collection": args.enable_dust_collection,
         "enable_immediate_execution": args.execute_script_now,
         "include_rewards": args.include_rewards,
+        "reward_withdrawal_amount": args.reward_withdrawal_amount,
     }
 
 
 def generate_transaction_plan(
     output_format,
     source_address,
     source_details,
@@ -370,14 +371,15 @@
     cardano_network,
     script_method,
     allowed_ttl_slots,
     enable_dust_collection=False,
     dust_collection_method=DustCollectionMethod.COLLECT_TO_SOURCE,
     dust_collection_threshold=10000000,
     include_rewards=False,
+    reward_amount=-1,
 ):
     """
     Generate Transaction Plan
 
     :param output_format: Script Output Format
     :param source_address: Source Address
     :param source_details: Map containing Address + Signing Key File Details
@@ -385,24 +387,26 @@
     :param cardano_network: Network where the script connects to
     :param script_method: Method used in the script logic
     :param allowed_ttl_slots: Number of slots allowed before the transaction to be deemed invalid
     :param enable_dust_collection: Flag on whether to execute dust collection or not
     :param dust_collection_method: Method that will be used for dust collection
     :param dust_collection_threshold: Maximum amount that will be the basis for dust collection
     :param include_rewards: Flag on whether to include getting the stake rewards
+    :param reward_amount: Amount that will be withdrawn from rewards
     :return: TransactionPlan object
     """
     print_to_console("Creating Preparation TX and Initial Groupings...", output_format)
     init_details = preparation_step(
         source_address,
         source_details,
         payments_csv_file,
         network=cardano_network,
         method=script_method,
         include_rewards=include_rewards,
+        reward_amount=reward_amount,
     )
 
     if init_details.get("require_dust_collection"):
         if enable_dust_collection:
             init_details = dust_collect(
                 input_utxos=init_details.get("wallet_utxos"),
                 payment_group_details=init_details.get("output_details"),
@@ -640,14 +644,20 @@
         "--include-rewards",
         help="Include Main Source Address Stake Rewards",
         nargs="?",
         default=False,
         const=True,
     )
     parser.add_argument(
+        "--reward-withdrawal-amount",
+        help="Amount that will be withdrawn from the rewards (if include reward flags is set)",
+        type=int,
+        default=-1,
+    )
+    parser.add_argument(
         "--allowed-ttl-slots",
         help="Number of allowable slots for the Transaction TTL",
         type=int,
         default=1000,
     )
     parser.add_argument(
         "--magic-number",
```

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/constants/commands.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/constants/commands.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/constants/common.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/constants/common.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/constants/exceptions.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/constants/exceptions.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/settings.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/settings.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/utils/cli_utils.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/utils/common.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/utils/common.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/utils/pycardano_utils.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/utils/pycardano_utils.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments/utils/script_utils.py` & `cardano-mass-payments-0.1.5/cardano_mass_payments/utils/script_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,23 +188,25 @@
 def preparation_step(
     source_address,
     source_details,
     payments_utxo_file,
     network=CardanoNetwork.PREPROD,
     method=ScriptMethod.METHOD_DOCKER_CLI,
     include_rewards=False,
+    reward_amount=-1,
 ):
     """
     Prepare and create an initial input utxo transaction
     :param source_address: source address
     :param source_details: source details map (address + signing key file)
     :param payments_utxo_file: csv file containing payment utxo details
     :param network: Network where the function will get the cardano details
     :param method: Method that will be used for creating initial input transaction
     :param include_rewards: Flag on whether to include getting the stake rewards
+    :param reward_amount: Amount that will be withdrawn from rewards
     :return: initial groups + initial transaction details
     """
     if not isinstance(source_address, str):
         raise InvalidType(
             type=type(source_address),
             message="Invalid source address type.",
         )
@@ -219,14 +221,19 @@
             message="Invalid payments UTxO file type.",
         )
     if not isinstance(include_rewards, bool):
         raise InvalidType(
             type=type(include_rewards),
             message="Invalid include rewards type.",
         )
+    if not isinstance(reward_amount, int):
+        raise InvalidType(
+            type=type(reward_amount),
+            message="Invalid reward amount type.",
+        )
 
     # Parse File
     try:
         output_list = parse_payment_utxo_file(filename=payments_utxo_file)
     except ScriptError as e:
         raise e
     except Exception as e:
@@ -260,15 +267,15 @@
     stake_reward_details = {}
     if include_rewards:
         stake_address = get_staking_address(
             full_address=source_address,
             network=network,
             method=method,
         )
-        stake_balance = get_stake_address_balance(
+        stake_balance = reward_amount if reward_amount > 0 else get_stake_address_balance(
             stake_address=stake_address,
             network=network,
             method=method,
         )
         stake_reward_details = {
             "stake_address": stake_address,
             "stake_amount": stake_balance,
@@ -1032,15 +1039,14 @@
     prep_tx_submission_status = transaction_plan.prep_detail.submission_status
     reward_details = transaction_plan.prep_detail.reward_details
 
     # Set num_witness
     input_address_set = set()
     for input_utxo in prep_input_utxos:
         input_address_set.add(input_utxo.address)
-    num_witness = len(input_address_set)
 
     pycardano_context = CACHE_VALUES.get("pycardano_context")
 
     prefix = masspayments_settings.command_prefix(method)
     if method == ScriptMethod.METHOD_PYCARDANO:
         prefix = pycardano_context.command_prefix
     network_flag = masspayments_settings.network_flag(network)
```

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments.egg-info/PKG-INFO` & `cardano-mass-payments-0.1.5/cardano_mass_payments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-mass-payments
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool for handling mass payments for Cardano (ADA)
 Home-page: https://github.com/adaplus/cardano-mass-payments
 Author: ADAPlus
 Author-email: hello@adaplus.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -109,15 +109,15 @@
 | `--source-address`            | Primary Source Address (should be in the `--sources-csv` file). If not provided, will use the first address in the `--sources-csv` file.                                                                                                                                                                                                                                                          |
 | `--source-signing-key-file`   | Signing Key File of Primary Source Address. If not provided, will use the corresponding signing key file of the primary source address in the `--sources-csv` file.                                                                                                                                                                                                                               |
 | `--metadata-json-file`        | JSON File containing the metadata template that will be included in the cardano transaction.                                                                                                                                                                                                                                                                                                      |
 | `--metadata-message-file`     | TXT File containing the message that will be added in the transaction metadata.                                                                                                                                                                                                                                                                                                                   |
 | `--transaction-plan-file`     | TXT Transaction Plan File which can be used to generate the script.                                                                                                                                                                                                                                                                                                                               |
 | `--magic-number`              | Cardano Network Magic Number where the python script will connect to.                                                                                                                                                                                                                                                                                                                             |
 | `--cardano-node-docker-image` | Docker Image name of the Cardano node.                                                                                                                                                                                                                                                                                                                                                            |
-
+| `--reward-withdrawal-amount`  | Amount of lovelace that will be withdrawn from the source's rewards                                                                                                                                                                                                                                                                                                                               |
 
 #### Flag Details
 
 
 
 | **Flag**                         | **Description**                                                                                                         |
 |----------------------------------|-------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `cardano-mass-payments-0.1.4/cardano_mass_payments.egg-info/SOURCES.txt` & `cardano-mass-payments-0.1.5/cardano_mass_payments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/setup.cfg` & `cardano-mass-payments-0.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardano-mass-payments
-version = 0.1.4
+version = 0.1.5
 author = ADAPlus
 author_email = hello@adaplus.io
 description = A tool for handling mass payments for Cardano (ADA)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/adaplus/cardano-mass-payments
 classifiers =
```

### Comparing `cardano-mass-payments-0.1.4/tests/mock_responses.py` & `cardano-mass-payments-0.1.5/tests/mock_responses.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/mock_utils.py` & `cardano-mass-payments-0.1.5/tests/mock_utils.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_create_transaction_command.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_create_transaction_command.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_create_transaction_file.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_create_transaction_file.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_latest_slot_number.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_latest_slot_number.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_protocol_parameters.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_protocol_parameters.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_stake_address_balance.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_stake_address_balance.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_staking_address.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_staking_address.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_total_amount_plus_fee.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_total_amount_plus_fee.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_transaction_byte_size.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_transaction_byte_size.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_transaction_fee.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_utxo_hash.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_utxo_hash.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_get_wallet_utxo.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_get_wallet_utxo.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_cli_function_tests/test_sign_tx_file.py` & `cardano-mass-payments-0.1.5/tests/test_cli_function_tests/test_sign_tx_file.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_process/test_script_process.py` & `cardano-mass-payments-0.1.5/tests/test_process/test_script_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         source_address=None,
         source_signing_key_file=None,
         metadata_json_file=None,
         metadata_message_file=None,
         transaction_plan_file=None,
         magic_number=1,
         include_rewards=False,
+        reward_withdrawal_amount=-1,
         cardano_node_docker_image="cardano_node_docker_image_name",
     ):
         command_arguments = argparse.Namespace()
 
         command_arguments.cardano_network = cardano_network
         command_arguments.script_method = script_method
         command_arguments.output_type = output_type
@@ -83,14 +84,15 @@
         command_arguments.source_address = source_address
         command_arguments.source_signing_key_file = source_signing_key_file
         command_arguments.metadata_json_file = metadata_json_file
         command_arguments.metadata_message_file = metadata_message_file
         command_arguments.transaction_plan_file = transaction_plan_file
         command_arguments.magic_number = magic_number
         command_arguments.include_rewards = include_rewards
+        command_arguments.reward_withdrawal_amount = reward_withdrawal_amount
         command_arguments.cardano_node_docker_image = cardano_node_docker_image
 
         return command_arguments
 
     def test_1_input_30_payments_success(self):
         payment_file = create_test_payment_csv(30)
         source_file = self.create_test_source_csv()
@@ -813,14 +815,71 @@
         command_arguments = self.generate_command_arguments(
             sources_csv=source_file.name,
             payments_csv=payment_file.name,
             include_rewards=True,
         )
 
         with patch.dict(
+                "cardano_mass_payments.cache.CACHE_VALUES",
+                {"metadata_file": None},
+        ), patch(
+            "cardano_mass_payments.utils.cli_utils.subprocess_popen",
+            side_effect=generate_mock_popen_function(mock_responses),
+        ), patch(
+            "cardano_mass_payments.utils.cli_utils.sign_tx_file",
+            side_effect=mock_sign_tx_file_cli,
+        ):
+            try:
+                transaction_plan = generate_script_process(command_arguments)
+            except Exception as e:
+                transaction_plan = e
+
+        assert isinstance(transaction_plan, TransactionPlan)
+        assert os.path.exists(transaction_plan.filename)
+
+        os.remove(transaction_plan.filename)
+        os.remove(f"{transaction_plan.uuid}.sh")
+        source_file.close()
+        payment_file.close()
+
+    def test_success_with_rewards_and_amount(self):
+        payment_file = create_test_payment_csv(30)
+        source_file = self.create_test_source_csv()
+
+        mock_responses = deepcopy(MOCK_TEST_RESPONSES)
+        mock_responses["calculate-min-fee"] = "100 Lovelace"
+        del mock_responses["cat"]
+        mock_responses[("cat", f"/tmp-files/utxo-{MOCK_FULL_ADDRESS}.json")] = {
+            "85d0364b65cd68e259cd93a33253e322a0d02a67338f85dc1b67b09791e35905#1": {
+                "address": MOCK_FULL_ADDRESS,
+                "value": {"lovelace": 1000000000},
+            },
+        }
+        mock_responses["cat"] = USE_SUBPROCESS_FUNCTION_FLAG
+        mock_responses["rm"] = {}
+        mock_responses[("query", "tip")] = {"slot": 1}
+        mock_responses[("query", "protocol-parameters")] = MOCK_PROTOCOL_PARAMETERS
+        mock_responses[("cardano-address", "address")] = {
+            "stake_key_hash": "test_stake_key_hash",
+        }
+        mock_responses['"bech32'] = MOCK_STAKE_ADDRESS
+        mock_responses[("query", "stake-address-info")] = [
+            {
+                "rewardAccountBalance": 1000000,
+            },
+        ]
+
+        command_arguments = self.generate_command_arguments(
+            sources_csv=source_file.name,
+            payments_csv=payment_file.name,
+            include_rewards=True,
+            reward_withdrawal_amount=1000000,
+        )
+
+        with patch.dict(
             "cardano_mass_payments.cache.CACHE_VALUES",
             {"metadata_file": None},
         ), patch(
             "cardano_mass_payments.utils.cli_utils.subprocess_popen",
             side_effect=generate_mock_popen_function(mock_responses),
         ), patch(
             "cardano_mass_payments.utils.cli_utils.sign_tx_file",
```

### Comparing `cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_adjust_utxos.py` & `cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_adjust_utxos.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_dust_collect.py` & `cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_dust_collect.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_generate_bash_script.py` & `cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_generate_bash_script.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_group_output_utxo.py` & `cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_group_output_utxo.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_parse_payment_utxo_file.py` & `cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_parse_payment_utxo_file.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_parse_sources_csv_file.py` & `cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_parse_sources_csv_file.py`

 * *Files identical despite different names*

### Comparing `cardano-mass-payments-0.1.4/tests/test_script_function_tests/test_preparation_step.py` & `cardano-mass-payments-0.1.5/tests/test_script_function_tests/test_preparation_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -553,26 +553,76 @@
         mock_responses[("query", "stake-address-info")] = [
             {
                 "rewardAccountBalance": 1000000,
             },
         ]
 
         with patch.dict(
+                "cardano_mass_payments.cache.CACHE_VALUES",
+                {"source_signing_key_file": ["test.skey"]},
+        ), patch(
+            "cardano_mass_payments.utils.cli_utils.subprocess_popen",
+            side_effect=generate_mock_popen_function(mock_responses),
+        ):
+            payments_file = create_test_payment_csv(100)
+            try:
+                result = preparation_step(
+                    source_address=MOCK_FULL_ADDRESS,
+                    source_details={MOCK_FULL_ADDRESS: ["test.skey"]},
+                    payments_utxo_file=payments_file.name,
+                    include_rewards=True,
+                )
+            except Exception as e:
+                result = e
+            payments_file.close()
+
+        assert isinstance(result, dict)
+
+    def test_success_with_rewards_and_amount(self):
+        mock_responses = deepcopy(MOCK_TEST_RESPONSES)
+        mock_responses[("cat", f"/tmp-files/utxo-{MOCK_FULL_ADDRESS}.json")] = {
+            "85d0364b65cd68e259cd93a33253e322a0d02a67338f85dc1b67b09791e35905#1": {
+                "address": MOCK_FULL_ADDRESS,
+                "value": {"lovelace": 1000000000},
+            },
+        }
+        mock_responses["sign"] = {}
+        mock_responses["rm"] = {}
+        mock_responses["cat"] = {}
+        mock_responses["build-raw"] = {}
+        mock_responses["calculate-min-fee"] = "100 Lovelace"
+        mock_responses[("query", "tip")] = {"slot": 1}
+        mock_protocol_parameters = deepcopy(MOCK_PROTOCOL_PARAMETERS)
+        mock_protocol_parameters["maxTxSize"] = 10000
+        mock_responses[("query", "protocol-parameters")] = mock_protocol_parameters
+        mock_responses[("cardano-address", "address")] = {
+            "stake_key_hash": "test_stake_key_hash",
+        }
+        mock_responses['"bech32'] = MOCK_STAKE_ADDRESS
+        mock_responses[("query", "stake-address-info")] = [
+            {
+                "rewardAccountBalance": 1000000,
+            },
+        ]
+
+        with patch.dict(
             "cardano_mass_payments.cache.CACHE_VALUES",
             {"source_signing_key_file": ["test.skey"]},
         ), patch(
             "cardano_mass_payments.utils.cli_utils.subprocess_popen",
             side_effect=generate_mock_popen_function(mock_responses),
         ):
             payments_file = create_test_payment_csv(100)
             try:
                 result = preparation_step(
                     source_address=MOCK_FULL_ADDRESS,
                     source_details={MOCK_FULL_ADDRESS: ["test.skey"]},
                     payments_utxo_file=payments_file.name,
                     include_rewards=True,
+                    reward_amount=10,
                 )
             except Exception as e:
                 result = e
             payments_file.close()
 
         assert isinstance(result, dict)
+        assert result.get("stake_reward_details", {}).get("stake_amount") == 10
```

