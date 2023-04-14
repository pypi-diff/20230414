# Comparing `tmp/opender-2.0.2.tar.gz` & `tmp/opender-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opender-2.0.2.tar", last modified: Mon Apr  3 14:14:08 2023, max compression
+gzip compressed data, was "opender-2.0.3.tar", last modified: Fri Apr 14 18:15:31 2023, max compression
```

## Comparing `opender-2.0.2.tar` & `opender-2.0.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.685103 opender-2.0.2/
--rw-rw-rw-   0        0        0     2185 2023-04-03 14:12:57.000000 opender-2.0.2/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1707 2023-03-20 17:14:30.000000 opender-2.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      288 2022-08-10 15:01:38.000000 opender-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6177 2023-04-03 14:14:08.684103 opender-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3063 2023-04-03 14:12:57.000000 opender-2.0.2/README.rst
--rw-rw-rw-   0        0        0       49 2022-08-10 15:01:38.000000 opender-2.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 14:14:08.685103 opender-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3432 2023-04-03 14:12:57.000000 opender-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.514067 opender-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.551073 opender-2.0.2/src/opender/
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.592083 opender-2.0.2/src/opender/Parameters/
--rw-rw-rw-   0        0        0     2183 2023-03-20 17:14:30.000000 opender-2.0.2/src/opender/Parameters/AS-with std-values.csv
--rw-rw-rw-   0        0        0      306 2022-08-10 15:01:38.000000 opender-2.0.2/src/opender/Parameters/Model-parameters.csv
--rw-rw-rw-   0        0        0      322 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.614089 opender-2.0.2/src/opender/active_power_support_funcs/
--rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.0.2/src/opender/active_power_support_funcs/__init__.py
--rw-rw-rw-   0        0        0     3415 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/active_power_support_funcs/active_power_limit.py
--rw-rw-rw-   0        0        0     2570 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/active_power_support_funcs/es_perf.py
--rw-rw-rw-   0        0        0     3516 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/active_power_support_funcs/es_perf_bess.py
--rw-rw-rw-   0        0        0     9679 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/active_power_support_funcs/frequency_droop.py
--rw-rw-rw-   0        0        0     1881 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/active_power_support_funcs/frequency_droop_bess.py
--rw-rw-rw-   0        0        0     7271 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/active_power_support_funcs/p_funcs.py
--rw-rw-rw-   0        0        0     6866 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/active_power_support_funcs/p_funcs_bess.py
--rw-rw-rw-   0        0        0     1257 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/active_power_support_funcs/p_funcs_pv.py
--rw-rw-rw-   0        0        0     5099 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/active_power_support_funcs/volt_watt.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.626091 opender-2.0.2/src/opender/auxiliary_funcs/
--rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.0.2/src/opender/auxiliary_funcs/__init__.py
--rw-rw-rw-   0        0        0     2543 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/auxiliary_funcs/cond_delay.py
--rw-rw-rw-   0        0        0     1851 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/auxiliary_funcs/flipflop.py
--rw-rw-rw-   0        0        0     2234 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/auxiliary_funcs/low_pass_filter.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/auxiliary_funcs/ramping.py
--rw-rw-rw-   0        0        0     1526 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/auxiliary_funcs/sym_component.py
--rw-rw-rw-   0        0        0     2996 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/auxiliary_funcs/time_delay.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.630092 opender-2.0.2/src/opender/bess_specifc/
--rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.0.2/src/opender/bess_specifc/__init__.py
--rw-rw-rw-   0        0        0     6806 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/bess_specifc/soc.py
--rw-rw-rw-   0        0        0    16960 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/capability_and_priority.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.641094 opender-2.0.2/src/opender/common_file_format/
--rw-rw-rw-   0        0        0      113 2022-08-26 15:18:01.000000 opender-2.0.2/src/opender/common_file_format/__init__.py
--rw-rw-rw-   0        0        0    92676 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/common_file_format/common_file_format.py
--rw-rw-rw-   0        0        0     9574 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/common_file_format/common_file_format_BESS.py
--rw-rw-rw-   0        0        0    11644 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/der.py
--rw-rw-rw-   0        0        0     2930 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/der_bess.py
--rw-rw-rw-   0        0        0     1302 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/der_pv.py
--rw-rw-rw-   0        0        0    11392 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/op_cond_proc.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.653097 opender-2.0.2/src/opender/operation_status/
--rw-rw-rw-   0        0        0      910 2023-03-20 17:14:30.000000 opender-2.0.2/src/opender/operation_status/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.664100 opender-2.0.2/src/opender/operation_status/enter_service_crit/
--rw-rw-rw-   0        0        0       85 2023-03-20 17:14:30.000000 opender-2.0.2/src/opender/operation_status/enter_service_crit/__init__.py
--rw-rw-rw-   0        0        0     6206 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/operation_status/enter_service_crit/es_crit.py
--rw-rw-rw-   0        0        0     1729 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/operation_status/enter_service_crit/es_crit_pv.py
--rw-rw-rw-   0        0        0     5618 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/operation_status/operating_status.py
--rw-rw-rw-   0        0        0     1519 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/operation_status/operating_status_pv.py
--rw-rw-rw-   0        0        0    11520 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/operation_status/rt_crit.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.674102 opender-2.0.2/src/opender/operation_status/trip_crit/
--rw-rw-rw-   0        0        0       73 2023-03-20 17:14:30.000000 opender-2.0.2/src/opender/operation_status/trip_crit/__init__.py
--rw-rw-rw-   0        0        0     7896 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/operation_status/trip_crit/trip_crit.py
--rw-rw-rw-   0        0        0     1613 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/operation_status/trip_crit/trip_crit_pv.py
--rw-rw-rw-   0        0        0     9166 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/output_options.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.683104 opender-2.0.2/src/opender/reactive_power_support_funcs/
--rw-rw-rw-   0        0        0        0 2022-08-10 15:01:38.000000 opender-2.0.2/src/opender/reactive_power_support_funcs/__init__.py
--rw-rw-rw-   0        0        0     3920 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/reactive_power_support_funcs/constant_pf.py
--rw-rw-rw-   0        0        0     2455 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/reactive_power_support_funcs/constant_vars.py
--rw-rw-rw-   0        0        0     9342 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/reactive_power_support_funcs/q_funcs.py
--rw-rw-rw-   0        0        0     6858 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/reactive_power_support_funcs/volt_var.py
--rw-rw-rw-   0        0        0     7676 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/reactive_power_support_funcs/watt_var.py
--rw-rw-rw-   0        0        0    15680 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/rt_perf.py
--rw-rw-rw-   0        0        0    10266 2023-04-03 14:12:57.000000 opender-2.0.2/src/opender/setting_execution_delay.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:14:08.577081 opender-2.0.2/src/opender.egg-info/
--rw-rw-rw-   0        0        0     6177 2023-04-03 14:14:08.000000 opender-2.0.2/src/opender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2532 2023-04-03 14:14:08.000000 opender-2.0.2/src/opender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 14:14:08.000000 opender-2.0.2/src/opender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-03 14:14:08.000000 opender-2.0.2/src/opender.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       49 2023-04-03 14:14:08.000000 opender-2.0.2/src/opender.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-03 14:14:08.000000 opender-2.0.2/src/opender.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.785634 opender-2.0.3/
+-rw-rw-rw-   0        0        0     2383 2023-04-14 18:15:23.000000 opender-2.0.3/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1707 2023-03-20 17:14:30.000000 opender-2.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      288 2022-08-10 15:01:38.000000 opender-2.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6375 2023-04-14 18:15:31.785634 opender-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3063 2023-04-03 14:12:57.000000 opender-2.0.3/README.rst
+-rw-rw-rw-   0        0        0       49 2022-08-10 15:01:38.000000 opender-2.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 18:15:31.786634 opender-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3432 2023-04-14 18:15:23.000000 opender-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.659614 opender-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.685610 opender-2.0.3/src/opender/
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.709614 opender-2.0.3/src/opender/Parameters/
+-rw-rw-rw-   0        0        0     2183 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/Parameters/AS-with std-values.csv
+-rw-rw-rw-   0        0        0      306 2022-08-10 15:01:38.000000 opender-2.0.3/src/opender/Parameters/Model-parameters.csv
+-rw-rw-rw-   0        0        0      322 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.736621 opender-2.0.3/src/opender/active_power_support_funcs/
+-rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/active_power_support_funcs/__init__.py
+-rw-rw-rw-   0        0        0     3415 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/active_power_limit.py
+-rw-rw-rw-   0        0        0     2570 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/es_perf.py
+-rw-rw-rw-   0        0        0     3516 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/es_perf_bess.py
+-rw-rw-rw-   0        0        0     9671 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/active_power_support_funcs/frequency_droop.py
+-rw-rw-rw-   0        0        0     1881 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/frequency_droop_bess.py
+-rw-rw-rw-   0        0        0     7267 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/active_power_support_funcs/p_funcs.py
+-rw-rw-rw-   0        0        0     6864 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/active_power_support_funcs/p_funcs_bess.py
+-rw-rw-rw-   0        0        0     1257 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/p_funcs_pv.py
+-rw-rw-rw-   0        0        0     5099 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/volt_watt.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.747624 opender-2.0.3/src/opender/auxiliary_funcs/
+-rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/auxiliary_funcs/__init__.py
+-rw-rw-rw-   0        0        0     2543 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/cond_delay.py
+-rw-rw-rw-   0        0        0     1851 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/flipflop.py
+-rw-rw-rw-   0        0        0     2234 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/low_pass_filter.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/ramping.py
+-rw-rw-rw-   0        0        0     1526 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/sym_component.py
+-rw-rw-rw-   0        0        0     2996 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/time_delay.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.749624 opender-2.0.3/src/opender/bess_specifc/
+-rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/bess_specifc/__init__.py
+-rw-rw-rw-   0        0        0     6806 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/bess_specifc/soc.py
+-rw-rw-rw-   0        0        0    16960 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/capability_and_priority.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.760627 opender-2.0.3/src/opender/common_file_format/
+-rw-rw-rw-   0        0        0      113 2022-08-26 15:18:01.000000 opender-2.0.3/src/opender/common_file_format/__init__.py
+-rw-rw-rw-   0        0        0    92676 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/common_file_format/common_file_format.py
+-rw-rw-rw-   0        0        0    10018 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/common_file_format/common_file_format_BESS.py
+-rw-rw-rw-   0        0        0    11644 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/der.py
+-rw-rw-rw-   0        0        0     2930 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/der_bess.py
+-rw-rw-rw-   0        0        0     1302 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/der_pv.py
+-rw-rw-rw-   0        0        0    11392 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/op_cond_proc.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.766627 opender-2.0.3/src/opender/operation_status/
+-rw-rw-rw-   0        0        0      910 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/operation_status/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.770628 opender-2.0.3/src/opender/operation_status/enter_service_crit/
+-rw-rw-rw-   0        0        0       85 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/operation_status/enter_service_crit/__init__.py
+-rw-rw-rw-   0        0        0     6206 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/enter_service_crit/es_crit.py
+-rw-rw-rw-   0        0        0     1729 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/enter_service_crit/es_crit_pv.py
+-rw-rw-rw-   0        0        0     5618 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/operating_status.py
+-rw-rw-rw-   0        0        0     1519 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/operating_status_pv.py
+-rw-rw-rw-   0        0        0    11520 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/rt_crit.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.775629 opender-2.0.3/src/opender/operation_status/trip_crit/
+-rw-rw-rw-   0        0        0       73 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/operation_status/trip_crit/__init__.py
+-rw-rw-rw-   0        0        0     7896 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/trip_crit/trip_crit.py
+-rw-rw-rw-   0        0        0     1613 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/trip_crit/trip_crit_pv.py
+-rw-rw-rw-   0        0        0     9166 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/output_options.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.783632 opender-2.0.3/src/opender/reactive_power_support_funcs/
+-rw-rw-rw-   0        0        0        0 2022-08-10 15:01:38.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/__init__.py
+-rw-rw-rw-   0        0        0     3920 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/constant_pf.py
+-rw-rw-rw-   0        0        0     2455 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/constant_vars.py
+-rw-rw-rw-   0        0        0     9342 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/q_funcs.py
+-rw-rw-rw-   0        0        0     6858 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/volt_var.py
+-rw-rw-rw-   0        0        0     7676 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/watt_var.py
+-rw-rw-rw-   0        0        0    15680 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/rt_perf.py
+-rw-rw-rw-   0        0        0    10266 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/setting_execution_delay.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.706614 opender-2.0.3/src/opender.egg-info/
+-rw-rw-rw-   0        0        0     6375 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2532 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       49 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/top_level.txt
```

### Comparing `opender-2.0.2/CHANGELOG.rst` & `opender-2.0.3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 
 Changelog
 =========
+2.0.3 (2023-04-14)
+------------------
+* Fixed the option to update BESS DER parameter when creating the object.
+* Fixed a bug when initializing a BESS DER during abnormal frequency condition.
+
 2.0.2 (2023-04-03)
 ------------------
 * Fixed a bug abnormal operation category (NP_ABNORMAL_OP_CAT) only accepts uppercase values
 * Updated ride-through performance to better represent actual inverter's behavior
 * Added an option to update DER parameter when creating the object.
 
 2.0.1 (2023-03-21)
```

### Comparing `opender-2.0.2/LICENSE.txt` & `opender-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/PKG-INFO` & `opender-2.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opender
-Version: 2.0.2
+Version: 2.0.3
 Summary: Open-source Distributed Energy Resources (DER) Model that represents IEEE Standard 1547-2018 requirements for steady-state and dynamic analyses
 Home-page: https://github.com/epri-dev/opender
 Author: Yiwei Ma, Wei Ren, Paulo Radatz, Jithendar Anandan
 Author-email: yma@epri.com, wren@epri.com, pradatz@epri.com
 License: BSD
 Project-URL: Homepage, https://www.epri.com/OpenDER
 Project-URL: Model Specification, https://www.epri.com/research/products/000000003002021694
@@ -95,14 +95,19 @@
 Execution command: pytest path-to-package\\tests
 
 
 
 
 Changelog
 =========
+2.0.3 (2023-04-14)
+------------------
+* Fixed the option to update BESS DER parameter when creating the object.
+* Fixed a bug when initializing a BESS DER during abnormal frequency condition.
+
 2.0.2 (2023-04-03)
 ------------------
 * Fixed a bug abnormal operation category (NP_ABNORMAL_OP_CAT) only accepts uppercase values
 * Updated ride-through performance to better represent actual inverter's behavior
 * Added an option to update DER parameter when creating the object.
 
 2.0.1 (2023-03-21)
```

### Comparing `opender-2.0.2/README.rst` & `opender-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/setup.py` & `opender-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 setup(
     name='opender',
-    version='2.0.2',
+    version='2.0.3',
     license='BSD',
     description='Open-source Distributed Energy Resources (DER) Model that represents IEEE Standard 1547-2018 '
                 'requirements for steady-state and dynamic analyses',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
```

### Comparing `opender-2.0.2/src/opender/Parameters/AS-with std-values.csv` & `opender-2.0.3/src/opender/Parameters/AS-with std-values.csv`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/__init__.py` & `opender-2.0.3/src/opender/active_power_support_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/active_power_limit.py` & `opender-2.0.3/src/opender/active_power_support_funcs/active_power_limit.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/es_perf.py` & `opender-2.0.3/src/opender/active_power_support_funcs/es_perf.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/es_perf_bess.py` & `opender-2.0.3/src/opender/active_power_support_funcs/es_perf_bess.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/frequency_droop.py` & `opender-2.0.3/src/opender/active_power_support_funcs/frequency_droop.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             self.p_out_w_prev = min(self.get_p_pu() * self.der_file.NP_P_MAX,
                                     ap_limit_rt * self.der_file.NP_P_MAX, p_pv_limit_pu * self.der_file.NP_P_MAX)
         else:
             self.p_out_w_prev = p_out_w
 
         # Initialize internal state variables of pre-disturbance active power output
         if self.p_pf_pre_pu_prev is None:
-            self.p_pf_pre_pu_prev = min(self.der_input.p_avl_pu, ap_limit_rt, p_pv_limit_pu)
+            self.p_pf_pre_pu_prev = min(self.get_p_pu(), ap_limit_rt, p_pv_limit_pu)
 
         # Eq. 3.7.1-11, calculate pre-disturbance active power output
         if self.pf_uf == 1 and self.pf_uf_prev == 1:
             self.p_pf_pre_pu = self.p_pf_pre_pu_prev
         elif self.pf_of == 1 and self.pf_of_prev == 1:
             self.p_pf_pre_pu = self.p_pf_pre_pu_prev
         else:
```

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/frequency_droop_bess.py` & `opender-2.0.3/src/opender/active_power_support_funcs/frequency_droop_bess.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/p_funcs.py` & `opender-2.0.3/src/opender/active_power_support_funcs/p_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,41 +39,41 @@
         self.p_desired_pu = None        # Desired active power from all active power support functions
 
         self.aplimit = active_power_limit.ActivePowerLimit(self.der_file, self.exec_delay)
         self.voltwatt = volt_watt.VoltWatt(self.der_file, self.exec_delay, self.der_input)
         self.freqdroop = frequency_droop.FreqDroop(self.der_obj)
         self.enterserviceperf = es_perf.EnterServicePerformance(der_obj)
 
-    def calculate_p_funcs(self, p_out_pu):
+    def calculate_p_funcs(self, p_out_w):
         """
         Call active power support functions and based on the results, generate desired active power output
 
         Output:
         :param p_desired_pu:	Desired output active power from active power support functions in per unit
         """
 
         # Active power limit function
         self.ap_limit_rt = self.aplimit.calculate_ap_limit_rt()
 
         # Volt-watt function
         self.p_pv_limit_pu = self.voltwatt.calculate_p_pv_limit_pu()
 
         # Frequency-droop function
-        self.p_pf_pu, self.pf_uf_active, self.pf_of_active = self.freqdroop.calculate_p_pf_pu(p_out_pu,
+        self.p_pf_pu, self.pf_uf_active, self.pf_of_active = self.freqdroop.calculate_p_pf_pu(p_out_w,
                                                                                               self.ap_limit_rt,
                                                                                               self.p_pv_limit_pu)
         # Enter service ramp performance
         self.p_es_pu = self.enterserviceperf.es_performance()
 
         # Calculate final desired active power based on other functions
-        self.p_desired_pu = self.calculate_p_desired_pu(p_out_pu)
+        self.p_desired_pu = self.calculate_p_desired_pu(p_out_w)
 
         return self.p_desired_pu
 
-    def calculate_p_desired_pu(self, p_out_pu):
+    def calculate_p_desired_pu(self, p_out_w):
         """
         Based on the calculated values from volt-watt, frequency-droop, active power limit, and enter service ramp,
         their enabling signal, and DER operating status, generate the DER desired active power output
         EPRI Report Reference: Section 3.7.1.5 in Report #3002026631: IEEE 1547-2018 OpenDER Model
 
         Variable used in this function:
         :param ap_limit_enable_exec:	Active power limit enable (AP_LIMIT_ENABLE) signal after execution delay
```

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/p_funcs_bess.py` & `opender-2.0.3/src/opender/active_power_support_funcs/p_funcs_bess.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.soc_calc = StateOfCharge(self.der_file)
         self.enterserviceperf = EnterServicePerformanceBESS(der_obj)
 
         self.p_act_supp_bess_pu = None      # Desired output active power from active power support functions in per
                                             # unit without considering the BESS related constraints
         self.p_es_dem_pu = None             # Active power demand considering enter service ramp
 
-    def calculate_p_desired_pu(self, p_out_pu):
+    def calculate_p_desired_pu(self, p_out_w):
         """
         Based on the calculated values from volt-watt, frequency-droop, active power limit, and enter service ramp,
         their enabling signal, and DER operating status, generate the DER desired active power output. Specifically
         for BESS DER, the State of Charge (SoC) and limitation of output active power due to SoC is considered.
         EPRI Report Reference: Section 3.7.3.3 in Report #3002026631: IEEE 1547-2018 OpenDER Model
 
         Variable used in this function:
@@ -50,15 +50,15 @@
         :param NP_P_MAX:	    Active power rating at unity power factor
         :param p_dem_pu:        BESS DER active power demand in pu
         """
 
         if DER.t_s <= 7200 and self.der_file.NP_BESS_CAPACITY is not None:
             # For time series simulation
             # Calculate SoC
-            self.soc_calc.calculate_soc(p_out_pu)
+            self.soc_calc.calculate_soc(p_out_w)
 
             # Calculate P limits
             self.soc_calc.calculate_p_max_by_soc()
         else:
             # For snapshot analysis
             self.soc_calc.snapshot_limits()
```

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/p_funcs_pv.py` & `opender-2.0.3/src/opender/active_power_support_funcs/p_funcs_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/active_power_support_funcs/volt_watt.py` & `opender-2.0.3/src/opender/active_power_support_funcs/volt_watt.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/auxiliary_funcs/__init__.py` & `opender-2.0.3/src/opender/auxiliary_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/auxiliary_funcs/cond_delay.py` & `opender-2.0.3/src/opender/auxiliary_funcs/cond_delay.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/auxiliary_funcs/flipflop.py` & `opender-2.0.3/src/opender/auxiliary_funcs/flipflop.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/auxiliary_funcs/low_pass_filter.py` & `opender-2.0.3/src/opender/auxiliary_funcs/low_pass_filter.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/auxiliary_funcs/ramping.py` & `opender-2.0.3/src/opender/auxiliary_funcs/ramping.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/auxiliary_funcs/sym_component.py` & `opender-2.0.3/src/opender/auxiliary_funcs/sym_component.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/auxiliary_funcs/time_delay.py` & `opender-2.0.3/src/opender/auxiliary_funcs/time_delay.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/bess_specifc/__init__.py` & `opender-2.0.3/src/opender/bess_specifc/__init__.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/bess_specifc/soc.py` & `opender-2.0.3/src/opender/bess_specifc/soc.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/capability_and_priority.py` & `opender-2.0.3/src/opender/capability_and_priority.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/common_file_format/common_file_format.py` & `opender-2.0.3/src/opender/common_file_format/common_file_format.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/common_file_format/common_file_format_BESS.py` & `opender-2.0.3/src/opender/common_file_format/common_file_format_BESS.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
                        'SOC_P_DISCHARGE_MAX', 'P_CHARGE_MAX_PU', 'SOC_P_CHARGE_MAX', 'SOC_INIT'
                        ]
 
     __slots__ = tuple(['_' + param for param in parameters_list]) + tuple(['param_inputs'])
 
     def __init__(self,
                  as_file_path=pathlib.Path(os.path.dirname(__file__)).joinpath("../Parameters", "AS-with std-values.csv"),
-                 model_file_path=pathlib.Path(os.path.dirname(__file__)).joinpath("../Parameters",
-                                                                                  "Model-parameters.csv")):
+                 model_file_path=pathlib.Path(os.path.dirname(__file__)).joinpath("../Parameters","Model-parameters.csv"),
+                 **kwargs):
         """
         Creating a DER common file format object
         :param as_file_path: File directory address for Common file format Applied Setting file.
         :param model_file_path: File directory address for Model custom parameter file.
         """
         super(DERCommonFileFormatBESS, self).__init__(as_file_path, model_file_path)
 
@@ -78,15 +78,23 @@
         if self.isNotNaN(self.param_inputs.P_CHARGE_MAX_PU):
             self.P_CHARGE_MAX_PU = self.param_inputs.P_CHARGE_MAX_PU
         if self.isNotNaN(self.param_inputs.SOC_P_CHARGE_MAX):
             self.SOC_P_CHARGE_MAX = self.param_inputs.SOC_P_CHARGE_MAX
         if self.isNotNaN(self.param_inputs.SOC_INIT):
             self.SOC_INIT = self.param_inputs.SOC_INIT
         self.initialize_NP_BESS_P_MAX_BY_SOC()
-    #
+
+        for key, value in kwargs.items():
+            if key in self._get_parameter_list():
+                setattr(self, key, value)
+            elif key=='convert' and isinstance(value, DERCommonFileFormat):
+                super(DERCommonFileFormatBESS, self).__init__(**{s: getattr(value, s) for s in value.parameters_list if hasattr(value, s) and not getattr(value, s) is None})
+            else:
+                logging.warning(f"'{key}' is not in the parameter list, please double check")
+
     def _get_parameter_list(self):
         return self.__class__.parameters_list
 
     def initialize_NP_BESS_P_MAX_BY_SOC(self):
         """
         Initialize Maximum active power limitation by SOC curve using 4 array inputs of P_DISCHARGE_MAX_PU,
         SOC_P_DISCHARGE_MAX, P_CHARGE_MAX_PU, SOC_P_CHARGE_MAX
```

### Comparing `opender-2.0.2/src/opender/der.py` & `opender-2.0.3/src/opender/der.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/der_bess.py` & `opender-2.0.3/src/opender/der_bess.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/der_pv.py` & `opender-2.0.3/src/opender/der_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/op_cond_proc.py` & `opender-2.0.3/src/opender/op_cond_proc.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/operation_status/__init__.py` & `opender-2.0.3/src/opender/operation_status/__init__.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/operation_status/enter_service_crit/es_crit.py` & `opender-2.0.3/src/opender/operation_status/enter_service_crit/es_crit.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/operation_status/enter_service_crit/es_crit_pv.py` & `opender-2.0.3/src/opender/operation_status/enter_service_crit/es_crit_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/operation_status/operating_status.py` & `opender-2.0.3/src/opender/operation_status/operating_status.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/operation_status/operating_status_pv.py` & `opender-2.0.3/src/opender/operation_status/operating_status_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/operation_status/rt_crit.py` & `opender-2.0.3/src/opender/operation_status/rt_crit.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/operation_status/trip_crit/trip_crit.py` & `opender-2.0.3/src/opender/operation_status/trip_crit/trip_crit.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/operation_status/trip_crit/trip_crit_pv.py` & `opender-2.0.3/src/opender/operation_status/trip_crit/trip_crit_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/output_options.py` & `opender-2.0.3/src/opender/output_options.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/reactive_power_support_funcs/constant_pf.py` & `opender-2.0.3/src/opender/reactive_power_support_funcs/constant_pf.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/reactive_power_support_funcs/constant_vars.py` & `opender-2.0.3/src/opender/reactive_power_support_funcs/constant_vars.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/reactive_power_support_funcs/q_funcs.py` & `opender-2.0.3/src/opender/reactive_power_support_funcs/q_funcs.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/reactive_power_support_funcs/volt_var.py` & `opender-2.0.3/src/opender/reactive_power_support_funcs/volt_var.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/reactive_power_support_funcs/watt_var.py` & `opender-2.0.3/src/opender/reactive_power_support_funcs/watt_var.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/rt_perf.py` & `opender-2.0.3/src/opender/rt_perf.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender/setting_execution_delay.py` & `opender-2.0.3/src/opender/setting_execution_delay.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.2/src/opender.egg-info/PKG-INFO` & `opender-2.0.3/src/opender.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opender
-Version: 2.0.2
+Version: 2.0.3
 Summary: Open-source Distributed Energy Resources (DER) Model that represents IEEE Standard 1547-2018 requirements for steady-state and dynamic analyses
 Home-page: https://github.com/epri-dev/opender
 Author: Yiwei Ma, Wei Ren, Paulo Radatz, Jithendar Anandan
 Author-email: yma@epri.com, wren@epri.com, pradatz@epri.com
 License: BSD
 Project-URL: Homepage, https://www.epri.com/OpenDER
 Project-URL: Model Specification, https://www.epri.com/research/products/000000003002021694
@@ -95,14 +95,19 @@
 Execution command: pytest path-to-package\\tests
 
 
 
 
 Changelog
 =========
+2.0.3 (2023-04-14)
+------------------
+* Fixed the option to update BESS DER parameter when creating the object.
+* Fixed a bug when initializing a BESS DER during abnormal frequency condition.
+
 2.0.2 (2023-04-03)
 ------------------
 * Fixed a bug abnormal operation category (NP_ABNORMAL_OP_CAT) only accepts uppercase values
 * Updated ride-through performance to better represent actual inverter's behavior
 * Added an option to update DER parameter when creating the object.
 
 2.0.1 (2023-03-21)
```

### Comparing `opender-2.0.2/src/opender.egg-info/SOURCES.txt` & `opender-2.0.3/src/opender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

