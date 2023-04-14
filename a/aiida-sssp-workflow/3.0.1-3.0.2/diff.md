# Comparing `tmp/aiida_sssp_workflow-3.0.1.tar.gz` & `tmp/aiida_sssp_workflow-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_sssp_workflow-3.0.1.tar", last modified: Fri Mar 31 16:17:22 2023, max compression
+gzip compressed data, was "aiida_sssp_workflow-3.0.2.tar", last modified: Fri Apr 14 09:00:31 2023, max compression
```

## Comparing `aiida_sssp_workflow-3.0.1.tar` & `aiida_sssp_workflow-3.0.2.tar`

### file list

```diff
@@ -1,1136 +1,1136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.518894 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.522894 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/birch_murnaghan_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/calculate_bands_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/calculate_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/wien2k_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.522894 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.522894 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/tools/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/tools/relabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/efermi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.522894 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/bands.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/control.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/criteria.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/delta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.522894 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.522894 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/
--rw-r--r--   0 runner    (1001) docker     (123)   113612 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/AE-average-oxides.json
--rw-r--r--   0 runner    (1001) docker     (123)    81057 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/AE-average-unaries.json
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_LANN.json
--rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_TYPICAL.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.522894 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/mapping.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.602895 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O3.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O5.cif
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_XO.cif
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_XO2.cif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_XO3.cif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.614896 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ag.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Al.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ar.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/As.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Au.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/B.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ba.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Be.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Bi.cif
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Br.cif
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/C.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ca.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cd.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/CeN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cl.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Co.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cr.cif
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cs.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cu.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/DyN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/ErN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/EuN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/F.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Fe.cif
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ga.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/GdN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ge.cif
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/H.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/He.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Hf.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Hg.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/HoN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/I.cif
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/In.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ir.cif
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/K.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Kr.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/LaN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Li.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Lu.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/LuN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Mg.cif
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Mn.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Mo.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/N.cif
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Na.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Nb.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/NdN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ne.cif
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ni.cif
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/O.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Os.cif
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/P.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Pb.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Pd.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/PmN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Po.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/PrN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Pt.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Rb.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Re.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Rh.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Rn.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ru.cif
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/S.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Sb.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Sc.cif
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Se.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Si.cif
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/SiF4.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/SmN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Sn.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Sr.cif
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ta.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/TbN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Tc.cif
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Te.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ti.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Tl.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/TmN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/V.cif
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/W.cif
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Xe.cif
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Y.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/YbN.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Zn.cif
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Zr.cif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.678897 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ac_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ac_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ac_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ac_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ag_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ag_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ag_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ag_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Al_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Al_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Al_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Al_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Am_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Am_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Am_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Am_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ar_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ar_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ar_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ar_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/As_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/As_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/As_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/As_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/At_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/At_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/At_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/At_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Au_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Au_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Au_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Au_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/B_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/B_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/B_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/B_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ba_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ba_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ba_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ba_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Be_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Be_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Be_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Be_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Bi_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Bi_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Bi_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Bi_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Br_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Br_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Br_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Br_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/C_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/C_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/C_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/C_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ca_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ca_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ca_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ca_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cd_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cd_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cd_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cd_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ce_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ce_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ce_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ce_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cl_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cl_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cl_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cl_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cm_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cm_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cm_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cm_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Co_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Co_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Co_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Co_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cs_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cs_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cs_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cs_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cu_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cu_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cu_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cu_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Dy_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Dy_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Dy_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Dy_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Er_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Er_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Er_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Er_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Eu_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Eu_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Eu_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Eu_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/F_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/F_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/F_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/F_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fe_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fe_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fe_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fe_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ga_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ga_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ga_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ga_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Gd_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Gd_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Gd_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Gd_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ge_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ge_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ge_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ge_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/H_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/H_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/H_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/H_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/He_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/He_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/He_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/He_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hf_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hf_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hf_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hf_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hg_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hg_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hg_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hg_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ho_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ho_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ho_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ho_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/I_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/I_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/I_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/I_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/In_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/In_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/In_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/In_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ir_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ir_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ir_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ir_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/K_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/K_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/K_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/K_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Kr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Kr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Kr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Kr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/La_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/La_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/La_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/La_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Li_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Li_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Li_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Li_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Lu_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Lu_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Lu_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Lu_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mg_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mg_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mg_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mg_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mn_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mn_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mn_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mn_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mo_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mo_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mo_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mo_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/N_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/N_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/N_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/N_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Na_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Na_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Na_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Na_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nd_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nd_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nd_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nd_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ne_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ne_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ne_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ne_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ni_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ni_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ni_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ni_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Np_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Np_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Np_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Np_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/O_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/O_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/O_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/O_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Os_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Os_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Os_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Os_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/P_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/P_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/P_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/P_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pa_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pa_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pa_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pa_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pd_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pd_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pd_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pd_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pm_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pm_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pm_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pm_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Po_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Po_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Po_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Po_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pt_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pt_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pt_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pt_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pu_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pu_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pu_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pu_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ra_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ra_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ra_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ra_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Re_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Re_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Re_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Re_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rh_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rh_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rh_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rh_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rn_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rn_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rn_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rn_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ru_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ru_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ru_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ru_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/S_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/S_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/S_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/S_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sc_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sc_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sc_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sc_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Se_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Se_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Se_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Se_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Si_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Si_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Si_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Si_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sm_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sm_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sm_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sm_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sn_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sn_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sn_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sn_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ta_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ta_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ta_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ta_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tc_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tc_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tc_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tc_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Te_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Te_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Te_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Te_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Th_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Th_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Th_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Th_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ti_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ti_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ti_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ti_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tl_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tl_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tl_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tl_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tm_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tm_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tm_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tm_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/U_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/U_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/U_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/U_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/V_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/V_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/V_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/V_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/W_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/W_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/W_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/W_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Xe_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Xe_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Xe_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Xe_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Y_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Y_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Y_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Y_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Yb_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Yb_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Yb_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Yb_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zn_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zn_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zn_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zn_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zr_BCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zr_Diamond.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zr_FCC.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zr_SC.cif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.678897 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/upf/
--rw-r--r--   0 runner    (1001) docker     (123)   632448 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/upf/N.us.z_5.ld1.theose.v0.upf
--rw-r--r--   0 runner    (1001) docker     (123)   880280 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/upf/O.paw.z_6.ld1.psl.v0.1.upf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/upf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.678897 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23611 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/bands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/cohesive_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/phonon_frequencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/pressure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_bands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_cohesive_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_eos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_phonon_frequencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_pressure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/measure/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/measure/bands.py
--rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/measure/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/verifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.518894 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-03-31 16:17:22.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    55501 2023-03-31 16:17:22.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 16:17:22.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-31 16:17:22.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-31 16:17:22.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-31 16:17:22.000000 aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/efermi/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/efermi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/pseudo_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/pseudo_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/pseudo_parser/upf_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/pseudo_parser/upf_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:17:22.682897 aiida_sssp_workflow-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-03-31 16:17:13.000000 aiida_sssp_workflow-3.0.1/tests/test_nightly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.715153 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/birch_murnaghan_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/calculate_bands_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/calculate_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/wien2k_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/relabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/efermi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/bands.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/control.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/criteria.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/delta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/
+-rw-r--r--   0 runner    (1001) docker     (123)   113612 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/AE-average-oxides.json
+-rw-r--r--   0 runner    (1001) docker     (123)    81057 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/AE-average-unaries.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_LANN.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_TYPICAL.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.787159 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O5.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_XO.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_XO2.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_XO3.cif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.799159 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ag.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Al.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ar.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/As.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Au.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/B.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ba.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Be.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Bi.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Br.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/C.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ca.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cd.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/CeN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cl.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Co.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cr.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cs.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cu.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/DyN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/ErN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/EuN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/F.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Fe.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ga.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/GdN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ge.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/H.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/He.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Hf.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Hg.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/HoN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/I.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/In.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ir.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/K.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Kr.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/LaN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Li.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Lu.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/LuN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Mg.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Mn.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Mo.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/N.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Na.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Nb.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/NdN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ne.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ni.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/O.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Os.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/P.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Pb.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Pd.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/PmN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Po.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/PrN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Pt.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Rb.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Re.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Rh.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Rn.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ru.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/S.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sb.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sc.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Se.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Si.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/SiF4.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/SmN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sn.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sr.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ta.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/TbN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Tc.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Te.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ti.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Tl.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/TmN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/V.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/W.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Xe.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Y.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/YbN.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Zn.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Zr.cif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.871165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_BCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_Diamond.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_FCC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_SC.cif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.871165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/
+-rw-r--r--   0 runner    (1001) docker     (123)   632448 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/N.us.z_5.ld1.theose.v0.upf
+-rw-r--r--   0 runner    (1001) docker     (123)   880280 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/O.paw.z_6.ld1.psl.v0.1.upf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.871165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/cohesive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/phonon_frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/pressure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_cohesive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_eos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_phonon_frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_pressure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/verifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.719154 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    55501 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 09:00:31.000000 aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/efermi/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/efermi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/pseudo_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/pseudo_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/pseudo_parser/upf_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/pseudo_parser/upf_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:00:31.875165 aiida_sssp_workflow-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-14 09:00:22.000000 aiida_sssp_workflow-3.0.2/tests/test_nightly.py
```

### Comparing `aiida_sssp_workflow-3.0.1/LICENSE` & `aiida_sssp_workflow-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/PKG-INFO` & `aiida_sssp_workflow-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida_sssp_workflow
-Version: 3.0.1
+Version: 3.0.2
 Summary: Package for the AiiDA SSSP workflow
 Home-page: https://github.com/aiidateam/aiida-sssp-workflow
 Author: Jusong Yu
 Author-email: jusong.yu@epfl.ch
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aiidateam/aiida-sssp-workflow/issues
 Classifier: License :: OSI Approved :: MIT License
@@ -191,14 +191,21 @@
 ### Logger level
 
 The aiida-core logger level is recommened to set to `REPORT` as default.
 In workflow, process related messages are pop to daemon logger in REPORT level.
 If process finished with none-zero exit_code, log a waring message.
 While for debug purpose, the INFO level is for showing the parameters infomations when processes are launched.
 
+### Issues of version
+
+- v3.0.1:
+    - nowf not turned on for saving inode purpose, fixed in next version
+    - the dual value of NC/SL is 8 for delta measure and bands for norm-conserving pseudopotentials, better to be 4. fixed in next version
+    - the dual value for high dual elements is 8 for non-NC pseudopotentials, better to be 16. fixed in next version
+
 ## License
 
 MIT
 
 
 ## Contact
```

### Comparing `aiida_sssp_workflow-3.0.1/README.md` & `aiida_sssp_workflow-3.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -169,14 +169,21 @@
 ### Logger level
 
 The aiida-core logger level is recommened to set to `REPORT` as default.
 In workflow, process related messages are pop to daemon logger in REPORT level.
 If process finished with none-zero exit_code, log a waring message.
 While for debug purpose, the INFO level is for showing the parameters infomations when processes are launched.
 
+### Issues of version
+
+- v3.0.1:
+    - nowf not turned on for saving inode purpose, fixed in next version
+    - the dual value of NC/SL is 8 for delta measure and bands for norm-conserving pseudopotentials, better to be 4. fixed in next version
+    - the dual value for high dual elements is 8 for non-NC pseudopotentials, better to be 16. fixed in next version
+
 ## License
 
 MIT
 
 
 ## Contact
```

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/birch_murnaghan_fit.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/birch_murnaghan_fit.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/calculate_bands_distance.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/calculate_bands_distance.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/calculate_delta.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/calculate_delta.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/calculations/wien2k_ref.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/calculations/wien2k_ref.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/__init__.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/extract.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/extract.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/run.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/run.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/tools/dump.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/dump.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/cli/tools/relabel.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/cli/tools/relabel.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/efermi.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/efermi.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/bands.yml` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/bands.yml`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/control.yml` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/control.yml`

 * *Files 1% similar despite different names*

```diff
@@ -34,12 +34,12 @@
     nc_dual_scan: [2.0, 4.0] # at fix wfc
     nonnc_dual_scan: [6.0, 8.0]
     nonnc_high_dual_scan: [8.0, 12.0]
 
 opsp:
     description: To running opsp verification, make the calculations finished fast.
 
-    max_wfc: 50 # The max wfc cut for delta measure
-    wfc_scan: [30, 35, 40] # at fix rho
+    max_wfc: 40 # The max wfc cut for delta measure
+    wfc_scan: [30, 35] # at fix rho
     nc_dual_scan: [2.0, 4.0] # at fix wfc
     nonnc_dual_scan: [6.0, 8.0]
     nonnc_high_dual_scan: [8.0, 12.0]
```

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/converge.yml` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/converge.yml`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/criteria.yml` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/criteria.yml`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/protocol/delta.yml` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/protocol/delta.yml`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
     degauss: 0.0045
     smearing: fd
     electron_conv_thr: 1.0e-8
     kpoints_distance: 0.2
     scale_count: 7
     scale_increment: 0.02
     configurations:
-        - XO
         - XO2
-        - BCC
         - SC
 
 opsp-full:
     name: opsp-full
     description: For OPSP verifications with all configurations
 
     occupations: smearing
```

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/AE-average-oxides.json` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/AE-average-oxides.json`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/AE-average-unaries.json` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/AE-average-unaries.json`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_LANN.json` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_LANN.json`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_TYPICAL.json` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/AE_EOS/WIEN2K_TYPICAL.json`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/mapping.json` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/mapping.json`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ac_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ac_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ag_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ag_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Al_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Al_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Am_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Am_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ar_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ar_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/As_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/As_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/At_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/At_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Au_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Au_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/B_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/B_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ba_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ba_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Be_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Be_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Bi_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Bi_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Br_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Br_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/C_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/C_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ca_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ca_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cd_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cd_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ce_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ce_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cl_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cl_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cm_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cm_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Co_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Co_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cr_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cr_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cs_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cs_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Cu_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Cu_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Dy_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Dy_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Er_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Er_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Eu_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Eu_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/F_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/F_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fe_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fe_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Fr_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Fr_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ga_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ga_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Gd_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Gd_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ge_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ge_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/H_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/H_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/He_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/He_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hf_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hf_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Hg_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Hg_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ho_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ho_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/I_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/I_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/In_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/In_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ir_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ir_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/K_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/K_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Kr_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Kr_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/La_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/La_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Li_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Li_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Lu_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Lu_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mg_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mg_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mn_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mn_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Mo_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Mo_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/N_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/N_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Na_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Na_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nb_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nb_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Nd_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Nd_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ne_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ne_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ni_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ni_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Np_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Np_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Os_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Os_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/P_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/P_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pa_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pa_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pb_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pb_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pd_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pd_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pm_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pm_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Po_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Po_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pr_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pr_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pt_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pt_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Pu_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Pu_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ra_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ra_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rb_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rb_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Re_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Re_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rh_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rh_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Rn_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Rn_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ru_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ru_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/S_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/S_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sb_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sb_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sc_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sc_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Se_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Se_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Si_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Si_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sm_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sm_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sn_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sn_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Sr_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Sr_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ta_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ta_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tb_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tb_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tc_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tc_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Te_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Te_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Th_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Th_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Ti_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Ti_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tl_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tl_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Tm_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Tm_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/U_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/U_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/V_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/V_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/W_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/W_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Xe_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Xe_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Y_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Y_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Yb_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Yb_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zn_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zn_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O5.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_X2O5.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_XO.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_XO.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_XO2.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_XO2.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/oxides/Zr_XO3.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/oxides/Zr_XO3.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ag.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ag.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Al.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Al.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ar.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ar.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/As.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/As.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Au.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Au.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/B.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/B.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ba.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ba.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Be.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Be.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Bi.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Bi.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Br.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Br.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/C.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/C.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ca.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ca.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cd.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cd.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/CeN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/CeN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cl.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cl.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Co.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Co.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cr.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cr.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cs.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cs.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Cu.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Cu.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/DyN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/DyN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/ErN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/ErN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/EuN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/EuN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/F.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/F.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Fe.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Fe.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ga.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ga.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/GdN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/GdN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ge.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ge.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/H.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/H.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/He.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/He.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Hf.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Hf.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Hg.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Hg.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/HoN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/HoN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/I.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/I.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/In.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/In.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ir.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ir.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/K.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/K.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Kr.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Kr.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/LaN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/LaN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Li.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Li.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Lu.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Lu.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/LuN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/LuN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Mg.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Mg.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Mn.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Mn.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Mo.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Mo.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/N.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/N.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Na.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Na.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Nb.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Nb.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/NdN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/NdN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ne.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ne.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ni.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ni.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/O.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/O.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Os.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Os.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/P.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/P.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Pb.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Pb.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Pd.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Pd.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/PmN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/PmN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Po.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Po.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/PrN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/PrN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Pt.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Pt.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Rb.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Rb.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Re.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Re.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Rh.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Rh.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Rn.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Rn.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ru.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ru.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/S.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/S.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Sb.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sb.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Sc.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sc.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Se.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Se.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Si.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Si.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/SiF4.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/SiF4.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/SmN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/SmN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Sn.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sn.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Sr.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Sr.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ta.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ta.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/TbN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/TbN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Tc.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Tc.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Te.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Te.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Ti.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Ti.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Tl.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Tl.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/TmN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/TmN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/V.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/V.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/W.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/W.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Xe.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Xe.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Y.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Y.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/YbN.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/YbN.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Zn.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Zn.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/typical/Zr.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/typical/Zr.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ac_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ac_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ac_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ac_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ac_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ag_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ag_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ag_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ag_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ag_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Al_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Al_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Al_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Al_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Al_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Am_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Am_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Am_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Am_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Am_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ar_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ar_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ar_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ar_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ar_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/As_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/As_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/As_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/As_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/As_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/At_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/At_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/At_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/At_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/At_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Au_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Au_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Au_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Au_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Au_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/B_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/B_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/B_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/B_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/B_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ba_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ba_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ba_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ba_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ba_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Be_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Be_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Be_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Be_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Be_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Bi_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Bi_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Bi_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Bi_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Bi_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Br_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Br_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Br_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Br_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Br_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/C_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/C_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/C_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/C_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/C_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ca_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ca_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ca_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ca_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ca_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cd_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cd_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cd_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cd_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cd_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ce_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ce_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ce_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ce_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ce_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cl_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cl_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cl_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cl_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cl_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cm_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cm_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cm_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cm_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cm_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Co_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Co_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Co_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Co_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Co_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cr_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cr_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cr_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cr_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cr_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cs_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cs_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cs_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cs_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cs_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cu_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cu_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cu_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Cu_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Cu_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Dy_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Dy_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Dy_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Dy_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Dy_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Er_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Er_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Er_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Er_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Er_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Eu_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Eu_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Eu_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Eu_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Eu_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/F_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/F_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/F_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/F_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/F_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fe_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fe_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fe_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fe_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fe_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fr_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fr_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fr_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Fr_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Fr_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ga_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ga_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ga_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ga_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ga_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Gd_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Gd_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Gd_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Gd_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Gd_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ge_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ge_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ge_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ge_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ge_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/H_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/H_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/H_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/H_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/H_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/He_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/He_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/He_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/He_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/He_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hf_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hf_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hf_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hf_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hf_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hg_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hg_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hg_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Hg_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Hg_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ho_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ho_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ho_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ho_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ho_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/I_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/I_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/I_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/I_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/I_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/In_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/In_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/In_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/In_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/In_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ir_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ir_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ir_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ir_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ir_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/K_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/K_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/K_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/K_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/K_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Kr_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Kr_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Kr_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Kr_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Kr_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/La_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/La_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/La_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/La_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/La_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Li_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Li_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Li_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Li_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Li_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Lu_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Lu_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Lu_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Lu_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Lu_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mg_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mg_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mg_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mg_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mg_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mn_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mn_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mn_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mn_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mn_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mo_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mo_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mo_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Mo_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Mo_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/N_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/N_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/N_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/N_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/N_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Na_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Na_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Na_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Na_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Na_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nb_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nb_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nb_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nb_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nb_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nd_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nd_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nd_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Nd_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Nd_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ne_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ne_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ne_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ne_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ne_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ni_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ni_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ni_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ni_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ni_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Np_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Np_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Np_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Np_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Np_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/O_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/O_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/O_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/O_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/O_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Os_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Os_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Os_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Os_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Os_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/P_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/P_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/P_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/P_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/P_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pa_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pa_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pa_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pa_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pa_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pb_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pb_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pb_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pb_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pb_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pd_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pd_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pd_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pd_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pd_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pm_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pm_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pm_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pm_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pm_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Po_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Po_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Po_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Po_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Po_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pr_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pr_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pr_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pr_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pr_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pt_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pt_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pt_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pt_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pt_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pu_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pu_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pu_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Pu_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Pu_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ra_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ra_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ra_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ra_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ra_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rb_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rb_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rb_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rb_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rb_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Re_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Re_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Re_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Re_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Re_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rh_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rh_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rh_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rh_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rh_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rn_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rn_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rn_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Rn_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Rn_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ru_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ru_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ru_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ru_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ru_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/S_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/S_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/S_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/S_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/S_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sb_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sb_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sb_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sb_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sb_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sc_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sc_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sc_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sc_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sc_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Se_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Se_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Se_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Se_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Se_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Si_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Si_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Si_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Si_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Si_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sm_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sm_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sm_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sm_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sm_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sn_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sn_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sn_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sn_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sn_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sr_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sr_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sr_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Sr_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Sr_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ta_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ta_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ta_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ta_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ta_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tb_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tb_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tb_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tb_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tb_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tc_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tc_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tc_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tc_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tc_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Te_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Te_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Te_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Te_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Te_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Th_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Th_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Th_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Th_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Th_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ti_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ti_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ti_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Ti_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Ti_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tl_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tl_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tl_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tl_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tl_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tm_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tm_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tm_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Tm_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Tm_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/U_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/U_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/U_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/U_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/U_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/V_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/V_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/V_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/V_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/V_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/W_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/W_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/W_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/W_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/W_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Xe_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Xe_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Xe_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Xe_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Xe_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Y_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Y_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Y_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Y_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Y_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Yb_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Yb_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Yb_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Yb_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Yb_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zn_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zn_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zn_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zn_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zn_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zr_BCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_BCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zr_Diamond.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_Diamond.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zr_FCC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_FCC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/cif/unaries/Zr_SC.cif` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/cif/unaries/Zr_SC.cif`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/upf/N.us.z_5.ld1.theose.v0.upf` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/N.us.z_5.ld1.theose.v0.upf`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/statics/upf/O.paw.z_6.ld1.psl.v0.1.upf` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/statics/upf/O.paw.z_6.ld1.psl.v0.1.upf`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/utils.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/__init__.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/common.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/common.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/_base.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         self.ctx.reference_ecutwfc = self._ECUTWFC_LIST[-1]
 
         self.ctx.extra_pw_parameters = {}
         self.ctx.element, self.ctx.pseudo_type = get_pseudo_element_and_type(self.inputs.pseudo)
 
         # set the ecutrho according to the type of pseudopotential
         # dual 4 for NC and 10 for all other type of PP.
-        if self.ctx.pseudo_type == 'nc':
+        if self.ctx.pseudo_type in ['nc', 'sl']:
             self.ctx.dual = 4.0
             self.ctx.dual_scan_list = cutoff_control['nc_dual_scan']
         else:
             if self.ctx.element  in HIGH_DUAL_ELEMENTS:
                 self.ctx.dual = 18.0
                 self.ctx.dual_scan_list = cutoff_control['nonnc_high_dual_scan']
             else:
```

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/bands.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/bands.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/caching.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/caching.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/cohesive_energy.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/cohesive_energy.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/delta.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/delta.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/phonon_frequencies.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/phonon_frequencies.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/convergence/pressure.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/convergence/pressure.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/__init__.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_bands.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_bands.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_cohesive_energy.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_cohesive_energy.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_delta.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_delta.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_eos.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_eos.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_phonon_frequencies.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_phonon_frequencies.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/evaluate/_pressure.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/evaluate/_pressure.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/measure/__init__.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/measure/bands.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/bands.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,20 +160,20 @@
         )
 
     def _get_inputs(self, pseudos):
         """
         get inputs for the bands evaluation with given pseudo
         """
         element, pseudo_type = get_pseudo_element_and_type(self.inputs.pseudo)
-        if pseudo_type in ['NC', 'SL']:
+        if pseudo_type in ['nc', 'sl']:
             ecutrho = self.ctx.ecutwfc * 4
         else:
             ecutrho = self.ctx.ecutwfc * 8
 
-        if element in HIGH_DUAL_ELEMENTS and pseudo_type not in ['NC', 'SL']:
+        if element in HIGH_DUAL_ELEMENTS and pseudo_type not in ['nc', 'sl']:
             ecutrho = self.ctx.ecutwfc * 18
 
         if element in RARE_EARTH_ELEMENTS:
             # since nitrides is used, the pseudo of N is non-NC
             # The N.us.z_5.ld1.theose.v0 is used so set dual equal to 8
             ecutrho = self.ctx.ecutwfc * 8
```

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/measure/delta.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/measure/delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
                 pw_parameters["SYSTEM"]["nbnd"] = int(nbnd)
 
         if configuration in self._UNARIE_CONFIGURATIONS:  # include regular 'TYPICAL'
             # pseudos for BCC, FCC, SC, Diamond and TYPYCAL configurations
             pseudos = self.ctx.pseudos_elementary
             pw_parameters = self.ctx.pw_parameters
             kpoints_distance = self.ctx.kpoints_distance
-            if pseudo_type in ["NC", "SL"]:
+            if pseudo_type in ["nc", "sl"]:
                 ecutrho = self.ctx.ecutwfc * 4
             else:
                 ecutrho = self.ctx.ecutwfc * 8
 
         if configuration == "TYPICAL" and self.ctx.element in MAGNETIC_ELEMENTS:
             # specific setting for magnetic elements typical since mag on
             pseudos = self.ctx.pseudos_magnetic
@@ -330,15 +330,15 @@
                 },
             }
             pw_parameters = update_dict(parameters, self.ctx.pw_nitride_parameters)
             kpoints_distance = self.ctx.kpoints_distance + 0.1
             # Since non-NC nitrogen pseudo is used
             ecutrho = self.ctx.ecutwfc * 8
 
-        if element in HIGH_DUAL_ELEMENTS and pseudo_type not in ["NC", "SL"]:
+        if element in HIGH_DUAL_ELEMENTS and pseudo_type not in ["nc", "sl"]:
             ecutrho = self.ctx.ecutwfc * 18
 
         parameters = {
             "SYSTEM": {
                 "ecutwfc": round(self.ctx.ecutwfc),
                 "ecutrho": round(ecutrho),
             },
```

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow/workflows/verifications.py` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow/workflows/verifications.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/PKG-INFO` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-sssp-workflow
-Version: 3.0.1
+Version: 3.0.2
 Summary: Package for the AiiDA SSSP workflow
 Home-page: https://github.com/aiidateam/aiida-sssp-workflow
 Author: Jusong Yu
 Author-email: jusong.yu@epfl.ch
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aiidateam/aiida-sssp-workflow/issues
 Classifier: License :: OSI Approved :: MIT License
@@ -191,14 +191,21 @@
 ### Logger level
 
 The aiida-core logger level is recommened to set to `REPORT` as default.
 In workflow, process related messages are pop to daemon logger in REPORT level.
 If process finished with none-zero exit_code, log a waring message.
 While for debug purpose, the INFO level is for showing the parameters infomations when processes are launched.
 
+### Issues of version
+
+- v3.0.1:
+    - nowf not turned on for saving inode purpose, fixed in next version
+    - the dual value of NC/SL is 8 for delta measure and bands for norm-conserving pseudopotentials, better to be 4. fixed in next version
+    - the dual value for high dual elements is 8 for non-NC pseudopotentials, better to be 16. fixed in next version
+
 ## License
 
 MIT
 
 
 ## Contact
```

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/SOURCES.txt` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/aiida_sssp_workflow.egg-info/entry_points.txt` & `aiida_sssp_workflow-3.0.2/aiida_sssp_workflow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/pseudo_parser/upf_parser/__init__.py` & `aiida_sssp_workflow-3.0.2/pseudo_parser/upf_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_sssp_workflow-3.0.1/setup.cfg` & `aiida_sssp_workflow-3.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aiida_sssp_workflow
-version = 3.0.1
+version = 3.0.2
 description = Package for the AiiDA SSSP workflow
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aiidateam/aiida-sssp-workflow
 author = Jusong Yu
 author_email = jusong.yu@epfl.ch
 license = MIT
@@ -64,15 +64,15 @@
 [flake8]
 ignore = 
 	E501  # Line length handled by black.
 	W503  # Line break before binary operator, preferred formatting for black.
 	E203  # Whitespace before ':', preferred formatting for black.
 
 [bumpver]
-current_version = "3.0.1"
+current_version = "3.0.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `aiida_sssp_workflow-3.0.1/tests/test_nightly.py` & `aiida_sssp_workflow-3.0.2/tests/test_nightly.py`

 * *Files identical despite different names*

