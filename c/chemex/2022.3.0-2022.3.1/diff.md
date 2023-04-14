# Comparing `tmp/chemex-2022.3.0.tar.gz` & `tmp/chemex-2022.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemex-2022.3.0.tar", max compression
+gzip compressed data, was "chemex-2022.3.1.tar", max compression
```

## Comparing `chemex-2022.3.0.tar` & `chemex-2022.3.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0    34916 2023-02-22 22:19:55.533429 chemex-2022.3.0/LICENSE.md
--rw-r--r--   0        0        0     1046 2023-02-22 22:19:55.533429 chemex-2022.3.0/README.md
--rw-r--r--   0        0        0      326 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/__init__.py
--rw-r--r--   0        0        0      185 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/__main__.py
--rw-r--r--   0        0        0     2583 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/chemex.py
--rw-r--r--   0        0        0     5876 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/cli.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/configuration/__init__.py
--rw-r--r--   0        0        0      447 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/configuration/base.py
--rw-r--r--   0        0        0     4619 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/configuration/conditions.py
--rw-r--r--   0        0        0     1491 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/configuration/data.py
--rw-r--r--   0        0        0     1418 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/configuration/experiment.py
--rw-r--r--   0        0        0     4588 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/configuration/methods.py
--rw-r--r--   0        0        0     1971 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/configuration/parameters.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/containers/__init__.py
--rw-r--r--   0        0        0     3158 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/containers/data.py
--rw-r--r--   0        0        0     1478 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/containers/dataset.py
--rw-r--r--   0        0        0     5406 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/containers/experiment.py
--rw-r--r--   0        0        0     4238 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/containers/experiments.py
--rw-r--r--   0        0        0     3840 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/containers/profile.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/experiments/__init__.py
--rw-r--r--   0        0        0     4379 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/experiments/builder.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.533429 chemex-2022.3.0/chemex/experiments/catalog/__init__.py
--rw-r--r--   0        0        0     3678 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cest_13c.py
--rw-r--r--   0        0        0     3588 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cest_15n.py
--rw-r--r--   0        0        0     4060 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cest_15n_cw.py
--rw-r--r--   0        0        0     4353 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cest_15n_tr.py
--rw-r--r--   0        0        0     3682 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cest_1hn_ap.py
--rw-r--r--   0        0        0     4771 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4084 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
--rw-r--r--   0        0        0     5188 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/coscest_13c.py
--rw-r--r--   0        0        0     5472 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/coscest_1hn_ip_ap.py
--rw-r--r--   0        0        0     4782 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_13c_ip.py
--rw-r--r--   0        0        0     5174 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_13co_ap.py
--rw-r--r--   0        0        0     4864 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_15n_ip.py
--rw-r--r--   0        0        0     5702 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_15n_ip_0013.py
--rw-r--r--   0        0        0     5456 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_15n_tr.py
--rw-r--r--   0        0        0     7561 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_15n_tr_0013.py
--rw-r--r--   0        0        0     4965 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_1hn_ap.py
--rw-r--r--   0        0        0     7376 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
--rw-r--r--   0        0        0     5016 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
--rw-r--r--   0        0        0     5869 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
--rw-r--r--   0        0        0     6696 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
--rw-r--r--   0        0        0     5871 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
--rw-r--r--   0        0        0     7400 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
--rw-r--r--   0        0        0     4292 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_mq.py
--rw-r--r--   0        0        0     4916 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
--rw-r--r--   0        0        0     5290 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/cpmg_hn_dq_zq.py
--rw-r--r--   0        0        0     4412 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/dcest_13c.py
--rw-r--r--   0        0        0     4643 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/dcest_15n.py
--rw-r--r--   0        0        0     3330 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/relaxation_hznz.py
--rw-r--r--   0        0        0     2991 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/relaxation_nz.py
--rw-r--r--   0        0        0     2921 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/shift_15n_sq.py
--rw-r--r--   0        0        0     3283 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/catalog/shift_15n_sqmq.py
--rw-r--r--   0        0        0     3235 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/factories.py
--rw-r--r--   0        0        0      970 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/experiments/loader.py
--rw-r--r--   0        0        0     2671 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/filterers.py
--rw-r--r--   0        0        0     7125 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/messages.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/__init__.py
--rw-r--r--   0        0        0     2753 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/constraints.py
--rw-r--r--   0        0        0     1071 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/factory.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/__init__.py
--rw-r--r--   0        0        0      575 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_1st.py
--rw-r--r--   0        0        0     1241 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_2st.py
--rw-r--r--   0        0        0     2954 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_2st_a_a2.py
--rw-r--r--   0        0        0     2958 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_2st_a_a3.py
--rw-r--r--   0        0        0     2966 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_2st_a_a4.py
--rw-r--r--   0        0        0     2722 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_2st_binding.py
--rw-r--r--   0        0        0     2878 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_2st_eyring.py
--rw-r--r--   0        0        0     1985 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_2st_hd.py
--rw-r--r--   0        0        0     1278 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_2st_rs.py
--rw-r--r--   0        0        0     4590 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_3st_a_a2_a3.py
--rw-r--r--   0        0        0     4298 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_3st_a_a2_a4.py
--rw-r--r--   0        0        0     5043 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_3st_double_binding.py
--rw-r--r--   0        0        0     4463 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_3st_eyring.py
--rw-r--r--   0        0        0     4079 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_3st_induced_fit.py
--rw-r--r--   0        0        0     3994 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_4st_hd.py
--rw-r--r--   0        0        0     4768 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/kinetic/settings_nst.py
--rw-r--r--   0        0        0      945 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/loader.py
--rw-r--r--   0        0        0     1396 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/models/model.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/nmr/__init__.py
--rw-r--r--   0        0        0    10952 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/nmr/basis.py
--rw-r--r--   0        0        0     6309 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/nmr/constants.py
--rw-r--r--   0        0        0     9538 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/nmr/liouvillian.py
--rw-r--r--   0        0        0     8795 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/nmr/rates.py
--rw-r--r--   0        0        0    13135 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/nmr/spectrometer.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/optimize/__init__.py
--rw-r--r--   0        0        0     5309 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/optimize/fitting.py
--rw-r--r--   0        0        0     8679 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/optimize/gridding.py
--rw-r--r--   0        0        0     2946 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/optimize/grouping.py
--rw-r--r--   0        0        0     5459 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/optimize/helper.py
--rw-r--r--   0        0        0     2763 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/optimize/minimizer.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/parameters/__init__.py
--rw-r--r--   0        0        0    12817 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/parameters/database.py
--rw-r--r--   0        0        0     3236 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/parameters/factory.py
--rw-r--r--   0        0        0     4659 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/parameters/name.py
--rw-r--r--   0        0        0     3937 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/parameters/setting.py
--rw-r--r--   0        0        0    12664 2023-02-22 22:19:55.537429 chemex-2022.3.0/chemex/parameters/spin_system.py
--rw-r--r--   0        0        0     9168 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/parameters/spins.py
--rw-r--r--   0        0        0      901 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/parameters/userfunctions.py
--rw-r--r--   0        0        0      316 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/plotters/__init__.py
--rw-r--r--   0        0        0     7907 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/plotters/cest.py
--rw-r--r--   0        0        0     6634 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/plotters/cpmg.py
--rw-r--r--   0        0        0     2376 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/plotters/plot.py
--rw-r--r--   0        0        0      329 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/plotters/plotter.py
--rw-r--r--   0        0        0     3706 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/plotters/relaxation.py
--rw-r--r--   0        0        0     1674 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/plotters/shift.py
--rw-r--r--   0        0        0        0 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/printers/__init__.py
--rw-r--r--   0        0        0     1785 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/printers/data.py
--rw-r--r--   0        0        0     4510 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/printers/parameters.py
--rw-r--r--   0        0        0     2679 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/printers/plot.py
--rw-r--r--   0        0        0     2929 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/toml.py
--rw-r--r--   0        0        0       98 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/tools/__init__.py
--rw-r--r--   0        0        0     9332 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/tools/pick_cest.py
--rw-r--r--   0        0        0     1819 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/tools/plot_param.py
--rw-r--r--   0        0        0     2667 2023-02-22 22:19:55.541430 chemex-2022.3.0/chemex/uncertainty.py
--rw-r--r--   0        0        0     1045 2023-02-22 22:19:55.761439 chemex-2022.3.0/pyproject.toml
--rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 chemex-2022.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-04-14 11:37:01.941999 chemex-2022.3.1/LICENSE.md
+-rw-r--r--   0        0        0     1046 2023-04-14 11:37:01.941999 chemex-2022.3.1/README.md
+-rw-r--r--   0        0        0      326 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/__main__.py
+-rw-r--r--   0        0        0     2583 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/chemex.py
+-rw-r--r--   0        0        0     5876 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/cli.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/base.py
+-rw-r--r--   0        0        0     4619 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/conditions.py
+-rw-r--r--   0        0        0     1491 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/data.py
+-rw-r--r--   0        0        0     1418 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/experiment.py
+-rw-r--r--   0        0        0     4588 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/methods.py
+-rw-r--r--   0        0        0     1971 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/configuration/parameters.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/__init__.py
+-rw-r--r--   0        0        0     3158 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/data.py
+-rw-r--r--   0        0        0     1497 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/dataset.py
+-rw-r--r--   0        0        0     5406 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/experiment.py
+-rw-r--r--   0        0        0     4238 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/experiments.py
+-rw-r--r--   0        0        0     3840 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/containers/profile.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/experiments/__init__.py
+-rw-r--r--   0        0        0     4379 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/experiments/builder.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.941999 chemex-2022.3.1/chemex/experiments/catalog/__init__.py
+-rw-r--r--   0        0        0     3678 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_13c.py
+-rw-r--r--   0        0        0     3588 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_15n.py
+-rw-r--r--   0        0        0     4060 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_15n_cw.py
+-rw-r--r--   0        0        0     4353 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_15n_tr.py
+-rw-r--r--   0        0        0     3682 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_1hn_ap.py
+-rw-r--r--   0        0        0     4771 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4084 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py
+-rw-r--r--   0        0        0     5188 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/coscest_13c.py
+-rw-r--r--   0        0        0     5472 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/coscest_1hn_ip_ap.py
+-rw-r--r--   0        0        0     4782 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_13c_ip.py
+-rw-r--r--   0        0        0     5174 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_13co_ap.py
+-rw-r--r--   0        0        0     4864 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_ip.py
+-rw-r--r--   0        0        0     5702 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_ip_0013.py
+-rw-r--r--   0        0        0     5456 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_tr.py
+-rw-r--r--   0        0        0     7561 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_tr_0013.py
+-rw-r--r--   0        0        0     4965 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_1hn_ap.py
+-rw-r--r--   0        0        0     7340 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_1hn_ap_0013.py
+-rw-r--r--   0        0        0     5016 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py
+-rw-r--r--   0        0        0     5869 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_dq.py
+-rw-r--r--   0        0        0     6696 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_sq.py
+-rw-r--r--   0        0        0     5871 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_tq.py
+-rw-r--r--   0        0        0     7400 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py
+-rw-r--r--   0        0        0     4292 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_mq.py
+-rw-r--r--   0        0        0     4916 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_chd2_1h_ap.py
+-rw-r--r--   0        0        0     5290 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/cpmg_hn_dq_zq.py
+-rw-r--r--   0        0        0     4412 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/dcest_13c.py
+-rw-r--r--   0        0        0     4643 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/dcest_15n.py
+-rw-r--r--   0        0        0     3330 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/relaxation_hznz.py
+-rw-r--r--   0        0        0     2991 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/relaxation_nz.py
+-rw-r--r--   0        0        0     2921 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/shift_15n_sq.py
+-rw-r--r--   0        0        0     3283 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/catalog/shift_15n_sqmq.py
+-rw-r--r--   0        0        0     3235 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/factories.py
+-rw-r--r--   0        0        0      970 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/experiments/loader.py
+-rw-r--r--   0        0        0     2671 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/filterers.py
+-rw-r--r--   0        0        0     7125 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/messages.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/__init__.py
+-rw-r--r--   0        0        0     2753 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/constraints.py
+-rw-r--r--   0        0        0     1071 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/factory.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_1st.py
+-rw-r--r--   0        0        0     1241 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st.py
+-rw-r--r--   0        0        0     2954 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a2.py
+-rw-r--r--   0        0        0     2958 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a3.py
+-rw-r--r--   0        0        0     2966 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a4.py
+-rw-r--r--   0        0        0     2722 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_binding.py
+-rw-r--r--   0        0        0     2878 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_eyring.py
+-rw-r--r--   0        0        0     1985 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_hd.py
+-rw-r--r--   0        0        0     1278 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_2st_rs.py
+-rw-r--r--   0        0        0     4590 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_a_a2_a3.py
+-rw-r--r--   0        0        0     4298 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_a_a2_a4.py
+-rw-r--r--   0        0        0     5043 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_double_binding.py
+-rw-r--r--   0        0        0     4463 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_eyring.py
+-rw-r--r--   0        0        0     4079 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_3st_induced_fit.py
+-rw-r--r--   0        0        0     3994 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_4st_hd.py
+-rw-r--r--   0        0        0     4768 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/kinetic/settings_nst.py
+-rw-r--r--   0        0        0      945 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/loader.py
+-rw-r--r--   0        0        0     1396 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/models/model.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/__init__.py
+-rw-r--r--   0        0        0    10952 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/basis.py
+-rw-r--r--   0        0        0     6309 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/constants.py
+-rw-r--r--   0        0        0     9538 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/liouvillian.py
+-rw-r--r--   0        0        0     8795 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/rates.py
+-rw-r--r--   0        0        0    13135 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/nmr/spectrometer.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/__init__.py
+-rw-r--r--   0        0        0     5309 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/fitting.py
+-rw-r--r--   0        0        0     8679 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/gridding.py
+-rw-r--r--   0        0        0     2946 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/grouping.py
+-rw-r--r--   0        0        0     5459 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/helper.py
+-rw-r--r--   0        0        0     2763 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/optimize/minimizer.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/__init__.py
+-rw-r--r--   0        0        0    12772 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/database.py
+-rw-r--r--   0        0        0     3236 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/factory.py
+-rw-r--r--   0        0        0     4659 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/name.py
+-rw-r--r--   0        0        0     3937 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/setting.py
+-rw-r--r--   0        0        0    12664 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/spin_system.py
+-rw-r--r--   0        0        0     9618 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/spins.py
+-rw-r--r--   0        0        0      901 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/parameters/userfunctions.py
+-rw-r--r--   0        0        0      316 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/__init__.py
+-rw-r--r--   0        0        0     7907 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/cest.py
+-rw-r--r--   0        0        0     6634 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/cpmg.py
+-rw-r--r--   0        0        0     2376 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/plot.py
+-rw-r--r--   0        0        0      329 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/plotter.py
+-rw-r--r--   0        0        0     3706 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/relaxation.py
+-rw-r--r--   0        0        0     1674 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/plotters/shift.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/printers/__init__.py
+-rw-r--r--   0        0        0     1785 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/printers/data.py
+-rw-r--r--   0        0        0     4510 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/printers/parameters.py
+-rw-r--r--   0        0        0     2679 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/printers/plot.py
+-rw-r--r--   0        0        0     2929 2023-04-14 11:37:01.945999 chemex-2022.3.1/chemex/toml.py
+-rw-r--r--   0        0        0       98 2023-04-14 11:37:01.949999 chemex-2022.3.1/chemex/tools/__init__.py
+-rw-r--r--   0        0        0     9332 2023-04-14 11:37:01.949999 chemex-2022.3.1/chemex/tools/pick_cest.py
+-rw-r--r--   0        0        0     1819 2023-04-14 11:37:01.949999 chemex-2022.3.1/chemex/tools/plot_param.py
+-rw-r--r--   0        0        0     2667 2023-04-14 11:37:01.949999 chemex-2022.3.1/chemex/uncertainty.py
+-rw-r--r--   0        0        0     1057 2023-04-14 11:37:02.122002 chemex-2022.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 chemex-2022.3.1/PKG-INFO
```

### Comparing `chemex-2022.3.0/LICENSE.md` & `chemex-2022.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/README.md` & `chemex-2022.3.1/README.md`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/chemex.py` & `chemex-2022.3.1/chemex/chemex.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/cli.py` & `chemex-2022.3.1/chemex/cli.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/configuration/conditions.py` & `chemex-2022.3.1/chemex/configuration/conditions.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/configuration/data.py` & `chemex-2022.3.1/chemex/configuration/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/configuration/experiment.py` & `chemex-2022.3.1/chemex/configuration/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/configuration/methods.py` & `chemex-2022.3.1/chemex/configuration/methods.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/configuration/parameters.py` & `chemex-2022.3.1/chemex/configuration/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/containers/data.py` & `chemex-2022.3.1/chemex/containers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/containers/dataset.py` & `chemex-2022.3.1/chemex/containers/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     data_path = normalize_path(base_path, settings.data.path)
     dtype = [("metadata", "f8"), ("exp", "f8"), ("err", "f8")]
 
     dataset: Dataset = []
     for spin_system, filepaths in settings.data.profiles.items():
         for filepath in filepaths:
-            raw_data = np.loadtxt(data_path / filepath, dtype=dtype)
+            raw_data = np.loadtxt(data_path / filepath, dtype=dtype, usecols=[0, 1, 2])
             dataset.append(
                 (
                     spin_system,
                     Data(
                         exp=raw_data["exp"],
                         err=raw_data["err"],
                         metadata=raw_data["metadata"],
```

### Comparing `chemex-2022.3.0/chemex/containers/experiment.py` & `chemex-2022.3.1/chemex/containers/experiment.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/containers/experiments.py` & `chemex-2022.3.1/chemex/containers/experiments.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/containers/profile.py` & `chemex-2022.3.1/chemex/containers/profile.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/builder.py` & `chemex-2022.3.1/chemex/experiments/builder.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cest_13c.py` & `chemex-2022.3.1/chemex/experiments/catalog/cest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cest_15n.py` & `chemex-2022.3.1/chemex/experiments/catalog/cest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cest_15n_cw.py` & `chemex-2022.3.1/chemex/experiments/catalog/cest_15n_cw.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cest_15n_tr.py` & `chemex-2022.3.1/chemex/experiments/catalog/cest_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cest_1hn_ap.py` & `chemex-2022.3.1/chemex/experiments/catalog/cest_1hn_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cest_1hn_ip_ap.py` & `chemex-2022.3.1/chemex/experiments/catalog/cest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py` & `chemex-2022.3.1/chemex/experiments/catalog/cest_ch3_1h_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/coscest_13c.py` & `chemex-2022.3.1/chemex/experiments/catalog/coscest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/coscest_1hn_ip_ap.py` & `chemex-2022.3.1/chemex/experiments/catalog/coscest_1hn_ip_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_13c_ip.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_13c_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_13co_ap.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_13co_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_15n_ip.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_ip.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_15n_ip_0013.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_ip_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_15n_tr.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_tr.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_15n_tr_0013.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_15n_tr_0013.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_1hn_ap.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_1hn_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_1hn_ap_0013.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_1hn_ap_0013.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
         state = self.experiment.observed_state
         return ToBeFitted(rates=[f"r2_i_{state}"], model_free=[f"tauc_{state}"])
 
 
 def build_spectrometer(
     config: Cpmg1HnAp0013Config, spin_system: SpinSystem
 ) -> Spectrometer:
-
     settings = config.experiment
     conditions = config.conditions
 
     basis = Basis(type="ixyzsz", spin_system="hn")
     liouvillian = LiouvillianIS(spin_system, basis, conditions)
     spectrometer = Spectrometer(liouvillian)
 
@@ -128,15 +127,14 @@
         )
         indexes = np.arange(int(ncyc))
         phases1 = np.take(cp_phases1, np.flip(indexes), mode="wrap", axis=1)
         phases2 = np.take(cp_phases2, indexes, mode="wrap", axis=1)
         return phases1, phases2
 
     def calculate(self, spectrometer: Spectrometer, data: Data) -> np.ndarray:
-
         ncycs = data.metadata
 
         # Calculation of the spectrometers corresponding to all the delays
         tau_cps, deltas, all_delays = self._get_delays(ncycs)
         delays = dict(zip(all_delays, spectrometer.delays(all_delays)))
         d_neg = delays[self.settings.t_neg]
         d_taua = delays[self.settings.taua]
@@ -147,35 +145,34 @@
 
         # Calculation of the spectrometers corresponding to all the pulses
         p90 = spectrometer.p90_i
         p180 = spectrometer.p180_i
         pp90_i = spectrometer.perfect90_i
         pp180_isx = spectrometer.perfect180_i[0] @ spectrometer.perfect180_s[0]
 
-        # Calculation of the spectrometers for INEPT and purge elements
+        # Calculation of the propagators for INEPT and purge elements
         inept = pp90_i[1] @ d_taua @ pp180_isx @ d_taua @ pp90_i[0]
         zfilter = spectrometer.zfilter
 
         # Getting the starting magnetization
         start = spectrometer.get_start_magnetization(terms=self.settings.start)
 
         # Calculating the central refocusing block
         if self.settings.eburp_flg:
             p180pmy = p180[[1, 3]]
             pp90pmy = spectrometer.perfect90_i[[1, 3]]
             e180e_pmy = pp90pmy @ d_eburp @ p180pmy @ d_eburp @ pp90pmy
-            middle = [p180pmy @ e180e_pmy, e180e_pmy @ p180pmy]
+            middle = np.stack([p180pmy @ e180e_pmy, e180e_pmy @ p180pmy])
         elif self.settings.reburp_flg:
             pp180pmy = spectrometer.perfect180_i[[1, 3]]
             middle = d_reburp @ pp180pmy @ d_reburp
         else:
             middle = p180[[1, 3]]
-        middle = np.mean(middle, axis=0)
 
-        # Calculating the instensities as a function of ncyc
+        # Calculating the intensities as a function of ncyc
         centre = {0.0: d_delta[0] @ p90[0] @ middle @ p90[0]}
 
         for ncyc in set(ncycs) - {0.0}:
             phases1, phases2 = self._get_phases(ncyc)
             echo = d_cp[ncyc] @ p180 @ d_cp[ncyc]
             cpmg1 = reduce(np.matmul, echo[phases1.T])
             cpmg2 = reduce(np.matmul, echo[phases2.T])
```

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_13c_h2c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_1h_dq.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_dq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_1h_sq.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_1h_tq.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_tq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_1h_tq_diff.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_ch3_mq.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_ch3_mq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_chd2_1h_ap.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_chd2_1h_ap.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/cpmg_hn_dq_zq.py` & `chemex-2022.3.1/chemex/experiments/catalog/cpmg_hn_dq_zq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/dcest_13c.py` & `chemex-2022.3.1/chemex/experiments/catalog/dcest_13c.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/dcest_15n.py` & `chemex-2022.3.1/chemex/experiments/catalog/dcest_15n.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/relaxation_hznz.py` & `chemex-2022.3.1/chemex/experiments/catalog/relaxation_hznz.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/relaxation_nz.py` & `chemex-2022.3.1/chemex/experiments/catalog/relaxation_nz.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/shift_15n_sq.py` & `chemex-2022.3.1/chemex/experiments/catalog/shift_15n_sq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/catalog/shift_15n_sqmq.py` & `chemex-2022.3.1/chemex/experiments/catalog/shift_15n_sqmq.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/factories.py` & `chemex-2022.3.1/chemex/experiments/factories.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/experiments/loader.py` & `chemex-2022.3.1/chemex/experiments/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/filterers.py` & `chemex-2022.3.1/chemex/filterers.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/messages.py` & `chemex-2022.3.1/chemex/messages.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/constraints.py` & `chemex-2022.3.1/chemex/models/constraints.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/factory.py` & `chemex-2022.3.1/chemex/models/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_1st.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_1st.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_2st.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_2st.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_2st_a_a2.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a2.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_2st_a_a3.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a3.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_2st_a_a4.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_2st_a_a4.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_2st_binding.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_2st_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_2st_eyring.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_2st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_2st_hd.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_2st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_2st_rs.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_2st_rs.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_3st_a_a2_a3.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_3st_a_a2_a3.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_3st_a_a2_a4.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_3st_a_a2_a4.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_3st_double_binding.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_3st_double_binding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_3st_eyring.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_3st_eyring.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_3st_induced_fit.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_3st_induced_fit.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_4st_hd.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_4st_hd.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/kinetic/settings_nst.py` & `chemex-2022.3.1/chemex/models/kinetic/settings_nst.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/loader.py` & `chemex-2022.3.1/chemex/models/loader.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/models/model.py` & `chemex-2022.3.1/chemex/models/model.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/nmr/basis.py` & `chemex-2022.3.1/chemex/nmr/basis.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/nmr/constants.py` & `chemex-2022.3.1/chemex/nmr/constants.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/nmr/liouvillian.py` & `chemex-2022.3.1/chemex/nmr/liouvillian.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/nmr/rates.py` & `chemex-2022.3.1/chemex/nmr/rates.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/nmr/spectrometer.py` & `chemex-2022.3.1/chemex/nmr/spectrometer.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/optimize/fitting.py` & `chemex-2022.3.1/chemex/optimize/fitting.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/optimize/gridding.py` & `chemex-2022.3.1/chemex/optimize/gridding.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/optimize/grouping.py` & `chemex-2022.3.1/chemex/optimize/grouping.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/optimize/helper.py` & `chemex-2022.3.1/chemex/optimize/helper.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/optimize/minimizer.py` & `chemex-2022.3.1/chemex/optimize/minimizer.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/parameters/database.py` & `chemex-2022.3.1/chemex/parameters/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,56 +51,53 @@
     to_be_evaluated = grid_expression.replace("lin", "np.linspace")
     to_be_evaluated = to_be_evaluated.replace("log", "np.geomspace")
     return np.asarray(eval(to_be_evaluated))
 
 
 @dataclass
 class ParameterCatalog:
-    __parameters: Parameters = field(default_factory=dict)
-    __index: ParameterIndex = ParameterIndex()
+    _parameters: Parameters = field(default_factory=dict)
+    _index: ParameterIndex = ParameterIndex()
 
     def _add(self, parameter: ParamSetting) -> None:
-
-        if parameter.id not in self.__parameters:
-            self.__parameters[parameter.id] = parameter
-            self.__index.add(parameter.param_name)
+        if parameter.id not in self._parameters:
+            self._parameters[parameter.id] = parameter
+            self._index.add(parameter.param_name)
 
         if parameter.vary:
-            self.__parameters[parameter.id].vary = True
-            self.__parameters[parameter.id].expr = ""
+            self._parameters[parameter.id].vary = True
+            self._parameters[parameter.id].expr = ""
 
     def add_multiple(self, parameters: Parameters) -> None:
         for parameter in parameters.values():
             self._add(parameter)
 
     def get_parameters(self, param_ids: Iterable[str]) -> Parameters:
-
         relevant_ids = set()
 
-        pool_ids = set(self.__parameters) & set(param_ids)
+        pool_ids = set(self._parameters) & set(param_ids)
 
         while pool_ids:
             for param_id in pool_ids.copy():
                 relevant_ids.add(param_id)
                 pool_ids.discard(param_id)
-                pool_ids.update(self.__parameters[param_id].dependencies)
+                pool_ids.update(self._parameters[param_id].dependencies)
             pool_ids -= relevant_ids
 
         return {
             param_id: parameter
-            for param_id, parameter in self.__parameters.items()
+            for param_id, parameter in self._parameters.items()
             if param_id in relevant_ids
         }
 
     def build_lmfit_params(
         self, param_ids: Iterable[str] | None = None
     ) -> ParametersLF:
-
         if param_ids is None:
-            param_ids = set(self.__parameters)
+            param_ids = set(self._parameters)
 
         parameters = self.get_parameters(param_ids)
 
         parameter_args = (parameter.args for parameter in parameters.values())
 
         usersyms = rate_functions | user_function_registry.get(model.name)
         lmfit_params = ParametersLF(usersyms=usersyms)
@@ -110,44 +107,43 @@
         for id, lf_param in lmfit_params.items():
             lf_param.stderr = parameters[id].stderr
 
         return lmfit_params
 
     def update_from_lmfit_params(self, parameters: ParametersLF) -> None:
         for param_id, parameter in parameters.items():
-            self.__parameters[param_id].value = parameter.value
-            self.__parameters[param_id].stderr = parameter.stderr
+            self._parameters[param_id].value = parameter.value
+            self._parameters[param_id].stderr = parameter.stderr
 
     def get_matching_ids(self, param_name: ParamName) -> set[str]:
-        return self.__index.get_matching_ids(param_name)
+        return self._index.get_matching_ids(param_name)
 
     def get_value(self, id_: str) -> float | None:
-        return self.__parameters[id_].value
+        return self._parameters[id_].value
 
     def set_values(self, par_values: dict[str, float]) -> None:
         for id_, value in par_values.items():
-            if id_ in self.__parameters:
-                self.__parameters[id_].value = value
+            if id_ in self._parameters:
+                self._parameters[id_].value = value
 
     def set_defaults(self, defaults: DefaultListType) -> None:
-        id_pool = set(self.__parameters)
+        id_pool = set(self._parameters)
         for name_to_set, setting in reversed(defaults):
             matching_ids = self.get_matching_ids(name_to_set) & id_pool
             id_pool -= matching_ids
             for matching_id in matching_ids:
-                self.__parameters[matching_id].set(setting)
+                self._parameters[matching_id].set(setting)
 
     def _count_per_section(self, param_ids: set[str]) -> Counter[str]:
         return Counter(
-            self.__parameters[param_id].param_name.section for param_id in param_ids
+            self._parameters[param_id].param_name.section for param_id in param_ids
         )
 
     def set_vary(self, section_names: Sequence[str], vary: bool) -> Counter[str]:
-
-        parameters = self.__parameters
+        parameters = self._parameters
 
         ids_modified = set()
         ids_pool = {
             param_id
             for param_id, setting in parameters.items()
             if setting.vary != vary or setting.expr
         }
@@ -160,65 +156,62 @@
                 if vary:
                     parameters[matching_id].expr = ""
             ids_modified.update(matching_ids)
 
         return self._count_per_section(ids_modified)
 
     def fix_all(self) -> None:
-        for parameter in self.__parameters.values():
+        for parameter in self._parameters.values():
             parameter.vary = False
 
     def _get_ids_left(self, expression: str) -> set[str]:
         return self.get_matching_ids(ParamName.from_section(expression))
 
     def _get_ids_right(self, expression: str) -> dict[str, set[str]]:
         ids_right = {}
         for match in _RE_PARAM_NAME.finditer(expression):
             param_name = ParamName.from_section(match.group(1))
             ids_right[match.group(0)] = self.get_matching_ids(param_name)
         return ids_right
 
     def _set_expression(self, expression: str, ids_pool: set[str]) -> set[str]:
-
         left, right, *something_else = expression.split("=")
 
         if something_else:
             print(
                 f'\nError reading constraints:\n  -> "{expression}"\n\nProgram aborted\n'
             )
             exit()
 
         ids_left = self._get_ids_left(left) & ids_pool
         ids_right_dict = self._get_ids_right(right)
 
         for id_left in ids_left:
             new_expression = right.strip()
             for section_name, ids_right in ids_right_dict.items():
-                name = self.__parameters[id_left].param_name
+                name = self._parameters[id_left].param_name
                 id_replace = name.get_closest_id(ids_right)
                 new_expression = new_expression.replace(section_name, id_replace)
-            self.__parameters[id_left].expr = new_expression
+            self._parameters[id_left].expr = new_expression
 
         return ids_left
 
     def set_expressions(self, expression_list: Sequence[str]) -> Counter[str]:
-
         ids_modified = set()
-        ids_pool = set(self.__parameters)
+        ids_pool = set(self._parameters)
 
         for expression in reversed(expression_list):
             ids_changed = self._set_expression(expression, ids_pool)
             ids_pool -= ids_changed
             ids_modified.update(ids_changed)
 
         return self._count_per_section(ids_modified)
 
     def parse_grid(self, grid_entries: list[str]) -> dict[str, np.ndarray]:
-
-        ids_pool = set(self.__parameters)
+        ids_pool = set(self._parameters)
 
         grid_values: dict[str, np.ndarray] = {}
 
         for entry in reversed(grid_entries):
             name, expression, *something_else = entry.replace(" ", "").split("=")
 
             if something_else or not _RE_GRID_DEFINITION.match(expression):
@@ -235,15 +228,15 @@
             self.set_vary([name], False)
 
         return grid_values
 
     def check_params(self):
         """Check whether the J couplings have the right sign"""
         messages = []
-        for setting in self.__parameters.values():
+        for setting in self._parameters.values():
             param_name = setting.param_name
             if not param_name.name.startswith("J_") or setting.value is None:
                 continue
             atoms = {atom.name for atom in param_name.spin_system.atoms.values()}
             if atoms == {"N", "H"} and setting.value > 0.0:
                 messages.append(
                     "Warning: Some 1J(NH) scalar couplings are set with positive values.\n"
@@ -258,33 +251,33 @@
                 )
         if messages:
             print("")
             print("\n\n".join(np.unique(messages)))
 
     def sort(self) -> None:
         sorted_items = sorted(
-            self.__parameters.items(), key=lambda item: item[1].param_name
+            self._parameters.items(), key=lambda item: item[1].param_name
         )
-        self.__parameters = dict(sorted_items)
+        self._parameters = dict(sorted_items)
 
 
 @dataclass
 class ParamManager:
-    __database: ParameterCatalog
-    __database_mf: ParameterCatalog
+    _database: ParameterCatalog
+    _database_mf: ParameterCatalog
 
     @property
     def database(self) -> ParameterCatalog:
-        return self.__database_mf if model.model_free else self.__database
+        return self._database_mf if model.model_free else self._database
 
     def add_multiple(self, parameters: Parameters) -> None:
-        self.__database.add_multiple(parameters)
+        self._database.add_multiple(parameters)
 
     def add_multiple_mf(self, parameters: Parameters) -> None:
-        self.__database_mf.add_multiple(parameters)
+        self._database_mf.add_multiple(parameters)
 
     def get_parameters(self, param_ids: Iterable[str]) -> Parameters:
         return self.database.get_parameters(param_ids)
 
     def get_value(self, param_id: str) -> float | None:
         return self.database.get_value(param_id)
 
@@ -297,21 +290,20 @@
     def update_from_parameters(self, parameters: ParametersLF) -> None:
         self.database.update_from_lmfit_params(parameters)
 
     def set_values(self, par_values: dict[str, float]) -> None:
         return self.database.set_values(par_values)
 
     def set_defaults(self, defaults: DefaultListType) -> None:
-
-        self.__database_mf.set_defaults(defaults)
+        self._database_mf.set_defaults(defaults)
 
         if model.model_free:
             return
 
-        params_mf = self.__database_mf.build_lmfit_params()
+        params_mf = self._database_mf.build_lmfit_params()
         self.database.set_values(params_mf.valuesdict())
 
         self.database.set_defaults(defaults)
 
         self.database.check_params()
 
     def set_vary(self, section_names: Sequence[str], vary: bool) -> Counter[str]:
```

### Comparing `chemex-2022.3.0/chemex/parameters/factory.py` & `chemex-2022.3.1/chemex/parameters/factory.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/parameters/name.py` & `chemex-2022.3.1/chemex/parameters/name.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/parameters/setting.py` & `chemex-2022.3.1/chemex/parameters/setting.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/parameters/spin_system.py` & `chemex-2022.3.1/chemex/parameters/spin_system.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/parameters/spins.py` & `chemex-2022.3.1/chemex/parameters/spins.py`

 * *Files 6% similar despite different names*

```diff
@@ -244,32 +244,38 @@
 
     return settings_mf
 
 
 def _select_relevant_settings(
     all_settings: LocalSettings, basis: Basis
 ) -> LocalSettings:
-
     pool = set(all_settings) & set(basis.matrices)
     selection = set()
     while pool:
         name = pool.pop()
         selection.add(name)
         pool |= all_settings[name].dependencies
 
     return {name: all_settings[name] for name in selection}
 
 
 def build_spin_param_settings(
     basis: Basis, conditions: Conditions
 ) -> tuple[LocalSettings, LocalSettings]:
-
     all_settings: LocalSettings = {}
     for state in model.states:
         all_settings.update(create_base_param_settings(basis, state, conditions))
 
     all_settings_mf = _build_model_free_settings(all_settings, basis, conditions)
 
     settings = _select_relevant_settings(all_settings, basis)
     settings_mf = _select_relevant_settings(all_settings_mf, basis)
 
+    # Add back to `settings_mf` the parameters that were selected in `settings`,
+    # but not in settings_mf. This can happen when a constraint require parameters
+    # that are not in the basis. This way the starting value of these parameters
+    # can be calculated using the model free parameters.
+    if not model.model_free:
+        names = set(settings) - set(settings_mf)
+        settings_mf |= {name: all_settings_mf[name] for name in names}
+
     return settings, settings_mf
```

### Comparing `chemex-2022.3.0/chemex/parameters/userfunctions.py` & `chemex-2022.3.1/chemex/parameters/userfunctions.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/plotters/cest.py` & `chemex-2022.3.1/chemex/plotters/cest.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/plotters/cpmg.py` & `chemex-2022.3.1/chemex/plotters/cpmg.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/plotters/plot.py` & `chemex-2022.3.1/chemex/plotters/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/plotters/relaxation.py` & `chemex-2022.3.1/chemex/plotters/relaxation.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/plotters/shift.py` & `chemex-2022.3.1/chemex/plotters/shift.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/printers/data.py` & `chemex-2022.3.1/chemex/printers/data.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/printers/parameters.py` & `chemex-2022.3.1/chemex/printers/parameters.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/printers/plot.py` & `chemex-2022.3.1/chemex/printers/plot.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/toml.py` & `chemex-2022.3.1/chemex/toml.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/tools/pick_cest.py` & `chemex-2022.3.1/chemex/tools/pick_cest.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/tools/plot_param.py` & `chemex-2022.3.1/chemex/tools/plot_param.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/chemex/uncertainty.py` & `chemex-2022.3.1/chemex/uncertainty.py`

 * *Files identical despite different names*

### Comparing `chemex-2022.3.0/pyproject.toml` & `chemex-2022.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "chemex"
-version = "2022.3.0"
+version = "2022.3.1"
 description = "ChemEx is an analysis program for chemical exchange detected by NMR"
 authors = ["Guillaume Bouvignies <gbouvignies@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/gbouvignies/chemex"
 homepage = "http://gbouvignies.github.io/ChemEx/"
 classifiers = [
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
 
   [tool.poetry.dependencies]
   python     = ">=3.9,<3.11"
-  numpy      = "^1.24.1"
-  scipy      = "^1.10.0"
-  matplotlib = "^3.6.2"
-  lmfit      = "^1.1.0"
-  pydantic   = "^1.10.4"
-  cachetools = "^5.2.0"
-  rich       = "^13.0.0"
+  numpy      = "^1.24.2"
+  scipy      = "^1.10.1"
+  matplotlib = "^3.7.1"
+  lmfit      = "^1.2.0"
+  pydantic   = "^1.10.7"
+  cachetools = "^5.3.0"
+  rich       = "^13.3.4"
   tomli      = "^2.0.1"
-  rapidfuzz  = "^2.13.7"
+  rapidfuzz  = "^2.15.1"
 
   [tool.poetry.group.dev.dependencies]
-  pre-commit       = "^2.17.0"
-  types-cachetools = "^4.2.9"
+  pre-commit       = ">=2.17,<4.0"
+  types-cachetools = ">=4.2.9,<6.0.0"
 
 [tool.poetry.scripts]
 chemex = "chemex.chemex:main"
 
 [tool.black]
 target-version = ['py39']
```

### Comparing `chemex-2022.3.0/PKG-INFO` & `chemex-2022.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: chemex
-Version: 2022.3.0
+Version: 2022.3.1
 Summary: ChemEx is an analysis program for chemical exchange detected by NMR
 Home-page: http://gbouvignies.github.io/ChemEx/
 License: GPL-3.0-only
 Author: Guillaume Bouvignies
 Author-email: gbouvignies@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: cachetools (>=5.2.0,<6.0.0)
-Requires-Dist: lmfit (>=1.1.0,<2.0.0)
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: rapidfuzz (>=2.13.7,<3.0.0)
-Requires-Dist: rich (>=13.0.0,<14.0.0)
-Requires-Dist: scipy (>=1.10.0,<2.0.0)
+Requires-Dist: cachetools (>=5.3.0,<6.0.0)
+Requires-Dist: lmfit (>=1.2.0,<2.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: rapidfuzz (>=2.15.1,<3.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/gbouvignies/chemex
 Description-Content-Type: text/markdown
 
 # ChemEx
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

