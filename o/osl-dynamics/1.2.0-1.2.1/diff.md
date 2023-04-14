# Comparing `tmp/osl-dynamics-1.2.0.tar.gz` & `tmp/osl-dynamics-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osl-dynamics-1.2.0.tar", last modified: Mon Mar 20 14:15:39 2023, max compression
+gzip compressed data, was "osl-dynamics-1.2.1.tar", last modified: Fri Apr 14 14:57:17 2023, max compression
```

## Comparing `osl-dynamics-1.2.0.tar` & `osl-dynamics-1.2.1.tar`

### file list

```diff
@@ -1,187 +1,192 @@
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:39.358438 osl-dynamics-1.2.0/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5462 2023-03-20 14:15:39.358653 osl-dynamics-1.2.0/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5149 2023-03-19 14:43:44.000000 osl-dynamics-1.2.0/README.rst
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:37.646217 osl-dynamics-1.2.0/osl_dynamics/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      574 2023-02-20 16:10:35.000000 osl-dynamics-1.2.0/osl_dynamics/__init__.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:37.848600 osl-dynamics-1.2.0/osl_dynamics/analysis/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      215 2023-02-19 13:57:27.000000 osl-dynamics-1.2.0/osl_dynamics/analysis/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    26615 2023-03-12 11:34:38.000000 osl-dynamics-1.2.0/osl_dynamics/analysis/connectivity.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5751 2023-03-13 17:18:28.000000 osl-dynamics-1.2.0/osl_dynamics/analysis/gmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20807 2023-02-19 13:57:27.000000 osl-dynamics-1.2.0/osl_dynamics/analysis/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    16620 2023-03-16 10:16:55.000000 osl-dynamics-1.2.0/osl_dynamics/analysis/power.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3268 2023-02-19 13:57:27.000000 osl-dynamics-1.2.0/osl_dynamics/analysis/regression.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    43342 2023-02-19 13:57:27.000000 osl-dynamics-1.2.0/osl_dynamics/analysis/spectral.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6857 2023-02-19 13:57:27.000000 osl-dynamics-1.2.0/osl_dynamics/analysis/static.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5683 2023-02-13 16:00:07.000000 osl-dynamics-1.2.0/osl_dynamics/analysis/workbench.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7257 2022-10-30 10:07:31.000000 osl-dynamics-1.2.0/osl_dynamics/array_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:37.903337 osl-dynamics-1.2.0/osl_dynamics/data/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      185 2023-01-28 15:39:30.000000 osl-dynamics-1.2.0/osl_dynamics/data/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    35304 2023-03-19 18:18:38.000000 osl-dynamics-1.2.0/osl_dynamics/data/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-01-28 15:39:30.000000 osl-dynamics-1.2.0/osl_dynamics/data/osl.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6752 2023-02-13 16:00:07.000000 osl-dynamics-1.2.0/osl_dynamics/data/processing.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8574 2023-03-19 18:18:38.000000 osl-dynamics-1.2.0/osl_dynamics/data/rw.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2809 2023-03-18 14:07:34.000000 osl-dynamics-1.2.0/osl_dynamics/data/spm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2372 2022-10-24 10:06:46.000000 osl-dynamics-1.2.0/osl_dynamics/data/task.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4726 2023-01-28 15:39:30.000000 osl-dynamics-1.2.0/osl_dynamics/data/tf.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:37.947267 osl-dynamics-1.2.0/osl_dynamics/files/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      868 2023-03-12 13:35:51.000000 osl-dynamics-1.2.0/osl_dynamics/files/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      443 2022-10-30 10:07:31.000000 osl-dynamics-1.2.0/osl_dynamics/files/functions.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:38.189062 osl-dynamics-1.2.0/osl_dynamics/files/mask/
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1572 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/mask/__init__.py
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-03-10 15:37:52.000000 osl-dynamics-1.2.0/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:38.258437 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-03-10 15:37:52.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-03-10 15:37:52.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       77 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-03-10 15:37:52.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:38.261746 osl-dynamics-1.2.0/osl_dynamics/files/scanner/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/ctf275_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:38.696261 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/4D148.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/4D248.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF151.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF275.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/EEG1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/EEG1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/EEG1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi160.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi256.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi32.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM1.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM1.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM10.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM10.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM11.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM11.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM14.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM14.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM15.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM15.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM16.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM17.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM17.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM20.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM20.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM22.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM22.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM23.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM23.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM24.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM24.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM25.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM25.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM3.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM3.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM7.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM7.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/elec1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/elec1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/elec1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/quickcap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/quickcap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scanner/neuromag306_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:38.698718 osl-dynamics-1.2.0/osl_dynamics/files/scene/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scene/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/files/scene/mode_scene.scene
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:38.846264 osl-dynamics-1.2.0/osl_dynamics/inference/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/inference/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7118 2023-01-28 15:39:30.000000 osl-dynamics-1.2.0/osl_dynamics/inference/callbacks.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7378 2023-03-20 14:13:14.000000 osl-dynamics-1.2.0/osl_dynamics/inference/initializers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    42087 2023-03-20 14:13:14.000000 osl-dynamics-1.2.0/osl_dynamics/inference/layers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    10529 2023-02-13 16:00:07.000000 osl-dynamics-1.2.0/osl_dynamics/inference/metrics.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    10696 2023-02-20 11:22:45.000000 osl-dynamics-1.2.0/osl_dynamics/inference/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6797 2023-02-13 15:05:52.000000 osl-dynamics-1.2.0/osl_dynamics/inference/regularizers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1647 2023-02-19 13:57:27.000000 osl-dynamics-1.2.0/osl_dynamics/inference/tf_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:39.153590 osl-dynamics-1.2.0/osl_dynamics/models/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1426 2023-02-28 15:36:39.000000 osl-dynamics-1.2.0/osl_dynamics/models/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    16776 2023-02-13 16:00:07.000000 osl-dynamics-1.2.0/osl_dynamics/models/dynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11106 2023-02-13 15:51:15.000000 osl-dynamics-1.2.0/osl_dynamics/models/dynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    40538 2023-03-18 14:07:34.000000 osl-dynamics-1.2.0/osl_dynamics/models/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15865 2023-03-03 11:25:33.000000 osl-dynamics-1.2.0/osl_dynamics/models/inf_mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    23636 2023-03-01 16:43:51.000000 osl-dynamics-1.2.0/osl_dynamics/models/mage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20236 2023-02-19 13:57:27.000000 osl-dynamics-1.2.0/osl_dynamics/models/mdynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11366 2023-02-19 13:57:27.000000 osl-dynamics-1.2.0/osl_dynamics/models/mdynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15771 2023-03-18 14:07:34.000000 osl-dynamics-1.2.0/osl_dynamics/models/mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    19191 2023-03-01 16:43:51.000000 osl-dynamics-1.2.0/osl_dynamics/models/sage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    28441 2023-03-20 14:13:14.000000 osl-dynamics-1.2.0/osl_dynamics/models/sedynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    29860 2023-03-20 14:13:15.000000 osl-dynamics-1.2.0/osl_dynamics/models/sedynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13447 2023-03-01 16:43:51.000000 osl-dynamics-1.2.0/osl_dynamics/models/state_dynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5649 2023-03-18 14:07:55.000000 osl-dynamics-1.2.0/osl_dynamics/pipeline.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:39.251805 osl-dynamics-1.2.0/osl_dynamics/simulation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      545 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/simulation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      974 2023-01-28 15:39:30.000000 osl-dynamics-1.2.0/osl_dynamics/simulation/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    30062 2023-01-28 15:39:30.000000 osl-dynamics-1.2.0/osl_dynamics/simulation/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12958 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/simulation/hsmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2710 2022-10-24 10:06:46.000000 osl-dynamics-1.2.0/osl_dynamics/simulation/mar.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    26032 2023-03-01 16:42:13.000000 osl-dynamics-1.2.0/osl_dynamics/simulation/mvn.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4809 2023-01-28 15:39:30.000000 osl-dynamics-1.2.0/osl_dynamics/simulation/sin.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5350 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/simulation/sm.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:39.357215 osl-dynamics-1.2.0/osl_dynamics/utils/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      287 2022-10-30 10:07:31.000000 osl-dynamics-1.2.0/osl_dynamics/utils/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5701 2022-10-30 10:07:31.000000 osl-dynamics-1.2.0/osl_dynamics/utils/decorators.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12402 2023-02-27 15:28:00.000000 osl-dynamics-1.2.0/osl_dynamics/utils/misc.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3597 2022-10-30 10:07:31.000000 osl-dynamics-1.2.0/osl_dynamics/utils/model.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2206 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/osl_dynamics/utils/parcellation.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    53381 2023-03-13 17:24:06.000000 osl-dynamics-1.2.0/osl_dynamics/utils/plotting.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9063 2022-10-24 10:06:46.000000 osl-dynamics-1.2.0/osl_dynamics/utils/topoplots.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-03-20 14:15:37.705992 osl-dynamics-1.2.0/osl_dynamics.egg-info/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5462 2023-03-20 14:15:37.701641 osl-dynamics-1.2.0/osl_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8051 2023-03-20 14:15:37.702589 osl-dynamics-1.2.0/osl_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2023-03-20 14:15:37.703787 osl-dynamics-1.2.0/osl_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      134 2023-03-20 14:15:37.705117 osl-dynamics-1.2.0/osl_dynamics.egg-info/requires.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2023-03-20 14:15:37.706131 osl-dynamics-1.2.0/osl_dynamics.egg-info/top_level.txt
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1031 2023-03-20 14:15:39.359402 osl-dynamics-1.2.0/setup.cfg
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      189 2022-10-17 12:20:33.000000 osl-dynamics-1.2.0/setup.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.768564 osl-dynamics-1.2.1/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4441 2023-04-14 14:57:17.768810 osl-dynamics-1.2.1/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4128 2023-03-26 09:15:19.000000 osl-dynamics-1.2.1/README.rst
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.546273 osl-dynamics-1.2.1/osl_dynamics/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      643 2023-04-14 14:48:06.000000 osl-dynamics-1.2.1/osl_dynamics/__init__.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.638726 osl-dynamics-1.2.1/osl_dynamics/analysis/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      231 2023-04-06 15:27:35.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    27101 2023-04-06 15:27:32.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/connectivity.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6323 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/fisher_kernel.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6165 2023-04-06 15:27:32.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/gmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    22485 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    18679 2023-04-06 15:27:32.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/power.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3268 2023-02-19 13:57:27.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/regression.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    44293 2023-04-14 14:48:06.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/spectral.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7487 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/static.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7333 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/statistics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5688 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/workbench.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8199 2023-03-30 19:34:59.000000 osl-dynamics-1.2.1/osl_dynamics/array_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.648697 osl-dynamics-1.2.1/osl_dynamics/config_api/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      222 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/config_api/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3837 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/config_api/pipeline.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    50431 2023-04-14 14:48:06.000000 osl-dynamics-1.2.1/osl_dynamics/config_api/wrappers.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.713324 osl-dynamics-1.2.1/osl_dynamics/data/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      185 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/data/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    36748 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/data/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/data/osl.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6757 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/data/processing.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8574 2023-03-23 11:26:21.000000 osl-dynamics-1.2.1/osl_dynamics/data/rw.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2809 2023-03-18 14:07:34.000000 osl-dynamics-1.2.1/osl_dynamics/data/spm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2447 2023-04-06 15:27:32.000000 osl-dynamics-1.2.1/osl_dynamics/data/task.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4726 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/data/tf.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.729270 osl-dynamics-1.2.1/osl_dynamics/files/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      883 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/files/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      434 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/files/functions.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.854311 osl-dynamics-1.2.1/osl_dynamics/files/mask/
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1649 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/__init__.py
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-03-10 15:37:52.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.954795 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-03-10 15:37:52.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-03-10 15:37:52.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      669 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-03-10 15:37:52.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.996108 osl-dynamics-1.2.1/osl_dynamics/files/scanner/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/ctf275_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.472410 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D148.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi160.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi256.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi32.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM1.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM1.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM10.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM10.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM11.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM11.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM14.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM14.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM15.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM15.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM16.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM17.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM17.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM20.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM20.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM22.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM22.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM23.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM23.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM24.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM24.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM25.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM25.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM3.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM3.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM7.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM7.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/quickcap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/quickcap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/neuromag306_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.481494 osl-dynamics-1.2.1/osl_dynamics/files/scene/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scene/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scene/mode_scene.scene
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.559530 osl-dynamics-1.2.1/osl_dynamics/inference/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/inference/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7118 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/inference/callbacks.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7378 2023-03-20 14:13:14.000000 osl-dynamics-1.2.1/osl_dynamics/inference/initializers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    42087 2023-03-20 14:13:14.000000 osl-dynamics-1.2.1/osl_dynamics/inference/layers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11394 2023-03-28 21:05:20.000000 osl-dynamics-1.2.1/osl_dynamics/inference/metrics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15572 2023-04-14 14:48:19.000000 osl-dynamics-1.2.1/osl_dynamics/inference/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6797 2023-02-13 15:05:52.000000 osl-dynamics-1.2.1/osl_dynamics/inference/regularizers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1647 2023-02-19 13:57:27.000000 osl-dynamics-1.2.1/osl_dynamics/inference/tf_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.658855 osl-dynamics-1.2.1/osl_dynamics/models/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1426 2023-02-28 15:36:39.000000 osl-dynamics-1.2.1/osl_dynamics/models/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    16781 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/models/dynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11105 2023-03-21 18:25:01.000000 osl-dynamics-1.2.1/osl_dynamics/models/dynemo_obs.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    41033 2023-03-21 18:26:08.000000 osl-dynamics-1.2.1/osl_dynamics/models/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15849 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/models/inf_mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    23641 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/models/mage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20241 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/models/mdynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11366 2023-02-19 13:57:27.000000 osl-dynamics-1.2.1/osl_dynamics/models/mdynemo_obs.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    16639 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/models/mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19196 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/models/sage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    28440 2023-03-21 18:25:01.000000 osl-dynamics-1.2.1/osl_dynamics/models/sedynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    29860 2023-03-20 14:13:15.000000 osl-dynamics-1.2.1/osl_dynamics/models/sedynemo_obs.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13439 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/models/state_dynemo.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.711809 osl-dynamics-1.2.1/osl_dynamics/simulation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      566 2023-03-28 21:05:20.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      974 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    30162 2023-03-28 21:05:20.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12958 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/hsmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2710 2022-10-24 10:06:46.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/mar.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    26028 2023-03-21 18:25:01.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/mvn.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4809 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/sin.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    10563 2023-03-28 21:05:20.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/sm.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.761643 osl-dynamics-1.2.1/osl_dynamics/utils/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      287 2022-10-30 10:07:31.000000 osl-dynamics-1.2.1/osl_dynamics/utils/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5701 2022-10-30 10:07:31.000000 osl-dynamics-1.2.1/osl_dynamics/utils/decorators.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13545 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/utils/misc.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6997 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/utils/model.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2206 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/utils/parcellation.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    55601 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/utils/plotting.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9063 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/utils/topoplots.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.557973 osl-dynamics-1.2.1/osl_dynamics.egg-info/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4441 2023-04-14 14:57:16.555301 osl-dynamics-1.2.1/osl_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8209 2023-04-14 14:57:16.555979 osl-dynamics-1.2.1/osl_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2023-04-14 14:57:16.556779 osl-dynamics-1.2.1/osl_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      141 2023-04-14 14:57:16.557409 osl-dynamics-1.2.1/osl_dynamics.egg-info/requires.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2023-04-14 14:57:16.558134 osl-dynamics-1.2.1/osl_dynamics.egg-info/top_level.txt
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1064 2023-04-14 14:57:17.769489 osl-dynamics-1.2.1/setup.cfg
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      189 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/setup.py
```

### Comparing `osl-dynamics-1.2.0/PKG-INFO` & `osl-dynamics-1.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osl-dynamics
-Version: 1.2.0
+Version: 1.2.1
 Summary: Models for infering dynamics in neuroimaging data
 Home-page: https://github.com/OHBA-analysis/osl-dynamics
 License: MIT
 Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 ============
@@ -99,60 +99,8 @@
 .. code-block:: shell
 
     pip install osl-dynamics
 
 Editing Source Code
 ===================
 
-Formatting and Conventions
---------------------------
-
-We use the python code formatter ``black`` to give a consistent code layout in our source files. To install:
-
-.. code-block:: shell
-
-    conda activate <env>
-    pip install black
-
-To format a source file:
-
-.. code-block:: shell
-
-    black <filename>.py
-
-Please run ``black`` on any edited files before commiting changes.
-
-Git Workflow
-------------
-
-We use git for version control. There is one ``main`` branch. To add changes:
-
-Create a feature branch for changes:
-
-.. code-block:: shell
-
-    git checkout main
-    git pull
-    git checkout -b <branch-name>
-
-Make changes to file and commit it to the branch:
-
-.. code-block:: shell
-
-    git add <file>
-    git commit -m "Short description of changes"
-
-When writing commit messages please follow the conventions `here <https://www.conventionalcommits.org/en/v1.0.0-beta.2/#specification>`_.
-
-Then either push the new branch to the remote repository:
-
-.. code-block:: shell
-
-    git push --set-upstream origin <branch-name>
-
-and create a pull request (recommended), or merge branch into ``main`` and push:
-
-.. code-block:: shell
-
-    git checkout main
-    git merge <branch-name>
-    git push
+See `here <https://github.com/OHBA-analysis/osl-dynamics/blob/main/doc/using_bmrc.rst>`_ for useful info regarding how to use the BMRC cluster and how to edit the source code.
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/__init__.py` & `osl-dynamics-1.2.1/osl_dynamics/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from pkg_resources import DistributionNotFound, get_distribution
 import logging
+from pkg_resources import DistributionNotFound, get_distribution
+
+from osl_dynamics.config_api.pipeline import run_pipeline
 
-from .pipeline import run_pipeline
 
+# Setup the version
 try:
     __version__ = get_distribution("osl-dynamics").version
 except DistributionNotFound:
     __version__ = "unknown"
 finally:
     del get_distribution, DistributionNotFound
 
-# Configure logging for package
+# Configure logging
 logging.basicConfig(
-    format="%(asctime)s %(levelname)s %(name)s: %(message)s",
+    format="%(asctime)s %(levelname)s %(name)s [%(filename)s:%(lineno)d:%(funcName)s]: %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     level=logging.INFO,
 )
-
 logger = logging.getLogger("osl-dynamics")
 logger.debug("Version %s", __version__)
-
 del logger, logging
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/analysis/connectivity.py` & `osl-dynamics-1.2.1/osl_dynamics/analysis/connectivity.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from pathlib import Path
 
 import numpy as np
 from nilearn import plotting
 from scipy import stats
-from tqdm import trange
+from tqdm.auto import trange
 
 from osl_dynamics import array_ops
 from osl_dynamics.analysis import gmm
 from osl_dynamics.analysis.spectral import get_frequency_args_range
 from osl_dynamics.utils.misc import override_dict_defaults
 from osl_dynamics.utils.parcellation import Parcellation
 
@@ -63,38 +63,32 @@
     if isinstance(data, np.ndarray):
         if data.ndim != 3:
             data = [data]
 
     # Calculate sliding window connectivity for each subject
     sliding_window_conn = []
     for i in trange(len(data), desc="Calculating connectivity"):
-        n_samples = data[i].shape[0]
-        n_channels = data[i].shape[1]
-
-        # Define indices of time points that start windows
-        time_idx = range(0, n_samples, step_size)
-        n_windows = n_samples // step_size
-
-        # Trim the data to only include complete window
-        data[i] = data[i][: n_windows * window_length]
+        ts = data[i]
+        n_samples = ts.shape[0]
+        n_channels = ts.shape[1]
+        n_windows = (n_samples - window_length - 1) // step_size + 1
 
         # Preallocate an array to hold moving average values
         swc = np.empty([n_windows, n_channels, n_channels], dtype=np.float32)
 
         # Compute connectivity matrix for each window
-        for k in range(n_windows):
-            j = time_idx[k]
-            window = data[i][j : j + window_length]
-            swc[k] = metric(window, rowvar=False)
+        for j in range(n_windows):
+            window_ts = ts[j * step_size : j * step_size + window_length]
+            swc[j] = metric(window_ts, rowvar=False)
 
         # Add to list to return
         sliding_window_conn.append(swc)
 
     if concatenate or len(sliding_window_conn) == 1:
-        sliding_window_conn = sliding_window_conn[0]
+        sliding_window_conn = np.concatenate(sliding_window_conn)
 
     return sliding_window_conn
 
 
 def covariance_from_spectra(
     frequencies,
     power_spectra,
@@ -618,19 +612,33 @@
     # Take absolute value
     if absolute_value:
         c = abs(c)
 
     # Set diagonal to nan
     c[:, :, range(n_channels), range(n_channels)] = np.nan
 
+    # Are the connectivity matrices symmetric?
+    c_is_symmetric = array_ops.check_symmetry(c, precision=1e-6)
+    m, n = np.triu_indices(n_channels, k=1)
+
     # Which edges are greater than the threshold?
     edges = np.empty([n_components, n_modes, n_channels, n_channels], dtype=bool)
     for i in range(n_components):
         for j in range(n_modes):
-            edges[i, j] = c[i, j] > np.nanpercentile(c[i, j], percentile[i, j])
+            if c_is_symmetric[i, j]:
+                # We have a symmetric connectivity matrix
+                # Threshold the upper triangle and copy to the lower triangle
+                edges[i, j, m, n] = c[i, j, m, n] > np.nanpercentile(
+                    c[i, j, m, n], percentile[i, j]
+                )
+                edges[i, j, n, m] = edges[i, j, m, n]
+            else:
+                # We have a directed connectivity matrix
+                # Threshold each entry independently
+                edges[i, j] = c[i, j] > np.nanpercentile(c[i, j], percentile[i, j])
 
     if return_edges:
         return np.squeeze(edges)
 
     # Zero the connections that are below the threshold
     conn_map[~edges] = 0
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/analysis/gmm.py` & `osl-dynamics-1.2.1/osl_dynamics/analysis/gmm.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     logit_transform=False,
     standardize=True,
     p_value=None,
     one_component_percentile=None,
     n_sigma=0,
     label_order="mean",
     sklearn_kwargs={},
+    return_statistics=False,
     show_plot=False,
     plot_filename=None,
     plot_kwargs={},
     log_message=True,
 ):
     """Fits a two component Bayesian Gaussian mixture model.
 
@@ -49,14 +50,16 @@
         Number of standard deviations of the 'off' component the mean
         of the 'on' component must be for the fit to be considered to
         have two components.
     label_order: str
         How do we order the inferred classes?
     sklearn_kwargs : dict
         Keyword arguments to pass to the sklearn class.
+    return_statistics: bool
+        Should we return statistics of the Gaussian mixture components?
     show_plot : bool
         Should we show the GMM fit to the distribution of X.
     plot_filename : str
         Filename to save a plot of the Gaussian mixture model.
     plot_kwargs : dict
         Keyword arguments to pass to plotting function.
         Only used if plot_filename is not None.
@@ -177,8 +180,19 @@
             **plot_kwargs,
         )
         ax.axvline(threshold_, color="black", linestyle="--")
         if plot_filename is not None:
             plotting.save(fig, plot_filename)
             plotting.close()
 
+    # Return Gaussian component metrics
+    if return_statistics:
+        metrics = dict(
+            threshold=threshold_,
+            data=X_[:, 0],
+            amplitudes=amplitudes,
+            means=means,
+            stddevs=stddevs,
+        )
+        return threshold, metrics
+
     return threshold
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/analysis/modes.py` & `osl-dynamics-1.2.1/osl_dynamics/analysis/modes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 
 import logging
 
 import numpy as np
 
-from osl_dynamics import array_ops
+from osl_dynamics import array_ops, inference
 
 _logger = logging.getLogger("osl-dynamics")
 
 
 def autocorrelation_functions(
     mode_covariances,
     n_embeddings,
@@ -160,66 +160,14 @@
             + f"covariances.shape={covariances.shape}, "
             + f"pca_components.shape={pca_components.shape}."
         )
 
     return pca_components @ covariances @ pca_components.T
 
 
-def partial_covariances(data, alpha):
-    """Calculate partial covariances.
-
-    Returns the multiple regression parameters estimates, pcovs, of the state
-    time courses regressed onto the data from each channel. The regression is
-    done separately for each channel. I.e. pcovs is the estimate of the
-    (n_modes, n_channels) matrix, Beta. We fit the regression Y_i = X @ Beta_i + e,
-    where:
-
-    - Y_i is (n_samples, 1) the data amplitude/envelope/power/abs time course at channel i.
-    - X is (n_samples, n_modes) matrix of the variance normalised mode time courses (i.e. alpha).
-    - Beta_i is (n_modes, 1) vector of multiple regression parameters for channel i.
-    - e is the error.
-
-    NOTE: state time courses are variance normalised so that all amplitude info goes
-    into Beta (i.e. pcovs).
-
-    Parameters
-    ----------
-    data : np.ndarray or list of np.ndarray
-        Training data for each subject.
-    alpha : np.ndarray or list of np.ndarray
-        State/mode time courses for each subject.
-
-    Returns
-    -------
-    pcovs : np.ndarray
-        Matrix of partial covariance (multiple regression parameter estimates).
-        Shape is (n_modes, n_channels).
-    """
-    if type(data) != type(alpha):
-        raise ValueError(
-            "data and alpha must be the same type: numpy arrays or lists of numpy arrays."
-        )
-    if isinstance(data, np.ndarray):
-        data = [data]
-        alpha = [alpha]
-    for i in range(len(data)):
-        if data[i].shape[0] != alpha[i].shape[0]:
-            raise ValueError("Difference number of samples in data and alpha.")
-
-    pcovs = []
-    for X, a in zip(data, alpha):
-        # Variance normalise state/mode time courses
-        a /= np.std(a, axis=0, keepdims=True)
-
-        # Do multiple regression of alpha onto data
-        pcovs.append(np.linalg.pinv(a) @ X)
-
-    return np.squeeze(pcovs)
-
-
 def state_activation(state_time_course):
     """Calculate state activations from a state time course.
 
     Given a state time course (strictly binary), calculate the beginning and
     end of each activation of each state.
 
     Parameters
@@ -641,7 +589,112 @@
     # Compute simple moving average
     for n in range(n_windows):
         j = time_idx[n]
         mov_window = data[j : j + window_length]
         mov_avg[n] = np.mean(mov_window, axis=0)
 
     return mov_avg
+
+
+def partial_covariances(data, alpha):
+    """Calculate partial covariances.
+
+    Returns the multiple regression parameters estimates, pcovs, of the state
+    time courses regressed onto the data from each channel. The regression is
+    done separately for each channel. I.e. pcovs is the estimate of the
+    (n_modes, n_channels) matrix, Beta. We fit the regression::
+
+        Y_i = X @ Beta_i + e
+
+    where:
+
+    - Y_i is (n_samples, 1) the data amplitude/envelope/power/abs time course at channel i.
+    - X is (n_samples, n_modes) matrix of the variance normalised mode time courses
+      (i.e. alpha).
+    - Beta_i is (n_modes, 1) vector of multiple regression parameters for channel i.
+    - e is the error.
+
+    NOTE: state time courses are variance normalised so that all amplitude info goes
+    into Beta (i.e. pcovs).
+
+    Parameters
+    ----------
+    data : np.ndarray or list of np.ndarray
+        Training data for each subject.
+    alpha : np.ndarray or list of np.ndarray
+        State/mode time courses for each subject.
+
+    Returns
+    -------
+    pcovs : np.ndarray
+        Matrix of partial covariance (multiple regression parameter estimates).
+        Shape is (n_modes, n_channels).
+    """
+    if type(data) != type(alpha):
+        raise ValueError(
+            "data and alpha must be the same type: numpy arrays or lists of numpy arrays."
+        )
+    if isinstance(data, np.ndarray):
+        data = [data]
+        alpha = [alpha]
+    for i in range(len(data)):
+        if data[i].shape[0] != alpha[i].shape[0]:
+            raise ValueError("Difference number of samples in data and alpha.")
+
+    pcovs = []
+    for X, a in zip(data, alpha):
+        # Variance normalise state/mode time courses
+        a /= np.std(a, axis=0, keepdims=True)
+
+        # Do multiple regression of alpha onto data
+        pcovs.append(np.linalg.pinv(a) @ X)
+
+    return np.squeeze(pcovs)
+
+
+def ae_hmm_networks(data, alpha):
+    """Calculate subject-specific AE-HMM networks.
+
+    Parameters
+    ----------
+    data : list of np.ndarray
+        Amplitude envelope data (i.e. after preparation).
+        Shape is (n_subjects, n_channels).
+    alpha : list of np.ndarray
+        Inferred state probabilities. Shape is (n_subjects, n_states).
+
+    Returns
+    -------
+    means : np.ndarray
+        Subject-specific mean activity maps. Shape is (n_subjects, n_states, n_channels).
+    aecs : np.ndarray
+        Subject-specific amplitude envelope correlation maps.
+        Shape is (n_subjects, n_states, n_channels, n_channels).
+    """
+    if type(data) != type(alpha):
+        raise ValueError(
+            "data and alpha must be the same type: numpy arrays or lists of numpy arrays."
+        )
+    if isinstance(data, np.ndarray):
+        data = [data]
+        alpha = [alpha]
+
+    # Hard classify the state probabilties
+    stc = inference.modes.argmax_time_courses(alpha)
+
+    # Number of subjects, channels and states
+    n_subjects = len(data)
+    n_channels = data[0].shape[1]
+    n_states = stc[0].shape[1]
+
+    # Calculate subject and state specific networks
+    _logger.info(f"Calculating AE networks")
+    means = np.empty([n_subjects, n_states, n_channels], dtype=np.float32)
+    aecs = np.empty([n_subjects, n_states, n_channels, n_channels], dtype=np.float32)
+    for i in range(n_subjects):
+        d = data[i][: stc[i].shape[0]]
+        for j in range(n_states):
+            x = d[stc[i][:, j] == 1]
+            means[i, j] = np.mean(x, axis=0)
+            aecs[i, j] = np.corrcoef(x, rowvar=False)
+
+    return means, aecs
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/analysis/power.py` & `osl-dynamics-1.2.1/osl_dynamics/analysis/power.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,86 @@
 import os
 import logging
 from pathlib import Path
 
 import nibabel as nib
 import numpy as np
 from nilearn import plotting
-from tqdm import trange
+from tqdm.auto import trange
 
 from osl_dynamics import array_ops, files, utils
 from osl_dynamics.analysis.spectral import get_frequency_args_range
 
 _logger = logging.getLogger("osl-dynamics")
 
 
+def sliding_window_power(
+    data, window_length, step_size=None, power_type="mean", concatenate=False
+):
+    """Calculate sliding window power.
+
+    Parameters
+    ----------
+    data : list or np.ndarray
+        Time series data. Shape must be (n_subjects, n_samples, n_channels)
+        or (n_samples, n_channels).
+    window_length : int
+        Window length in samples.
+    step_size : int
+        Number of samples to slide the window along the time series.
+        If None is passed, then a 50% overlap is used.
+    power_type : str
+        Type of power to calculate. Can be "mean" or "var".
+    concatenate : bool
+        Should we concatenate the sliding window power from each subject
+        into one big time series?
+
+    Returns
+    -------
+    sliding_window_power : list or np.ndarray
+        Time series of power vectors. Shape is (n_subjects, n_windows, n_channels)
+        or (n_windows, n_channels).
+    """
+    # Validation
+    if power_type not in ["mean", "var"]:
+        raise ValueError(f"power_type must be 'mean' or 'var', not {power_type}")
+
+    if power_type == "var":
+        metric = np.var
+    else:
+        metric = np.mean
+
+    if step_size is None:
+        step_size = window_length // 2
+
+    if isinstance(data, np.ndarray):
+        if data.ndim != 3:
+            data = [data]
+
+    # Calculate sliding window power for each subject
+    sliding_window_power = []
+    for i in trange(len(data), desc="Calculating sliding window power"):
+        ts = data[i]
+        n_samples = ts.shape[0]
+        n_channels = ts.shape[1]
+        n_windows = (n_samples - window_length - 1) // step_size + 1
+
+        swp = np.empty([n_windows, n_channels], dtype=np.float32)
+        for j in range(n_windows):
+            window_ts = ts[j * step_size : j * step_size + window_length]
+            swp[j] = metric(window_ts, axis=0)
+
+        sliding_window_power.append(swp)
+
+    if concatenate or len(sliding_window_power) == 1:
+        sliding_window_power = np.concatenate(sliding_window_power)
+
+    return sliding_window_power
+
+
 def variance_from_spectra(
     frequencies,
     power_spectra,
     components=None,
     frequency_range=None,
 ):
     """Calculates variance from power spectra.
@@ -136,23 +200,23 @@
 
 
 def power_map_grid(mask_file, parcellation_file, power_map):
     """Takes a power map and returns the power at locations on a spatial grid."""
 
     # Load the mask
     mask = nib.load(mask_file)
-    mask_grid = mask.get_data()
+    mask_grid = mask.get_fdata()
     mask_grid = mask_grid.ravel(order="F")
 
     # Get indices of non-zero elements, i.e. those which contain the brain
     non_zero_voxels = mask_grid != 0
 
     # Load the parcellation
     parcellation = nib.load(parcellation_file)
-    parcellation_grid = parcellation.get_data()
+    parcellation_grid = parcellation.get_fdata()
 
     # Make a 2D array of voxel weights for each parcel
     n_parcels = parcellation.shape[-1]
 
     # check parcellation is compatible:
     if power_map.shape[1] is not n_parcels:
         _logger.error(
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/analysis/regression.py` & `osl-dynamics-1.2.1/osl_dynamics/analysis/regression.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/analysis/spectral.py` & `osl-dynamics-1.2.1/osl_dynamics/analysis/spectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import warnings
 
 import numpy as np
 from pqdm.processes import pqdm
 from scipy.signal.windows import dpss, hann
 from sklearn.decomposition import non_negative_factorization
-from tqdm import trange
+from tqdm.auto import trange
 
 from osl_dynamics import array_ops
 from osl_dynamics.analysis import regression
 
 _logger = logging.getLogger("osl-dynamics")
 
 
@@ -646,14 +646,15 @@
     time_half_bandwidth,
     n_tapers,
     segment_length=None,
     frequency_range=None,
     return_weights=False,
     standardize=True,
     n_jobs=1,
+    keepdims=False,
 ):
     """Calculates spectra for inferred states using a multitaper.
 
     This includes power and coherence spectra.
     Follows the same procedure as the OSL function HMM-MAR/spectral/hmmspectamt.m
 
     Parameters
@@ -677,26 +678,30 @@
     return_weights : bool
         Should we return the weights for subject-specific PSDs?
         Useful for calculating the group average PSD.
     standardize : bool
         Should we standardize the data before calculating the multitaper?
     n_jobs : int
         Number of parallel jobs.
+    keepdims : bool
+        Should we enforce a (n_subject, n_states, ...) array is returned for
+        psd and coh? If False, we remove any dimensions of length 1.
 
     Returns
     -------
     frequencies : np.ndarray
-        Frequencies of the power spectra and coherences.
-        Shape is (n_freq,).
+        Frequencies of the power spectra and coherences. Shape is (n_freq,).
     power_spectra : np.ndarray
-        Power spectra for each state.
-        Shape is (n_subjects, n_states, n_channels, n_freq).
+        Power spectra for each subject and state. Shape is (n_subjects,
+        n_states, n_channels, n_freq). Any axis of length 1 is removed if
+        :code:`keepdims=False`.
     coherences : np.ndarray
-        Coherences for each state.
-        Shape is (n_subjects, n_states, n_channels, n_channels, n_freq).
+        Coherences for each state. Shape is (n_subjects, n_states, n_channels,
+        n_channels, n_freq). Any axis of length 1 is removed if
+        :code:`keepdims=False`.
     weights : np.ndarray
         Weight for each subject-specific PSD. Only returned if return_weights=True.
         Shape is (n_subjects,).
     """
 
     # Validation
     if (isinstance(data, list) != isinstance(alpha, list)) or (
@@ -835,18 +840,23 @@
         power_spectra.append(p)
         coherences.append(c)
 
     # Weights for calculating the group average PSD
     n_samples = [d.shape[0] for d in data]
     weights = np.array(n_samples) / np.sum(n_samples)
 
+    if not keepdims:
+        # Remove any axes that are of length 1
+        power_spectra = np.squeeze(power_spectra)
+        coherences = np.squeeze(coherences)
+
     if return_weights:
-        return frequencies, np.squeeze(power_spectra), np.squeeze(coherences), weights
+        return frequencies, power_spectra, coherences, weights
     else:
-        return frequencies, np.squeeze(power_spectra), np.squeeze(coherences)
+        return frequencies, power_spectra, coherences
 
 
 def single_regression_spectra(
     data,
     alpha,
     window_length,
     sampling_frequency,
@@ -927,14 +937,15 @@
     psd_only=False,
     step_size=1,
     n_sub_windows=1,
     return_weights=False,
     return_coef_int=False,
     standardize=True,
     n_jobs=1,
+    keepdims=False,
 ):
     """Calculates the PSD of each mode by regressing a time-varying PSD with alpha.
 
     Parameters
     ----------
     data : np.ndarray or list
         Data to calculate a time-varying PSD for. Shape must be (n_subjects,
@@ -964,27 +975,33 @@
     return_coef_int : bool
         Should we return the regression coefficients and intercept
         separately for the PSDs?
     standardize : bool
         Should we standardize the data before calculating the spectrogram?
     n_jobs : int
         Number of parallel jobs.
+    keepdims : bool
+        Should we enforce a (n_subject, n_states, ...) array is returned for
+        psd and coh? If False, we remove any dimensions of length 1.
 
     Returns
     -------
     f : np.ndarray
-        Frequency axis.
+        Frequency axis. Shape is (n_freq).
     psd : np.ndarray
         Mode PSDs. A numpy array with shape (n_subjects, 2, n_modes, n_channels, n_freq)
-        where the first axis is the coefficients/intercept if return_coef_int=True,
-        otherwise shape is (n_subjects, n_modes, n_channels, n_freq).
+        where axis=1 is the coefficients/intercept if return_coef_int=True, otherwise
+        shape is (n_subjects, n_modes, n_channels, n_freq). Any axis of length 1 is
+        removed if :code:`keepdims=False`.
     coh : np.ndarray
-        Mode coherences.
+        Mode coherences. Shape is (n_subjects, n_modes, n_channels, n_channels, n_freq).
+        Any axis of length 1 is removed if :code:`keepdims=False`.
     w : np.ndarray
-        Weight for each subject-specific PSD. Only returned if return_weights=True.
+        Weight for each subject-specific PSD. Shape is (n_subjects).
+        Only returned if return_weights=True.
     """
 
     # Validation
     if isinstance(data, list):
         if not isinstance(alpha, list):
             raise ValueError(
                 "data and alpha must both be lists or both be numpy arrays."
@@ -1136,18 +1153,23 @@
         p = np.sum(P[i], axis=0)  # sum coefs and intercept
         coh[i] = coherence_spectra(p, log_message=False)
 
     if not return_coef_int:
         # Sum coefficients and intercept
         psd = np.sum(psd, axis=1)
 
+    if not keepdims:
+        # Remove any axes that are of length 1
+        psd = np.squeeze(psd)
+        coh = np.squeeze(coh)
+
     if return_weights:
-        return f, np.squeeze(psd), np.squeeze(coh), weights
+        return f, psd, coh, weights
     else:
-        return f, np.squeeze(psd), np.squeeze(coh)
+        return f, psd, coh
 
 
 def spectrogram(
     data,
     window_length,
     sampling_frequency=1.0,
     frequency_range=None,
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/analysis/static.py` & `osl-dynamics-1.2.1/osl_dynamics/analysis/static.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 def power_spectra(
     data,
     window_length,
     sampling_frequency=1.0,
     frequency_range=None,
     step_size=None,
+    return_weights=False,
     standardize=True,
     calc_coh=False,
     n_jobs=1,
 ):
     """Calculate static power spectra.
 
     This function uses Welch's method to calculate the spectra.
@@ -65,14 +66,17 @@
     window_length : int
         Number of data points to use when calculating the periodogram.
     sampling_frequency : float
         Sampling frequency in Hz.
     step_size : int
         Step size for shifting the window. By default we will use half
         the window length.
+    return_weights : bool
+        Should we return the weights for subject-specific PSDs?
+        Useful for calculating the group average PSD.
     standardize : bool
         Should we standardise the data?
     calc_coh : bool
         Should we also return the coherence spectra?
     n_jobs : int
         Number of parallel jobs.
 
@@ -81,14 +85,16 @@
     f : np.ndarray
         Frequency axis. Shape is (n_freq,).
     psd : np.ndarray
         Power spectral density. Shape is (n_subjects, n_channels, n_freq).
     coh : np.ndarray
         Coherence spectra. Shape is (n_subjects, n_channels, n_channels, n_freq).
         Only returned is calc_coh=True.
+    weights : np.ndarray
+        Weight for each subject-specific PSD. Only returned if return_weights=True.
     """
 
     # Validation
     if isinstance(data, np.ndarray):
         data = [data]
 
     if frequency_range is None:
@@ -138,14 +144,18 @@
 
     # Unpack results
     psd = []
     for result in results:
         _, f, p = result
         psd.append(np.mean(p, axis=0))
 
+    # Weights for calculating the group average PSD
+    n_samples = [d.shape[0] for d in data]
+    weights = np.array(n_samples) / np.sum(n_samples)
+
     if calc_coh:
         psd = np.array(psd)
         n_subjects = psd.shape[0]
         n_channels = data[0].shape[1]
         n_freq = psd.shape[2]
 
         # Build an n_channels by n_channels cross spectra matrix
@@ -159,18 +169,24 @@
 
         # Calculate coherences
         coh = spectral.coherence_spectra(cpsd)
 
         # The PSD is the diagonal of the cross spectra matrix
         psd = cpsd[:, range(n_channels), range(n_channels)].real
 
-        return f, np.squeeze(psd), np.squeeze(coh)
+        if return_weights:
+            return f, np.squeeze(psd), np.squeeze(coh), weights
+        else:
+            return f, np.squeeze(psd), np.squeeze(coh)
 
     else:
-        return f, np.squeeze(psd)
+        if return_weights:
+            return f, np.squeeze(psd), weights
+        else:
+            return f, np.squeeze(psd)
 
 
 def multitaper_spectra(
     data,
     sampling_frequency,
     time_half_bandwidth,
     n_tapers,
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/analysis/workbench.py` & `osl-dynamics-1.2.1/osl_dynamics/analysis/workbench.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import pathlib
 import re
 import subprocess
 import warnings
 
 import nibabel as nib
-from tqdm import trange
+from tqdm.auto import trange
 
 from osl_dynamics import files
 
 surfs = {
     0: [files.mask.surf_left, files.mask.surf_right],
     1: [files.mask.surf_left_inf, files.mask.surf_right_inf],
     2: [files.mask.surf_left_vinf, files.mask.surf_right_vinf],
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/array_ops.py` & `osl-dynamics-1.2.1/osl_dynamics/array_ops.py`

 * *Files 11% similar despite different names*

```diff
@@ -228,7 +228,40 @@
                 array = array[np.newaxis, ...]
 
     # Check no other dimensionality has been passed
     if array.ndim != correct_dimensionality:
         raise ValueError(error_message)
 
     return array
+
+
+def check_symmetry(mat, precision=1e-6):
+    """Checks if one or more matrices are symmetric.
+
+    Parameters
+    ----------
+    mat : np.ndarray or list of np.ndarray
+        Matrices to be checked. Shape of a matrix should be (..., N, N).
+    precision : float
+        Precision for comparing values. Corresponds to an absolute tolerance parameter.
+        Default is 1e-6.
+
+    Returns
+    -------
+    symmetry : np.ndarray
+        Array indicating whether matrices are symmetric.
+    """
+    mat = np.array(mat)
+    if mat.ndim < 2:
+        raise ValueError("Input matrix must be an array with shape (..., N, N).")
+    transpose_axes = np.concatenate((np.arange(mat.ndim - 2), [-1, -2]))
+    symmetry = np.all(
+        np.isclose(
+            mat,
+            np.transpose(mat, axes=transpose_axes),
+            rtol=0,
+            atol=precision,
+            equal_nan=True,
+        ),
+        axis=(-1, -2),
+    )
+    return symmetry
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/data/base.py` & `osl-dynamics-1.2.1/osl_dynamics/data/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from functools import partial
 from os import path
 from shutil import rmtree
 
 import numpy as np
 from pqdm.threads import pqdm
 from scipy import signal
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from osl_dynamics.data import processing, rw, tf
 from osl_dynamics.utils import misc
 
 _logger = logging.getLogger("osl-dynamics")
 
 
@@ -56,22 +56,36 @@
         If a fif file is passed we load the data using the MNE object's get_data()
         method. If the fif file contains a mne.Raw object, we pass this argument to
         the get_data() method. This argument is optional. By default
         reject_by_annotation=None retrieves all time points. Use
         reject_by_annotation="omit" to remove segments marked as bad.
     sampling_frequency : float
         Sampling frequency of the data in Hz. This argument is optional.
+    mask_file : str
+        Path to mask file used to source reconstruct the data. This argument is
+        optional.
+    parcellation_file : str
+        Path to parcellation file used to source reconstruct the data. This argument
+        is optional.
     store_dir : str
         We don't read all the data into memory. Instead we create store them on
         disk and create memmaps (unless load_memmaps=False is passed).
         This is the directory to save memmaps to. Default is ./tmp.
         This argument is optional.
     n_embeddings : int
-        Number of embeddings. Can be passed if data has already been prepared.
-        This argument is optional.
+        Number of time-delay embeddings that have already been appleid to the data.
+        This argument is optional. It is useful to pass this argument if the data has
+        already been prepared.
+    n_window : int
+        Length of sliding window that has already been applied to the data. This
+        argument is optional. It is useful to pass this argument if the data has
+        already been prepared.
+    amplitude_envelope : bool
+        Is the data we're loading amplitude envelope data? This argument is optional.
+        It is useful to pass this argument if the data has already been prepared.
     time_axis_first : bool
         Is the input data of shape (n_samples, n_channels)? Default is True.
         If your data is in format (n_channels, n_samples), use
         time_axis_first=False. This argument is optional.
     load_memmaps: bool
         Should we load the data as memory maps (memmaps)? If False, we will load data
         into memory rather than storing it on disk. By default we will keep the data
@@ -84,26 +98,34 @@
     def __init__(
         self,
         inputs,
         data_field="X",
         picks=None,
         reject_by_annotation=None,
         sampling_frequency=None,
+        mask_file=None,
+        parcellation_file=None,
         store_dir="tmp",
         n_embeddings=None,
+        n_window=None,
+        amplitude_envelope=None,
         time_axis_first=True,
         load_memmaps=True,
         n_jobs=1,
     ):
         self._identifier = id(self)
         self.data_field = data_field
         self.picks = picks
         self.reject_by_annotation = reject_by_annotation
         self.sampling_frequency = sampling_frequency
+        self.mask_file = mask_file
+        self.parcellation_file = parcellation_file
         self.n_embeddings = n_embeddings
+        self.n_window = n_window
+        self.amplitude_envelope = amplitude_envelope
         self.time_axis_first = time_axis_first
         self.load_memmaps = load_memmaps
         self.n_jobs = n_jobs
         self.prepared = False
         self.prepared_data_filenames = []
 
         # Validate inputs
@@ -458,14 +480,17 @@
         ) and self.sampling_frequency is None:
             raise ValueError(
                 "Data.sampling_frequency must be set if we are filtering the data. "
                 + "Use Data.set_sampling_frequency() or pass "
                 + "Data(..., sampling_frequency=...) when creating the Data object."
             )
 
+        if n_window % 2 == 0:
+            raise ValueError("n_window must be an odd number.")
+
         # Save settings
         self.amplitude_envelope = True
         self.low_freq = low_freq
         self.high_freq = high_freq
         self.n_window = n_window
         self.n_embeddings = 1
         self.n_te_channels = self.n_raw_data_channels
@@ -689,59 +714,67 @@
 
         self.prepared_data_memmaps = []
 
     def trim_time_series(
         self,
         sequence_length=None,
         n_embeddings=1,
+        n_window=1,
         prepared=True,
         concatenate=False,
     ):
         """Trims the data time series.
 
         Removes the data points that are lost when the data is prepared,
         i.e. due to time embedding and separating into sequences, but does not
         perform time embedding or batching into sequences on the time series.
 
         Parameters
         ----------
         sequence_length : int
             Length of the segement of data to feed into the model.
         n_embeddings : int
-            Number of data points to embed the data.
+            Number of data points used to embed the data.
+        n_window : int
+            Number of data points the sliding window applied to the data.
         prepared : bool
             Should we return the prepared data? If not we return the raw data.
         concatenate : bool
             Should we concatenate the data for each subject?
 
         Returns
         -------
         list of np.ndarray
             Trimed time series for each subject.
         """
-        if self.n_embeddings is None:
+        if self.n_embeddings is None and self.n_window is None:
             # Data has not been prepared so we can't trim the prepared data
             prepared = False
 
         if not prepared:
-            # We're trimming the raw data, how many time embedding data
-            # points do we need to remove?
-            n_embeddings = self.n_embeddings or n_embeddings
+            # We're trimming the raw data, how many data points do we
+            # need to remove due to time embedding or moving average?
+            if self.amplitude_envelope:
+                n_remove = self.n_window or n_window
+            else:
+                n_remove = self.n_embeddings or n_embeddings
+        else:
+            n_remove = 1
 
         # What data should we trim?
         if prepared:
             memmaps = self.subjects
         else:
             memmaps = self.raw_data_memmaps
 
         trimmed_time_series = []
         for memmap in memmaps:
             # Remove data points lost to time embedding
-            if n_embeddings != 1:
-                memmap = memmap[n_embeddings // 2 : -(n_embeddings // 2)]
+            if n_remove != 1:
+                memmap = memmap[n_remove // 2 : -(n_remove // 2)]
 
             # Remove data points lost to separating into sequences
             if sequence_length is not None:
                 n_sequences = memmap.shape[0] // sequence_length
                 memmap = memmap[: n_sequences * sequence_length]
 
             trimmed_time_series.append(memmap)
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/data/osl.py` & `osl-dynamics-1.2.1/osl_dynamics/data/osl.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/data/processing.py` & `osl-dynamics-1.2.1/osl_dynamics/data/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Functions to process data.
 
 """
 
 import numpy as np
 from scipy import signal
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from osl_dynamics import array_ops
 from osl_dynamics.data.spm import SPM
 
 
 def standardize(
     time_series,
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/data/rw.py` & `osl-dynamics-1.2.1/osl_dynamics/data/rw.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/data/spm.py` & `osl-dynamics-1.2.1/osl_dynamics/data/spm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/data/task.py` & `osl-dynamics-1.2.1/osl_dynamics/data/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 import numpy as np
 
 
 def epoch(
     data,
     time_index,
-    pre=125,
-    post=1000,
-    pad=True,
+    pre,
+    post,
+    pad=False,
 ):
     """Transform [time x channel] data to [time x channel x epoch] data.
 
     Given a series of triggers given by `time_index`, spit a continuous dataset into
     epochs. `time_index` should be a sequence of integers representing the triggers
     of the epochs. `pre` and `post` specify the window around each trigger event.
 
@@ -32,27 +32,29 @@
         Pad with NaNs so that initial epochs will always been included.
 
     Returns
     -------
     epoched : numpy.ndarray
         A [time x channels x epochs] dataset.
     """
-    # If there are not enough time points before the first trigger, discard it.
     if pad:
+        # Pad before and after the data with zeros
         data = np.pad(data, ((pre, post), (0, 0)), constant_values=np.nan)
         time_index = time_index + pre
-    elif time_index[0] - pre < 0:
-        time_index = time_index[1:]
+    else:
+        # Only keep epochs we have all time points for
+        keep = np.logical_and(time_index - pre > 0, time_index + post < data.shape[0])
+        time_index = time_index[keep]
 
     starts, stops = time_index - pre, time_index + post
     epoched = np.array([data[start:stop] for start, stop in zip(starts, stops)])
     return epoched
 
 
-def epoch_mean(data, time_index, pre=125, post=1000, pad=True):
+def epoch_mean(data, time_index, pre, post, pad=False):
     """Get the mean over epochs of a [time x channels] dataset.
 
     Calls `epoch_mean`, and takes a mean over epochs, returning data with dimensions
     [time x channels] in which the time is the length of the epoch window.
 
     Parameters
     ----------
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/data/tf.py` & `osl-dynamics-1.2.1/osl_dynamics/data/tf.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/__init__.py` & `osl-dynamics-1.2.1/osl_dynamics/files/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-"""Useful files kept in the osl-dynamics package.
+"""Files included within osl-dynamics.
 
 This includes parcellation/mask files and scanner layouts.
 
 Available parcellations:
 
 - fMRI_parcellation_ds8mm.nii.gz
-- fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
+- fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz (the 'Giles parcellation')
 - fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
 - fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
 - fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
 - fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
 - aal_cortical_merged_8mm_stacked.nii.gz
 - Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
 - Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
 - giles_39_binary.nii.gz
 
 Available masks:
 
 - MNI152_T1_8mm_brain.nii.gz
 - ft_8mm_brain_mask.nii.gz
-
 """
 
 from osl_dynamics.files import mask, parcellation, scanner, scene
 from osl_dynamics.files.functions import *
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/mask/__init__.py` & `osl-dynamics-1.2.1/osl_dynamics/files/mask/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Mask files.
+
+- MNI152_T1_8mm_brain.nii.gz
+- ft_8mm_brain_mask.nii.gz
+"""
+
 from pathlib import Path
 
 import nibabel as nib
 import numpy as np
 
 surf_right = str(
     Path(__file__).parent / "ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii"
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/parcellation/giles_39_binary.nii.gz` & `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/giles_39_binary.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/ctf275_channel_names.npy` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/ctf275_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/4D148.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D148.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/4D248.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/4D248_helmet.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/4D248_helmet.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF151.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF275.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/EEG1005.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/EEG1010.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/EEG1020.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi128.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi16.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi160.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi256.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi32.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/biosemi64.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM1.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM1.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM1.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM1.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM10.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM10.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM10.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM10.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM11.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM11.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM11.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM11.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM14.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM14.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM14.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM14.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM15.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM15.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM15.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM15.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM16.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM16.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM16.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM17.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM17.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM17.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM17.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM20.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM20.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM20.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM20.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM22.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM22.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM22.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM22.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM23.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM23.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM23.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM23.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM24.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM24.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM24.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM24.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM25.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM25.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM25.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM25.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM3.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM3.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM3.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM3.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM7.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM7.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/easycapM7.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM7.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/elec1005.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/elec1010.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/elec1020.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag122planar.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag122planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306all.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306mag.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306planar.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/quickcap64.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/quickcap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/quickcap64.outline` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/quickcap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440all.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scanner/neuromag306_channel_names.npy` & `osl-dynamics-1.2.1/osl_dynamics/files/scanner/neuromag306_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/files/scene/mode_scene.scene` & `osl-dynamics-1.2.1/osl_dynamics/files/scene/mode_scene.scene`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/inference/callbacks.py` & `osl-dynamics-1.2.1/osl_dynamics/inference/callbacks.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/inference/initializers.py` & `osl-dynamics-1.2.1/osl_dynamics/inference/initializers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/inference/layers.py` & `osl-dynamics-1.2.1/osl_dynamics/inference/layers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/inference/metrics.py` & `osl-dynamics-1.2.1/osl_dynamics/inference/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Metrics for evaluating model performance.
 
 """
 
 import numpy as np
 from scipy.linalg import eigvalsh
 from sklearn.metrics import confusion_matrix as sklearn_confusion_matrix
-from tqdm import trange
+from tqdm.auto import trange
 
 
 def alpha_correlation(alpha_1, alpha_2):
     """Calculates the correlation between modes of two alpha time series.
 
     Parameters
     ----------
@@ -323,7 +323,37 @@
         cc = nom / np.sqrt(np.dot(denom1, denom2))
         C[index[0], index[1]] = cc
 
     if remove_diagonal:
         C -= np.eye(n_matrices)
 
     return C
+
+
+def pairwise_l2_distance(arrays, batch_dims=0):
+    """Calculate the pairwise L2 distance
+    along the first axis after the batch dims.
+
+    Parameters
+    ----------
+    arrays : np.ndarray
+        Set of arrays. Shape is (..., n_arrays, ...).
+    batch_dims : int
+        Number of batch dimensions.
+
+    Returns
+    -------
+    pairwise_distance : np.ndarray
+        Matrix of pairwise L2 distance. Shape is (..., n_arrays, n_arrays)
+    """
+    if batch_dims > arrays.ndim - 1:
+        raise ValueError("batch_dims must be less than arrays.ndim - 1")
+    pairwise_axis = batch_dims
+    return np.sqrt(
+        np.sum(
+            np.square(
+                np.expand_dims(arrays, pairwise_axis)
+                - np.expand_dims(arrays, pairwise_axis + 1)
+            ),
+            axis=tuple(range(pairwise_axis + 2, arrays.ndim + 1)),
+        )
+    )
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/inference/regularizers.py` & `osl-dynamics-1.2.1/osl_dynamics/inference/regularizers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/inference/tf_ops.py` & `osl-dynamics-1.2.1/osl_dynamics/inference/tf_ops.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/__init__.py` & `osl-dynamics-1.2.1/osl_dynamics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/dynemo.py` & `osl-dynamics-1.2.1/osl_dynamics/models/dynemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dataclasses import dataclass
 from typing import Literal
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.keras import layers
-from tqdm import trange
+from tqdm.auto import trange
 
 from osl_dynamics.inference.layers import (
     CovarianceMatricesLayer,
     DiagonalMatricesLayer,
     InferenceRNNLayer,
     KLDivergenceLayer,
     KLLossLayer,
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/dynemo_obs.py` & `osl-dynamics-1.2.1/osl_dynamics/models/dynemo_obs.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,14 @@
                 training_dataset,
                 self.config.covariances_epsilon,
                 self.config.diagonal_covariances,
             )
 
 
 def _model_structure(config):
-
     # Layers for inputs
     data = layers.Input(shape=(config.sequence_length, config.n_channels), name="data")
     alpha = layers.Input(shape=(config.sequence_length, config.n_modes), name="alpha")
 
     # Observation model:
     # - We use a multivariate normal with a mean vector and covariance matrix for
     #   each mode as the observation model.
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/hmm.py` & `osl-dynamics-1.2.1/osl_dynamics/models/hmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 from dataclasses import dataclass
 from pathlib import Path
 
 import numba
 import numpy as np
 import tensorflow as tf
 import tensorflow_probability as tfp
-from scipy.special import xlogy, logsumexp
 from numba.core.errors import NumbaWarning
+from scipy.special import logsumexp, xlogy
 from tensorflow.keras import backend, layers, utils
+from tqdm.auto import trange
 
 import osl_dynamics.data.tf as dtf
 from osl_dynamics.inference import initializers
 from osl_dynamics.inference.layers import (
     CategoricalLogLikelihoodLossLayer,
     CovarianceMatricesLayer,
     DiagonalMatricesLayer,
@@ -146,15 +147,15 @@
         """Builds a keras model."""
         self.model = _model_structure(self.config)
 
         self.rho = 1
         self.set_trans_prob(self.config.initial_trans_prob)
         self.set_state_probs_t0(self.config.state_probs_t0)
 
-    def fit(self, dataset, epochs=None, **kwargs):
+    def fit(self, dataset, epochs=None, use_tqdm=False, **kwargs):
         """Fit model to a dataset.
 
         Iterates between:
 
         - Baum-Welch updates of latent variable time courses and transition
           probability matrix.
         - TensorFlow updates of observation model parameters.
@@ -176,19 +177,27 @@
         """
         if epochs is None:
             epochs = self.config.n_epochs
 
         # Make a TensorFlow Dataset
         dataset = self.make_dataset(dataset, shuffle=True, concatenate=True)
 
+        # Training curves
         history = {"loss": [], "rho": [], "lr": []}
-        for n in range(epochs):
-            # Setup a progress bar
-            print("Epoch {}/{}".format(n + 1, epochs))
-            pb_i = utils.Progbar(len(dataset))
+
+        # Loop through epochs
+        if use_tqdm:
+            _range = trange(epochs)
+        else:
+            _range = range(epochs)
+        for n in _range:
+            # Setup a progress bar for this epoch
+            if not use_tqdm:
+                print("Epoch {}/{}".format(n + 1, epochs))
+                pb_i = utils.Progbar(len(dataset))
 
             # Update rho
             self._update_rho(n)
 
             # Set learning rate for the observation model
             lr = self.config.learning_rate * np.exp(
                 -self.config.observation_update_decay * n
@@ -211,25 +220,34 @@
                 # -> (batch_size, sequence_length, n_states)
                 gamma = gamma.reshape(x.shape[0], x.shape[1], -1)
 
                 # Update observation model
                 x_and_gamma = np.concatenate([x, gamma], axis=2)
                 h = self.model.fit(x_and_gamma, epochs=1, verbose=0, **kwargs)
 
+                # Get new loss
                 l = h.history["loss"][0]
                 if np.isnan(l):
                     _logger.error("Training failed!")
                     return
                 loss.append(l)
-                pb_i.add(1, values=[("rho", self.rho), ("lr", lr), ("loss", l)])
+
+                # Update progress bar
+                if use_tqdm:
+                    _range.set_postfix(rho=self.rho, lr=lr, loss=l)
+                else:
+                    pb_i.add(1, values=[("rho", self.rho), ("lr", lr), ("loss", l)])
 
             history["loss"].append(np.mean(loss))
             history["rho"].append(self.rho)
             history["lr"].append(lr)
 
+        if use_tqdm:
+            _range.close()
+
         return history
 
     def random_subset_initialization(
         self, training_data, n_epochs, n_init, take, **kwargs
     ):
         """Random subset initialization.
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/inf_mod_base.py` & `osl-dynamics-1.2.1/osl_dynamics/models/inf_mod_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         # Pick the initialization with the lowest free energy
         best_loss = np.Inf
         for n in range(n_init):
             _logger.info(f"Initialization {n}")
             self.reset()
             training_data_subset = training_data.shuffle(100000).take(n_batches)
             history = self.fit(training_data_subset, epochs=n_epochs, **kwargs)
-            loss = history.history["loss"][-1]
+            loss = history["loss"][-1]
             if loss < best_loss:
                 best_initialization = n
                 best_loss = loss
                 best_history = history
                 best_weights = self.get_weights()
 
         _logger.info(f"Using initialization {best_initialization}")
@@ -261,15 +261,15 @@
 
             # Get the dataset for this subject
             subject_dataset = training_data[subject]
 
             # Reset the model weights and train
             self.reset()
             history = self.fit(subject_dataset, epochs=n_epochs, **kwargs)
-            loss = history.history["loss"][-1]
+            loss = history["loss"][-1]
             losses.append(loss)
             _logger.info(f"Subject {subject} loss: {loss}")
 
             # Record the loss of this subject's data
             if loss < best_loss:
                 best_loss = loss
                 subject_chosen = subject
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/mage.py` & `osl-dynamics-1.2.1/osl_dynamics/models/mage.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import time
 from dataclasses import dataclass
 from typing import Literal
 
 import numpy as np
 from tensorflow.keras import layers, models, optimizers, utils
-from tqdm import trange
+from tqdm.auto import trange
 
 from osl_dynamics.inference.layers import (
     AdversarialLogLikelihoodLossLayer,
     ConcatVectorsMatricesLayer,
     CorrelationMatricesLayer,
     DiagonalMatricesLayer,
     InferenceRNNLayer,
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/mdynemo.py` & `osl-dynamics-1.2.1/osl_dynamics/models/mdynemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 from dataclasses import dataclass
 from typing import Literal
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.keras import layers
-from tqdm import trange
+from tqdm.auto import trange
 
 from osl_dynamics.inference.layers import (
     ConcatenateLayer,
     CorrelationMatricesLayer,
     DiagonalMatricesLayer,
     InferenceRNNLayer,
     KLDivergenceLayer,
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/mdynemo_obs.py` & `osl-dynamics-1.2.1/osl_dynamics/models/mdynemo_obs.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/mod_base.py` & `osl-dynamics-1.2.1/osl_dynamics/models/mod_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,16 @@
             args,
             kwargs,
             append=True,
         )
         if use_tqdm:
             args, kwargs = replace_argument(self.model.fit, "verbose", 0, args, kwargs)
 
-        return self.model.fit(*args, **kwargs)
+        history = self.model.fit(*args, **kwargs)
+        return history.history
 
     def load_weights(self, filepath):
         """Load weights of the model from a file.
 
         Parameters
         ----------
         filepath : str
@@ -314,30 +315,48 @@
             Training data time series.
         """
         return training_data.trim_time_series(
             self.config.sequence_length, prepared=prepared, concatenate=concatenate
         )
 
     def summary_string(self):
+        """Return a summary of the model as a string.
+
+        This is a modified version of the keras.Model.summary() method which
+        makes the output easier to parse.
+        """
         stringio = StringIO()
         self.model.summary(
             print_fn=lambda s: stringio.write(s + "\n"), line_length=1000
         )
         return stringio.getvalue()
 
     def summary_table(self, renderer):
+        """Return a summary of the model as a table (HTML or LaTeX).
+
+        Parameters
+        ----------
+        renderer : str
+            Renderer to use. Either "html" or "latex".
+
+        Returns
+        -------
+        table : str
+            Summary of the model as a table.
+        """
+
         summary = self.summary_string()
 
         renderers = {"html": HTMLTable, "latex": LatexTable}
 
         # Extract information
         headers = [h for h in re.split(r"\s{2,}", summary.splitlines()[2]) if h != ""]
         columns = [summary.splitlines()[2].find(title) for title in headers] + [-1]
 
-        # Create HTML table.
+        # Create HTML table
         table = renderers.get(renderer, HTMLTable)(headers)
         for line in summary.splitlines()[4:]:
             if (
                 line.startswith("_")
                 or line.startswith("=")
                 or line.startswith('Model: "')
             ):
@@ -353,20 +372,27 @@
                 table.append_last(elements[3])
             else:
                 table += elements
 
         return table.output()
 
     def html_summary(self):
+        """Return a summary of the model as an HTML table."""
         return self.summary_table(renderer="html")
 
     def latex_summary(self):
+        """Return a summary of the model as a LaTeX table."""
         return self.summary_table(renderer="latex")
 
     def _repr_html_(self):
+        """Display the model as an HTML table in Jupyter notebooks.
+
+        This is called when you type the variable name of the model in a
+        Jupyter notebook. It is unlikely that you will need to call this.
+        """
         return self.html_summary()
 
     def save_config(self, dirname):
         """Saves config object as a .yml file.
 
         Parameters
         ----------
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/sage.py` & `osl-dynamics-1.2.1/osl_dynamics/models/sage.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import time
 from dataclasses import dataclass
 from typing import Literal
 
 import numpy as np
 from tensorflow.keras import layers, models, optimizers, utils
-from tqdm import trange
+from tqdm.auto import trange
 
 from osl_dynamics.inference.layers import (
     AdversarialLogLikelihoodLossLayer,
     ConcatVectorsMatricesLayer,
     CovarianceMatricesLayer,
     InferenceRNNLayer,
     MixMatricesLayer,
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/sedynemo.py` & `osl-dynamics-1.2.1/osl_dynamics/models/sedynemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,14 @@
         """random subject initialisation not compatible with SE-DyNeMo."""
         raise AttributeError(
             " 'Model' object has no attribute 'random_subject_initialization'."
         )
 
 
 def _model_structure(config):
-
     # Layers for inputs
     data = layers.Input(shape=(config.sequence_length, config.n_channels), name="data")
     subj_id = layers.Input(shape=(config.sequence_length,), name="subj_id")
 
     # Inference RNN:
     # Layer definitions
     inference_input_dropout_layer = layers.Dropout(
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/sedynemo_obs.py` & `osl-dynamics-1.2.1/osl_dynamics/models/sedynemo_obs.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/models/state_dynemo.py` & `osl-dynamics-1.2.1/osl_dynamics/models/state_dynemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         for n in range(n_init):
             _logger.info(f"Initialization {n}")
             self.reset()
             self.set_random_state_time_course_initialization(training_data)
             training_dataset.shuffle(100000)
             training_data_subset = training_dataset.take(n_batches)
             history = self.fit(training_data_subset, epochs=n_epochs, **kwargs)
-            loss = history.history["loss"][-1]
+            loss = history["loss"][-1]
             if loss < best_loss:
                 best_initialization = n
                 best_loss = loss
                 best_history = history
                 best_weights = self.get_weights()
 
         if best_loss == np.Inf:
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/simulation/__init__.py` & `osl-dynamics-1.2.1/osl_dynamics/simulation/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,8 +12,8 @@
     HMM_MVN,
     MDyn_HMM_MVN,
     HierarchicalHMM_MVN,
     HMM_Sine,
     MSubj_HMM_MVN,
 )
 from osl_dynamics.simulation.hsmm import HSMM, HSMM_MVN, MixedHSMM_MVN
-from osl_dynamics.simulation.sm import MixedSine, MixedSine_MVN
+from osl_dynamics.simulation.sm import MixedSine, MixedSine_MVN, MSubj_MixedSine_MVN
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/simulation/base.py` & `osl-dynamics-1.2.1/osl_dynamics/simulation/base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/simulation/hmm.py` & `osl-dynamics-1.2.1/osl_dynamics/simulation/hmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     def __init__(
         self,
         trans_prob,
         stay_prob=None,
         n_states=None,
         random_seed=None,
     ):
-
         if isinstance(trans_prob, list):
             trans_prob = np.ndarray(trans_prob)
 
         if isinstance(trans_prob, np.ndarray):
             # Don't need to generate the transition probability matrix
 
             if trans_prob.ndim != 2:
@@ -462,14 +461,16 @@
         Number of channels.
     n_covariances_act : int
         Number of iterations to add activations to covariance matrices.
     n_subjects : int
         Number of subjects.
     n_groups : int
         Number of groups of subjects when subject means or covariances are 'random'.
+    between_group_scale : float
+        Scale of variability between subject observation parameters.
     stay_prob : float
         Used to generate the transition probability matrix is trans_prob is a str.
     subject_tc_std : float
         Standard deviation when generating subject specific stay probability.
     observation_error : float
         Standard deviation of the error added to the generated data.
     random_seed : int
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/simulation/hsmm.py` & `osl-dynamics-1.2.1/osl_dynamics/simulation/hsmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/simulation/mar.py` & `osl-dynamics-1.2.1/osl_dynamics/simulation/mar.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/simulation/mvn.py` & `osl-dynamics-1.2.1/osl_dynamics/simulation/mvn.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,14 @@
         data = np.zeros((n_samples, self.n_channels))
         self.instantaneous_covs = np.zeros(
             [n_samples, self.n_channels, self.n_channels]
         )
 
         # Loop through all unique combinations of modes
         for alpha in np.unique(state_time_course, axis=0):
-
             # Mean and covariance for this combination of modes
             mu = np.sum(self.means * alpha[:, np.newaxis], axis=0)
             sigma = np.sum(self.covariances * alpha[:, np.newaxis, np.newaxis], axis=0)
 
             self.instantaneous_covs[np.all(state_time_course == alpha, axis=1)] = sigma
 
             # Generate data for the time points that this combination of modes is
@@ -240,15 +239,14 @@
         data = np.zeros([n_samples, self.n_channels])
         self.instantaneous_covs = np.zeros(
             [n_samples, self.n_channels, self.n_channels]
         )
 
         # Loop through all unique combinations of states
         for time_courses in np.unique(state_time_courses, axis=0):
-
             # Extract the different time courses
             alpha = time_courses[:, 0]
             gamma = time_courses[:, 1]
 
             # Mean, standard deviation, FC for this combination of time courses
             mu = np.sum(self.means * alpha[:, np.newaxis], axis=0)
             G = np.diag(np.sum(self.stds * alpha[:, np.newaxis], axis=0))
@@ -327,15 +325,14 @@
         n_mode_embedding_dim=None,
         subject_embedding_scale=None,
         n_groups=None,
         between_group_scale=None,
         observation_error=0.0,
         random_seed=None,
     ):
-
         self._rng = np.random.default_rng(random_seed)
         self.n_covariances_act = n_covariances_act
         self.observation_error = observation_error
         self.instantaneous_covs = None
         self.n_subject_embedding_dim = n_subject_embedding_dim
         self.n_mode_embedding_dim = n_mode_embedding_dim
         self.subject_embedding_scale = subject_embedding_scale
@@ -621,15 +618,14 @@
 
         # Initialise array to hold data
         data = np.zeros((n_samples, self.n_channels))
         instantaneous_covs = np.zeros([n_samples, self.n_channels, self.n_channels])
 
         # Loop through all unique combinations of modes
         for alpha in np.unique(mode_time_course, axis=0):
-
             # Mean and covariance for this combination of modes
             mu = np.sum(self.subject_means[subject] * alpha[:, None], axis=0)
             sigma = np.sum(
                 self.subject_covariances[subject] * alpha[:, None, None], axis=0
             )
 
             instantaneous_covs[np.all(mode_time_course == alpha, axis=1)] = sigma
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/simulation/sin.py` & `osl-dynamics-1.2.1/osl_dynamics/simulation/sin.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/utils/decorators.py` & `osl-dynamics-1.2.1/osl_dynamics/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.0/osl_dynamics/utils/misc.py` & `osl-dynamics-1.2.1/osl_dynamics/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Miscellaneous utility classes and functions.
 
 """
 
 import inspect
 import logging
+import pickle
 import sys
 from copy import copy
 from pathlib import Path
 
 import numpy as np
 import yaml
 from yaml.constructor import ConstructorError
@@ -446,7 +447,58 @@
             raise ConstructorError(
                 "while constructing a Python object",
                 mark,
                 "cannot find %r in the module %r" % (object_name, module.__name__),
                 mark,
             )
         return getattr(module, object_name)
+
+
+def save(filename, array):
+    """Save a file.
+
+    Parameters
+    ----------
+    filename : str
+        Path to file to save to. Must be '.npy' or '.pkl'.
+    array : np.ndarray or list
+        Array to save.
+    """
+    # Validation
+    ext = Path(filename).suffix
+    if ext not in [".npy", ".pkl"]:
+        raise ValueError(f"filename extension must be .npy or .pkl.")
+
+    # Save
+    _logger.info(f"Saving {filename}")
+    if ext == ".pkl":
+        pickle.dump(array, open(filename, "wb"))
+    else:
+        np.save(filename, array)
+
+
+def load(filename):
+    """Load a file.
+
+    Parameters
+    ----------
+    filename : str
+        Path to file to load. Must be '.npy' or '.pkl'.
+
+    Returns
+    -------
+    array : np.ndarray or list
+        Array loaded from the file.
+    """
+    # Validation
+    ext = Path(filename).suffix
+    if ext not in [".npy", ".pkl"]:
+        raise ValueError(f"filename extension must be .npy or .pkl.")
+
+    # Load
+    _logger.info(f"Loading {filename}")
+    if ext == ".pkl":
+        array = pickle.load(open(filename, "rb"))
+    else:
+        array = np.load(filename)
+
+    return array
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/utils/parcellation.py` & `osl-dynamics-1.2.1/osl_dynamics/utils/parcellation.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Parcellation related classes and functions.
 
 """
 
-
 import nibabel as nib
 import numpy as np
 from pathlib import Path
 from nilearn.plotting import plot_markers
+
 from osl_dynamics import files
 
 
 class Parcellation:
     """Class for reading parcellation files.
 
     Parameters
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/utils/plotting.py` & `osl-dynamics-1.2.1/osl_dynamics/utils/plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,32 @@
 """Plotting functions.
 
 """
 
 import logging
 from itertools import zip_longest
 
+import numpy as np
+import pandas as pd
+import seaborn as sns
 import matplotlib
 import matplotlib.pyplot as plt
-import numpy as np
 from matplotlib import patches
 from matplotlib.path import Path
 from mpl_toolkits.axes_grid1.axes_divider import make_axes_locatable
 from nilearn.plotting import plot_markers
 
 from osl_dynamics.array_ops import get_one_hot
 from osl_dynamics.utils.misc import override_dict_defaults
 from osl_dynamics.utils.topoplots import Topology
 from osl_dynamics.utils.parcellation import Parcellation
 
 
 _logger = logging.getLogger("osl-dynamics")
 
-QUAL_CMAPS = [
-    "Pastel1",
-    "Pastel2",
-    "Paired",
-    "Accent",
-    "Dark2",
-    "Set1",
-    "Set2",
-    "Set3",
-    "tab10",
-    "tab20",
-    "tab20b",
-    "tab20c",
-]
-
 
 def set_style(params):
     """Sets matplotlib's style.
 
     Wrapper for plt.rcParams.update(). List of parameters can be found here:
     https://matplotlib.org/stable/api/matplotlib_configuration_api.html#matplotlib.rcParams
 
@@ -77,29 +64,30 @@
     """
     if tight_layout:
         plt.tight_layout()
     plt.show()
 
 
 def save(fig, filename, tight_layout=True):
-    """Saves a figure.
+    """Save and close a figure.
 
     Parameters
     ----------
     fig : matplotlib.figure.Figure
         matplotlib figure object.
     filename : str
         Output filename.
     tight_layout : bool
         Should we call fig.tight_layout()?
     """
     _logger.info(f"Saving {filename}")
     if tight_layout:
         fig.tight_layout()
     fig.savefig(filename)
+    close(fig)
 
 
 def close(fig=None):
     """Close a figure.
 
     Parameters
     ----------
@@ -212,17 +200,17 @@
         Axis object to plot on.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object. Only returned if ax=None.
+        Matplotlib figure object. Only returned if ax=None and filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s). Only returned if ax=None.
+        Matplotlib axis object(s). Only returned if ax=None and filename=None.
     """
 
     # Validation
     if len(x) != len(y):
         raise ValueError("Different number of x and y arrays given.")
 
     if x_range is None:
@@ -298,16 +286,15 @@
     # Add a legend
     if add_legend:
         ax.legend(loc=legend_loc)
 
     # Save figure
     if filename is not None:
         save(fig, filename)
-
-    if create_fig:
+    elif create_fig:
         return fig, ax
 
 
 def plot_scatter(
     x,
     y,
     labels=None,
@@ -361,17 +348,17 @@
         Axis object to plot on.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object. Only returned if ax=None.
+        Matplotlib figure object. Only returned if ax=None and filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s). Only returned if ax=None.
+        Matplotlib axis object(s). Only returned if ax=None and filename=None.
     """
 
     # Validation
     if len(x) != len(y):
         raise ValueError("Different number of x and y arrays given.")
 
     if x_range is None:
@@ -462,16 +449,15 @@
     # Add a legend
     if add_legend:
         ax.legend(loc=legend_loc)
 
     # Save figure
     if filename is not None:
         save(fig, filename)
-
-    if create_fig:
+    elif create_fig:
         return fig, ax
 
 
 def plot_hist(
     data,
     bins,
     labels=None,
@@ -516,17 +502,17 @@
         Axis object to plot on.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object. Only returned if ax=None.
+        Matplotlib figure object. Only returned if ax=None and filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s). Only returned if ax=None.
+        Matplotlib axis object(s). Only returned if ax=None and filename=None.
     """
 
     # Validation
     if len(data) != len(bins):
         raise ValueError("Different number of bins and data.")
 
     if x_range is None:
@@ -585,16 +571,15 @@
     # Add a legend
     if add_legend:
         ax.legend(loc=legend_loc)
 
     # Save the figure if a filename has been pass
     if filename is not None:
         save(fig, filename)
-
-    if create_fig:
+    elif create_fig:
         return fig, ax
 
 
 def plot_bar_chart(
     counts,
     x=None,
     x_range=None,
@@ -633,17 +618,17 @@
         Axis object to plot on.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object. Only returned if ax=None.
+        Matplotlib figure object. Only returned if ax=None and filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s). Only returned if ax=None.
+        Matplotlib axis object(s). Only returned if ax=None and filename=None.
     """
 
     # Validation
     if x is None:
         x = range(1, len(counts) + 1)
     elif len(x) != len(counts):
         raise ValueError("Incorrect number of x-values or counts passed.")
@@ -690,16 +675,15 @@
     ax.set_title(title)
     ax.set_xlabel(x_label)
     ax.set_ylabel(y_label)
 
     # Save the figure if a filename has been pass
     if filename is not None:
         save(fig, filename)
-
-    if create_fig:
+    elif create_fig:
         return fig, ax
 
 
 def plot_gmm(
     data,
     amplitudes,
     means,
@@ -718,14 +702,17 @@
 ):
     """Plot a two component Gaussian mixture model.
 
     Parameters
     ----------
     data : np.ndarray
         Raw data to plot as a histogram.
+    amplitudes : np.ndarray
+        Amplitudes of each Gaussian component.
+        Mixture weights scaled by mixture covariances.
     means : np.ndarray
         Mean of each Gaussian component.
     stddevs : np.ndarray
         Standard deviation of each Gaussian component.
     bins : list of int
         Number of bins for the historgram.
     legend_loc : int
@@ -748,17 +735,17 @@
         Axis object to plot on.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object. Only returned if ax=None.
+        Matplotlib figure object. Only returned if ax=None and filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s). Only returned if ax=None.
+        Matplotlib axis object(s). Only returned if ax=None and filename=None.
     """
 
     # Validation
     if x_range is None:
         x_range = [None, None]
 
     if y_range is None:
@@ -784,115 +771,93 @@
 
     # Create figure
     create_fig = ax is None
     if create_fig:
         fig, ax = create_figure(**fig_kwargs)
 
     # Plot histogram
-    ax.hist(data, bins=bins, histtype="step", density=True)
+    ax.hist(data, bins=bins, histtype="step", density=True, color="tab:blue")
 
     # Plot Gaussian components
     x = np.arange(min(data), max(data), (max(data) - min(data)) / bins)
     y1 = amplitudes[0] * np.exp(-((x - means[0]) ** 2) / (2 * stddevs[0] ** 2))
     y2 = amplitudes[1] * np.exp(-((x - means[1]) ** 2) / (2 * stddevs[1] ** 2))
-    ax.plot(x, y1, label="Off")
-    ax.plot(x, y2, label="On")
-    ax.plot(x, y1 + y2)
+    ax.plot(x, y1, label="Off", color="tab:orange")
+    ax.plot(x, y2, label="On", color="tab:green")
+    ax.plot(x, y1 + y2, color="tab:red")
 
     # Set axis range
-    ax.set_xlim(x_range[0], x_range[1])
-    ax.set_ylim(y_range[0], y_range[1])
+    if not any(r is None for r in x_range):
+        ax.set_xlim(x_range[0], x_range[1])
+    if not any(r is None for r in y_range):
+        ax.set_ylim(y_range[0], y_range[1])
 
     # Set title and axis labels
     ax.set_title(title)
     ax.set_xlabel(x_label)
     ax.set_ylabel(y_label)
 
     # Add legend
-    ax.legend(loc=legend_loc)
+    if legend_loc is not None:
+        ax.legend(loc=legend_loc)
 
     # Save the figure if a filename has been pass
     if filename is not None:
         save(fig, filename)
-
-    if create_fig:
+    elif create_fig:
         return fig, ax
 
 
 def plot_violin(
     data,
-    show_mean=True,
-    show_median=True,
-    legend_loc=1,
     x=None,
-    x_range=None,
-    y_range=None,
     x_label=None,
     y_label=None,
     title=None,
-    plot_kwargs=None,
     fig_kwargs=None,
     ax=None,
     filename=None,
 ):
     """Violin plot.
 
     Parameters
     ----------
     data : list of np.ndarray
         Data to plot.
-    show_mean : bool
-        Should we show the mean?
-    show_median : bool
-        Should we show the median?
-    legend_loc : int
-        Position for the legend.
     x : list or np.ndarray
         x-values for data.
-    x_range : list
-        Minimum and maximum for x-axis.
-    y_range : list
-        Minimum and maximum for y-axis.
     x_label : str
         Label for x-axis.
     y_label : str
         Label for y-axis.
     title : str
         Figure title.
-    plot_kwargs : dict
-        Arguments to pass to the ax.violinplot method.
     fig_kwargs : dict
         Arguments to pass to plt.subplots.
     ax : matplotlib.axes.axes
         Axis object to plot on.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object. Only returned if ax=None.
+        Matplotlib figure object. Only returned if ax=None and filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s). Only returned if ax=None.
+        Matplotlib axis object(s). Only returned if ax=None and filename=None.
     """
 
     # Validation
     if x is None:
-        x = range(len(data))
+        x = np.arange(len(data)) + 1
     elif len(x) != len(data):
         raise ValueError("Incorrect number of x-values or data passed.")
     else:
         x = [str(xi) for xi in x]
 
-    if x_range is None:
-        x_range = [None, None]
-
-    if y_range is None:
-        y_range = [None, None]
-
     if ax is not None:
         if filename is not None:
             raise ValueError(
                 "Please use plotting.save() to save the figure instead of the "
                 + "filename argument."
             )
         if isinstance(ax, np.ndarray):
@@ -900,54 +865,39 @@
 
     default_fig_kwargs = {"figsize": (7, 4)}
     if fig_kwargs is None:
         fig_kwargs = default_fig_kwargs
     else:
         fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
-    if plot_kwargs is None:
-        plot_kwargs = {}
-
-    # Replace emtpy lists in data with a pair of nans
-    data = [np.array([np.nan, np.nan]) if len(d) == 0 else d for d in data]
+    # Create a pandas DataFrame
+    data_dict = {}
+    for x, d in zip(x, data):
+        data_dict[x] = []
+        for y in d:
+            data_dict[x].append(y)
+    df = pd.DataFrame(data_dict)
 
     # Create figure
     create_fig = ax is None
     if create_fig:
         fig, ax = create_figure(**fig_kwargs)
 
     # Plot violins
-    ax.violinplot(data, positions=range(len(x)), showextrema=False)
-    if show_mean:
-        ax.scatter(
-            x, [np.mean(d) for d in data], label="Mean", marker="+", color="black"
-        )
-    if show_median:
-        ax.scatter(
-            x, [np.median(d) for d in data], label="Median", marker="x", color="black"
-        )
-
-    # Set axis range
-    ax.set_xlim(x_range[0], x_range[1])
-    ax.set_ylim(y_range[0], y_range[1])
+    sns.violinplot(df, ax=ax)
 
     # Set title and axis labels
     ax.set_title(title)
     ax.set_xlabel(x_label)
     ax.set_ylabel(y_label)
 
-    # Add a legend
-    if show_mean and show_median:
-        ax.legend(loc=legend_loc)
-
     # Save the figure if a filename has been pass
     if filename is not None:
         save(fig, filename)
-
-    if create_fig:
+    elif create_fig:
         return fig, ax
 
 
 def plot_time_series(
     time_series,
     n_samples=None,
     y_tick_values=None,
@@ -974,17 +924,17 @@
         The axis on which to plot the data. If not given, a new axis is created.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object. Only returned if ax=None.
+        Matplotlib figure object. Only returned if ax=None and filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s). Only returned if ax=None.
+        Matplotlib axis object(s). Only returned if ax=None and filename=None.
     """
     time_series = np.asarray(time_series)
     n_samples = min(n_samples or np.inf, time_series.shape[0])
     n_channels = time_series.shape[1]
 
     # Validation
     if ax is not None:
@@ -1033,16 +983,15 @@
         ax.set_yticklabels(y_tick_values)
     else:
         ax.set_yticks([])
 
     # Save figure
     if filename is not None:
         save(fig, filename)
-
-    if create_fig:
+    elif create_fig:
         return fig, ax
 
 
 def plot_separate_time_series(
     *time_series,
     n_samples=None,
     sampling_frequency=None,
@@ -1067,17 +1016,17 @@
         Keyword arguments to be passed on to matplotlib.pyplot.plot.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object.
+        Matplotlib figure object. Only returned if filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s).
+        Matplotlib axis object(s). Only returned if filename=None.
     """
     time_series = np.asarray(time_series)
     n_samples = n_samples or min([ts.shape[0] for ts in time_series])
     n_lines = time_series[0].shape[1]
 
     default_fig_kwargs = {"figsize": (20, 10), "sharex": "all"}
     if fig_kwargs is None:
@@ -1112,16 +1061,16 @@
         axes[-1].set_xlabel("Time (s)")
     else:
         axes[-1].set_xlabel("Sample")
 
     # Save figure
     if filename is not None:
         save(fig, filename)
-
-    return fig, axes
+    else:
+        return fig, axes
 
 
 def plot_epoched_time_series(
     data,
     time_index,
     sampling_frequency=None,
     pre=125,
@@ -1165,17 +1114,17 @@
         The axis on which to plot the data. If not given, a new axis is created.
     filename : str
         Output_filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object. Only returned if ax=None.
+        Matplotlib figure object. Only returned if ax=None and filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s). Only returned if ax=None.
+        Matplotlib axis object(s). Only returned if ax=None and filename=None.
     """
     from osl_dynamics.data.task import epoch_mean
 
     epoched_1 = epoch_mean(data, time_index, pre, post)
 
     x_label = "Sample"
     time_index = np.arange(-pre, post)
@@ -1225,16 +1174,15 @@
     # Add a legend
     if legend:
         ax.legend(loc=legend_loc)
 
     # Save the figure if a filename has been passed
     if filename is not None:
         save(fig, filename)
-
-    if create_fig:
+    elif create_fig:
         return fig, ax
 
 
 def plot_matrices(
     matrix,
     group_color_scale=True,
     titles=None,
@@ -1268,17 +1216,17 @@
         Should we show the elements on a log scale?
     filename: str
         A file to which to save the figure.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object.
+        Matplotlib figure object. Only returned if filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s).
+        Matplotlib axis object(s). Only returned if filename=None.
     """
     matrix = np.array(matrix)
     if matrix.ndim == 2:
         matrix = matrix[None, :]
     if matrix.ndim != 3:
         raise ValueError("Must be a 3D array.")
     short, long, empty = rough_square_axes(len(matrix))
@@ -1328,16 +1276,16 @@
             plt.colorbar(pl, cax=cax)
         plt.tight_layout()
 
     fig.suptitle(main_title)
 
     if filename is not None:
         save(fig, filename, tight_layout=False)
-
-    return fig, axes
+    else:
+        return fig, axes
 
 
 def plot_connections(
     weights,
     labels=None,
     ax=None,
     cmap="hot",
@@ -1367,17 +1315,17 @@
         A string corresponding to a matplotlib color.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object.
+        Matplotlib figure object. Only returned if filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s).
+        Matplotlib axis object(s). Only returned if filename=None.
     """
     weights = np.abs(weights)
     x, y = np.diag_indices_from(weights)
     weights[x, y] = 0
     weights /= weights.max()
 
     inner = 0.9
@@ -1499,16 +1447,16 @@
             )
 
         ax.autoscale_view()
         plt.setp(ax.spines.values(), visible=False)
 
     if filename is not None:
         save(fig, filename)
-
-    return fig, ax
+    else:
+        return fig, ax
 
 
 def topoplot(
     layout,
     data,
     channel_names=None,
     plot_boxes=False,
@@ -1555,15 +1503,15 @@
         number of field isolines to show on the plot.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object.
+        Matplotlib figure object. Only returned if filename=None.
     """
     topology = Topology(layout)
 
     if channel_names is not None:
         topology.keep_channels(channel_names)
 
     fig = topology.plot_data(
@@ -1576,16 +1524,16 @@
         axis=axis,
         cmap=cmap,
         n_contours=n_contours,
     )
 
     if filename is not None:
         save(fig, filename)
-
-    return fig
+    else:
+        return fig
 
 
 def plot_brain_surface(
     values,
     mask_file,
     parcellation_file,
     filename=None,
@@ -1653,14 +1601,15 @@
     cmap="Set3",
     sampling_frequency=None,
     y_labels=None,
     title=None,
     plot_kwargs=None,
     fig_kwargs=None,
     filename=None,
+    axes=None,
 ):
     """Plot alpha.
 
     Parameters
     ----------
     alpha : numpy.ndarray
         A collection of alphas passed as separate arguments.
@@ -1676,26 +1625,46 @@
         Title for the plot.
     plot_kwargs : dict
         Any parameters to be passed to matplotlib.pyplot.stackplot.
     fig_kwargs : dict
         Arguments to pass to matplotlib.pyplot.subplots.
     filename : str
         Output filename.
+    axes: list of matplotlib.pyplot.Axes
+        A list of matplotlib axes to plot on. If None, a new figure is created.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object.
+        Matplotlib figure object. Only returned if filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s).
+        Matplotlib axis object(s). Only returned if filename=None.
     """
     n_alphas = len(alpha)
+    if isinstance(axes, plt.Axes):
+        axes = [axes]
+    if axes is not None and len(axes) != n_alphas:
+        raise ValueError("Number of axes must match number of alphas.")
+
     n_modes = max(a.shape[1] for a in alpha)
     n_samples = min(n_samples or np.inf, alpha[0].shape[0])
-    if cmap in QUAL_CMAPS:
+    if cmap in [
+        "Pastel1",
+        "Pastel2",
+        "Paired",
+        "Accent",
+        "Dark2",
+        "Set1",
+        "Set2",
+        "Set3",
+        "tab10",
+        "tab20",
+        "tab20b",
+        "tab20c",
+    ]:
         cmap = plt.cm.get_cmap(name=cmap)
     else:
         cmap = plt.cm.get_cmap(name=cmap, lut=n_modes)
     colors = cmap.colors
 
     # Validation
     default_fig_kwargs = dict(
@@ -1715,19 +1684,21 @@
     if y_labels is None:
         y_labels = [None] * n_alphas
     elif isinstance(y_labels, str):
         y_labels = [y_labels] * n_alphas
     elif len(y_labels) != n_alphas:
         raise ValueError("Incorrect number of y_labels passed.")
 
-    # Create figure
-    fig, axes = create_figure(n_alphas, **fig_kwargs)
+    # Create figure if axes not passed
+    if axes is None:
+        fig, axes = create_figure(n_alphas, **fig_kwargs)
+    else:
+        fig = axes[0].get_figure()
 
-    # If n_alphas is one then axes won't be iterable
-    if not isinstance(axes, np.ndarray):
+    if isinstance(axes, plt.Axes):
         axes = [axes]
 
     # Plot data
     for a, ax, y_label in zip(alpha, axes, y_labels):
         time_vector = (
             np.arange(n_samples) / sampling_frequency
             if sampling_frequency
@@ -1753,16 +1724,16 @@
     cb_ax = fig.add_axes([0.95, 0.15, 0.025, 0.7])
     cb = fig.colorbar(mappable, cax=cb_ax, ticks=np.arange(0.5, n_modes, 1))
     cb.ax.set_yticklabels(range(1, n_modes + 1))
 
     # Save to file if a filename as been passed
     if filename is not None:
         save(fig, filename, tight_layout=False)
-
-    return fig, axes
+    else:
+        return fig, axes
 
 
 def plot_mode_lifetimes(
     mode_time_course,
     bins="auto",
     density=False,
     match_scale_x=False,
@@ -1804,17 +1775,17 @@
         Keyword arguments to pass to matplotlib.pyplot.subplots.
     filename : str
         A file to which to save the figure.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object.
+        Matplotlib figure object. Only returned if filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s).
+        Matplotlib axis object(s). Only returned if filename=None.
     """
     from osl_dynamics.analysis import modes
 
     n_plots = mode_time_course.shape[1]
     short, long, empty = rough_square_axes(n_plots)
     colors = get_colors(n_plots)
 
@@ -1888,16 +1859,16 @@
             axis.set_xlim(x_range[0], x_range[1])
         axis.set_xlabel(x_label)
         axis.set_ylabel(y_label)
 
     # Save file is a filename has been passed
     if filename is not None:
         save(fig, filename)
-
-    return fig, axes
+    else:
+        return fig, axes
 
 
 def plot_psd_topo(
     f, psd, parcellation_file=None, topomap_pos=[0.45, 0.55, 0.5, 0.55], filename=None
 ):
     """PLot PSDs for parcels and a topomap.
 
@@ -1916,35 +1887,35 @@
         right. This is not used if parcellation_file=None.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
-        Matplotlib figure object.
+        Matplotlib figure object. Only returned if filename=None.
     ax : matplotlib.pyplot.axis.
-        Matplotlib axis object(s).
+        Matplotlib axis object(s). Only returned if filename=None.
     """
 
     if parcellation_file is not None:
         # Get the center of each parcel
         parcellation = Parcellation(parcellation_file)
         roi_centers = parcellation.roi_centers()
 
         # Re-order to use colour to indicate anterior->posterior location
         order = np.argsort(roi_centers[:, 1])
         roi_centers = roi_centers[order]
-        psd = np.copy(psd)[order[::-1]]
+        psd = np.copy(psd)[order]
 
     n_parcels = psd.shape[0]
 
     # Plot PSDs
     fig, ax = create_figure()
-    cmap = plt.get_cmap()
-    for i in range(n_parcels):
+    cmap = plt.cm.viridis_r
+    for i in reversed(range(n_parcels)):
         ax.plot(f, psd[i], c=cmap(i / n_parcels))
     ax.set_xlabel("Frequency (Hz)")
     ax.set_ylabel("PSD (a.u.)")
     ax.set_xlim(f[0], f[-1])
     plt.tight_layout()
 
     if parcellation_file is not None:
@@ -1957,9 +1928,53 @@
             colorbar=False,
             axes=inside_ax,
         )
 
     # Save
     if filename is not None:
         save(fig, filename, tight_layout=False)
+    else:
+        return fig, ax
 
-    return fig, ax
+
+def plot_summary_stats_group_diff(name, summary_stats, pvalues, assignments, filename):
+    """Plot summary statistics for two groups as violin plots.
+
+    Parameters
+    ----------
+    name : str
+        Name of the summary statistic.
+    summary_stats : np.ndarray
+        Summary statistics. Shape is (n_subjects, n_states).
+    pvalues : np.ndarray
+        p-values for each summary statistic difference. Shape is (n_states,).
+    assignments : np.ndarray
+        Array of 1s and 2s indicating group assignment. Shape is (n_subjects,).
+    filename : str
+        Output filename.
+    """
+    # Create a pandas DataFrame to hold the summary stats
+    ss_dict = {name: [], "State": [], "Group": []}
+    n_subjects, n_states = summary_stats.shape
+    for subject in range(n_subjects):
+        for state in range(n_states):
+            ss_dict[name].append(summary_stats[subject, state])
+            ss_dict["State"].append(state + 1)
+            ss_dict["Group"].append(int(assignments[subject]))
+    ss_df = pd.DataFrame(ss_dict)
+
+    # Plot a half violin for each group
+    sns.violinplot(data=ss_df, x="State", y=name, hue="Group", split=True)
+
+    # Add a star above the violin to indicate significance
+    scatter_kwargs = {"c": "black", "s": 32, "marker": "*"}
+    for i in range(n_states):
+        if pvalues[i] < 0.01:
+            plt.scatter(i - 0.075, summary_stats[:, i].max() * 1.6, **scatter_kwargs)
+            plt.scatter(i + 0.075, summary_stats[:, i].max() * 1.6, **scatter_kwargs)
+        elif pvalues[i] < 0.05:
+            plt.scatter(i, summary_stats[:, i].max() * 1.6, **scatter_kwargs)
+
+    # Save
+    _logger.info(f"Saving {filename}")
+    plt.savefig(filename)
+    plt.close()
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics/utils/topoplots.py` & `osl-dynamics-1.2.1/osl_dynamics/utils/topoplots.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Classes and functions to make topoplots.
 
 """
 
-
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from scipy.interpolate import griddata
+
 from osl_dynamics.files.scanner import layouts
 
 
 def available_layouts():
     layout_names = [file.stem for file in sorted(layouts.glob("*.lay"))]
     return layout_names
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics.egg-info/PKG-INFO` & `osl-dynamics-1.2.1/osl_dynamics.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osl-dynamics
-Version: 1.2.0
+Version: 1.2.1
 Summary: Models for infering dynamics in neuroimaging data
 Home-page: https://github.com/OHBA-analysis/osl-dynamics
 License: MIT
 Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 ============
@@ -99,60 +99,8 @@
 .. code-block:: shell
 
     pip install osl-dynamics
 
 Editing Source Code
 ===================
 
-Formatting and Conventions
---------------------------
-
-We use the python code formatter ``black`` to give a consistent code layout in our source files. To install:
-
-.. code-block:: shell
-
-    conda activate <env>
-    pip install black
-
-To format a source file:
-
-.. code-block:: shell
-
-    black <filename>.py
-
-Please run ``black`` on any edited files before commiting changes.
-
-Git Workflow
-------------
-
-We use git for version control. There is one ``main`` branch. To add changes:
-
-Create a feature branch for changes:
-
-.. code-block:: shell
-
-    git checkout main
-    git pull
-    git checkout -b <branch-name>
-
-Make changes to file and commit it to the branch:
-
-.. code-block:: shell
-
-    git add <file>
-    git commit -m "Short description of changes"
-
-When writing commit messages please follow the conventions `here <https://www.conventionalcommits.org/en/v1.0.0-beta.2/#specification>`_.
-
-Then either push the new branch to the remote repository:
-
-.. code-block:: shell
-
-    git push --set-upstream origin <branch-name>
-
-and create a pull request (recommended), or merge branch into ``main`` and push:
-
-.. code-block:: shell
-
-    git checkout main
-    git merge <branch-name>
-    git push
+See `here <https://github.com/OHBA-analysis/osl-dynamics/blob/main/doc/using_bmrc.rst>`_ for useful info regarding how to use the BMRC cluster and how to edit the source code.
```

### Comparing `osl-dynamics-1.2.0/osl_dynamics.egg-info/SOURCES.txt` & `osl-dynamics-1.2.1/osl_dynamics.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 README.rst
 setup.cfg
 setup.py
 osl_dynamics/__init__.py
 osl_dynamics/array_ops.py
-osl_dynamics/pipeline.py
 osl_dynamics.egg-info/PKG-INFO
 osl_dynamics.egg-info/SOURCES.txt
 osl_dynamics.egg-info/dependency_links.txt
 osl_dynamics.egg-info/requires.txt
 osl_dynamics.egg-info/top_level.txt
 osl_dynamics/analysis/__init__.py
 osl_dynamics/analysis/connectivity.py
+osl_dynamics/analysis/fisher_kernel.py
 osl_dynamics/analysis/gmm.py
 osl_dynamics/analysis/modes.py
 osl_dynamics/analysis/power.py
 osl_dynamics/analysis/regression.py
 osl_dynamics/analysis/spectral.py
 osl_dynamics/analysis/static.py
+osl_dynamics/analysis/statistics.py
 osl_dynamics/analysis/workbench.py
+osl_dynamics/config_api/__init__.py
+osl_dynamics/config_api/pipeline.py
+osl_dynamics/config_api/wrappers.py
 osl_dynamics/data/__init__.py
 osl_dynamics/data/base.py
 osl_dynamics/data/osl.py
 osl_dynamics/data/processing.py
 osl_dynamics/data/rw.py
 osl_dynamics/data/spm.py
 osl_dynamics/data/task.py
```

### Comparing `osl-dynamics-1.2.0/setup.cfg` & `osl-dynamics-1.2.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 [metadata]
 name = osl-dynamics
-version = 1.2.0
+version = 1.2.1
 description = Models for infering dynamics in neuroimaging data
 license = MIT
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/OHBA-analysis/osl-dynamics
 project_urls = 
 	Documentation = https://osl-dynamics.readthedocs.io/en/latest/
 
 [options]
 install_requires = 
+	glmtools
 	mat73
 	matplotlib
 	mne
 	nibabel
 	nilearn
 	numba
 	numpy
 	pandas
-	pre-commit
 	pyyaml
 	pqdm
 	scipy
 	scikit-learn
 	seaborn
+	tabulate
 	tensorflow_probability
 	tqdm
 packages = 
 	osl_dynamics
 	osl_dynamics.analysis
+	osl_dynamics.config_api
 	osl_dynamics.data
 	osl_dynamics.files
 	osl_dynamics.files.mask
 	osl_dynamics.files.parcellation
 	osl_dynamics.files.scanner
 	osl_dynamics.files.scanner.layouts
 	osl_dynamics.files.scene
```

