# Comparing `tmp/dark_emulator-1.0.23.tar.gz` & `tmp/dark_emulator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dark_emulator-1.0.23.tar", last modified: Fri Oct 29 16:00:49 2021, max compression
+gzip compressed data, was "dark_emulator-1.1.1.tar", last modified: Fri Apr 14 06:46:53 2023, max compression
```

## Comparing `dark_emulator-1.0.23.tar` & `dark_emulator-1.1.1.tar`

### file list

```diff
@@ -1,110 +1,107 @@
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.560127 dark_emulator-1.0.23/
--rw-r--r--   0 nishimichi   (501) staff       (20)      170 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/MANIFEST.in
--rw-r--r--   0 nishimichi   (501) staff       (20)     3129 2021-10-29 16:00:49.559951 dark_emulator-1.0.23/PKG-INFO
--rw-r--r--   0 nishimichi   (501) staff       (20)     2372 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/README.md
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.545984 dark_emulator-1.0.23/dark_emulator/
--rw-r--r--   0 nishimichi   (501) staff       (20)      171 2021-10-29 15:58:27.000000 dark_emulator-1.0.23/dark_emulator/__init__.py
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.548066 dark_emulator-1.0.23/dark_emulator/darkemu/
--rw-r--r--   0 nishimichi   (501) staff       (20)       37 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/__init__.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     5031 2021-08-06 12:24:47.000000 dark_emulator-1.0.23/dark_emulator/darkemu/auto.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     5493 2021-05-07 09:38:04.000000 dark_emulator-1.0.23/dark_emulator/darkemu/cosmo_util.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     2640 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/cross.py
--rw-r--r--   0 nishimichi   (501) staff       (20)    50988 2021-05-07 09:38:04.000000 dark_emulator-1.0.23/dark_emulator/darkemu/de_interface.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     5225 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/gamma1.py
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.548318 dark_emulator-1.0.23/dark_emulator/darkemu/gp/
--rw-r--r--   0 nishimichi   (501) staff       (20)       23 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/gp/__init__.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     3611 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/gp/gp6d.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     5750 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/hmf.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     5962 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/pklin.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     4193 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/sigmaM.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     3401 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/sigmad.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     1854 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/darkemu/xinl.py
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.549214 dark_emulator-1.0.23/dark_emulator/data/
--rw-r--r--   0 nishimichi   (501) staff       (20)    90000 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/data/cparams_3d.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)   120000 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/data/cparams_4d.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)     9712 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/data/params.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)    29372 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/data/params_40x10.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)    12080 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/data/params_80models.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)      180 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/data/scales.dat
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.545038 dark_emulator-1.0.23/dark_emulator/learned_data/
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.549851 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/
--rw-r--r--   0 nishimichi   (501) staff       (20)     2688 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/coeff_all.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      832 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/gp6d_hyperparams.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      132 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/gp6d_kerneltype.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)    26336 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/pca_eigvec.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     2688 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/yerr.npy
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.550649 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1_dm/
--rw-r--r--   0 nishimichi   (501) staff       (20)     1408 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1_dm/coeff_all.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      480 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1_dm/gp6d_hyperparams.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      130 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1_dm/gp6d_kerneltype.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      800 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1_dm/pca_eigvec.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     1408 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/gamma1_dm/yerr.npy
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.551458 dark_emulator-1.0.23/dark_emulator/learned_data/hmf/
--rw-r--r--   0 nishimichi   (501) staff       (20)     3968 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/hmf/coeff_all.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     1184 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/hmf/gp6d_hyperparams.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      134 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/hmf/gp6d_kerneltype.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     2144 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/hmf/pca_eigvec.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     3968 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/hmf/yerr.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      464 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/hmf/ymeans.npy
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.552885 dark_emulator-1.0.23/dark_emulator/learned_data/pklin/
--rw-r--r--   0 nishimichi   (501) staff       (20)   612171 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/pklin/coeff_all.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)     2577 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/pklin/gp_params.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)       48 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/pklin/ktypes.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)      511 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/pklin/pca_avg.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)   101876 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/pklin/pca_eigvec.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)     5000 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/pklin/pca_mean.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)      500 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/pklin/pca_std.dat
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.553849 dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/
--rw-r--r--   0 nishimichi   (501) staff       (20)   122443 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/coeff_all.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)      604 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/gp_params.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)       12 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/ktypes.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)      102 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/pca_avg.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)    61703 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/pca_eigvec.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)    15240 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/pca_mean.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)      100 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/pca_std.dat
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.554437 dark_emulator-1.0.23/dark_emulator/learned_data/sigmad/
--rw-r--r--   0 nishimichi   (501) staff       (20)    30692 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmad/coeff_all.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)      150 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmad/gp_params.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)        3 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmad/ktypes.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)       25 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmad/sigd_avg.dat
--rw-r--r--   0 nishimichi   (501) staff       (20)       25 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/sigmad/sigd_std.dat
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.556016 dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/
--rw-r--r--   0 nishimichi   (501) staff       (20)     7808 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/coeff_all.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     2240 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/gp6d_hyperparams.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      140 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/gp6d_kerneltype.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      248 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/loge_xs.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)  1524224 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/pca_eigvec.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     7808 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/yerr.npy
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.557307 dark_emulator-1.0.23/dark_emulator/learned_data/xicross/
--rw-r--r--   0 nishimichi   (501) staff       (20)     3328 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xicross/coeff_all.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     1008 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xicross/gp6d_hyperparams.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      133 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xicross/gp6d_kerneltype.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      608 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xicross/loge_xs.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)   720848 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xicross/pca_eigvec.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     3328 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xicross/yerr.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)   144272 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xicross/ymeans.npy
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.558107 dark_emulator-1.0.23/dark_emulator/learned_data/xinl/
--rw-r--r--   0 nishimichi   (501) staff       (20)     3408 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xinl/coeff_all.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     1888 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xinl/gp6d_hyperparams.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)      138 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xinl/gp6d_kerneltype.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)    69008 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xinl/pca_eigvec.npy
--rw-r--r--   0 nishimichi   (501) staff       (20)     3408 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/learned_data/xinl/yerr.npy
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.558345 dark_emulator-1.0.23/dark_emulator/model_hod/
--rw-r--r--   0 nishimichi   (501) staff       (20)       72 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/model_hod/__init__.py
--rw-r--r--   0 nishimichi   (501) staff       (20)    79465 2021-10-29 01:41:27.000000 dark_emulator-1.0.23/dark_emulator/model_hod/hod_interface.py
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.558786 dark_emulator-1.0.23/dark_emulator/pyfftlog_interface/
--rw-r--r--   0 nishimichi   (501) staff       (20)       59 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/pyfftlog_interface/__init__.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     7214 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/pyfftlog_interface/pyfftlog_class.py
--rw-r--r--   0 nishimichi   (501) staff       (20)     7374 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/dark_emulator/pyfftlog_interface/pyfftlog_funcs.py
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.546673 dark_emulator-1.0.23/dark_emulator.egg-info/
--rw-r--r--   0 nishimichi   (501) staff       (20)     3129 2021-10-29 16:00:49.000000 dark_emulator-1.0.23/dark_emulator.egg-info/PKG-INFO
--rw-r--r--   0 nishimichi   (501) staff       (20)     3709 2021-10-29 16:00:49.000000 dark_emulator-1.0.23/dark_emulator.egg-info/SOURCES.txt
--rw-r--r--   0 nishimichi   (501) staff       (20)        1 2021-10-29 16:00:49.000000 dark_emulator-1.0.23/dark_emulator.egg-info/dependency_links.txt
--rw-r--r--   0 nishimichi   (501) staff       (20)       28 2021-10-29 16:00:49.000000 dark_emulator-1.0.23/dark_emulator.egg-info/requires.txt
--rw-r--r--   0 nishimichi   (501) staff       (20)      118 2021-10-29 16:00:49.000000 dark_emulator-1.0.23/dark_emulator.egg-info/top_level.txt
-drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2021-10-29 16:00:49.559215 dark_emulator-1.0.23/docs/
--rw-r--r--   0 nishimichi   (501) staff       (20)   271533 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/docs/tutorial-hod.ipynb
--rw-r--r--   0 nishimichi   (501) staff       (20)   878432 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/docs/tutorial.ipynb
--rw-r--r--   0 nishimichi   (501) staff       (20)      122 2021-05-07 01:04:23.000000 dark_emulator-1.0.23/requirements.txt
--rw-r--r--   0 nishimichi   (501) staff       (20)       38 2021-10-29 16:00:49.560179 dark_emulator-1.0.23/setup.cfg
--rw-r--r--   0 nishimichi   (501) staff       (20)     1373 2021-10-29 15:57:02.000000 dark_emulator-1.0.23/setup.py
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.314174 dark_emulator-1.1.1/
+-rw-r--r--   0 nishimichi   (501) staff       (20)     1075 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/LICENSE
+-rw-r--r--   0 nishimichi   (501) staff       (20)      170 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/MANIFEST.in
+-rw-r--r--   0 nishimichi   (501) staff       (20)     2887 2023-04-14 06:46:53.314036 dark_emulator-1.1.1/PKG-INFO
+-rw-r--r--   0 nishimichi   (501) staff       (20)     2461 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/README.md
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.301076 dark_emulator-1.1.1/dark_emulator/
+-rw-r--r--   0 nishimichi   (501) staff       (20)      186 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/__init__.py
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.303573 dark_emulator-1.1.1/dark_emulator/darkemu/
+-rw-r--r--   0 nishimichi   (501) staff       (20)       37 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/darkemu/__init__.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     5053 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/darkemu/auto.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     5522 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/darkemu/cosmo_util.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     2662 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/darkemu/cross.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)    51638 2023-04-14 06:04:18.000000 dark_emulator-1.1.1/dark_emulator/darkemu/de_interface.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     5255 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/darkemu/gamma1.py
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.303835 dark_emulator-1.1.1/dark_emulator/darkemu/gp/
+-rw-r--r--   0 nishimichi   (501) staff       (20)       23 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/darkemu/gp/__init__.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     3611 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/darkemu/gp/gp6d.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     5750 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/darkemu/hmf.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     5991 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/darkemu/pklin.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     4222 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/darkemu/sigmaM.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     3430 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/darkemu/sigmad.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)     1876 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/darkemu/xinl.py
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.304714 dark_emulator-1.1.1/dark_emulator/data/
+-rw-r--r--   0 nishimichi   (501) staff       (20)    90000 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/data/cparams_3d.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)   120000 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/data/cparams_4d.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)     9712 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/data/params.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)    29372 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/data/params_40x10.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)    12080 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/data/params_80models.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)      180 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/data/scales.dat
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.299824 dark_emulator-1.1.1/dark_emulator/learned_data/
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.305332 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/
+-rw-r--r--   0 nishimichi   (501) staff       (20)     2688 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/coeff_all.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      832 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/gp6d_hyperparams.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      132 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/gp6d_kerneltype.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)    26336 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/pca_eigvec.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     2688 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/yerr.npy
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.305965 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1_dm/
+-rw-r--r--   0 nishimichi   (501) staff       (20)     1408 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1_dm/coeff_all.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      480 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1_dm/gp6d_hyperparams.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      130 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1_dm/gp6d_kerneltype.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      800 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1_dm/pca_eigvec.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     1408 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/gamma1_dm/yerr.npy
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.306677 dark_emulator-1.1.1/dark_emulator/learned_data/hmf/
+-rw-r--r--   0 nishimichi   (501) staff       (20)     3968 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/hmf/coeff_all.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     1184 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/hmf/gp6d_hyperparams.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      134 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/hmf/gp6d_kerneltype.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     2144 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/hmf/pca_eigvec.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     3968 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/hmf/yerr.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      464 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/hmf/ymeans.npy
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.307870 dark_emulator-1.1.1/dark_emulator/learned_data/pklin/
+-rw-r--r--   0 nishimichi   (501) staff       (20)   612171 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/pklin/coeff_all.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)     2577 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/pklin/gp_params.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)       48 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/pklin/ktypes.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)      511 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/pklin/pca_avg.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)   101876 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/pklin/pca_eigvec.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)     5000 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/pklin/pca_mean.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)      500 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/pklin/pca_std.dat
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.308793 dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/
+-rw-r--r--   0 nishimichi   (501) staff       (20)   122443 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/coeff_all.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)      604 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/gp_params.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)       12 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/ktypes.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)      102 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/pca_avg.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)    61703 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/pca_eigvec.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)    15240 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/pca_mean.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)      100 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/pca_std.dat
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.309419 dark_emulator-1.1.1/dark_emulator/learned_data/sigmad/
+-rw-r--r--   0 nishimichi   (501) staff       (20)    30692 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmad/coeff_all.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)      150 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmad/gp_params.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)        3 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmad/ktypes.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)       25 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmad/sigd_avg.dat
+-rw-r--r--   0 nishimichi   (501) staff       (20)       25 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/sigmad/sigd_std.dat
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.310839 dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/
+-rw-r--r--   0 nishimichi   (501) staff       (20)     7808 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/coeff_all.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     2240 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/gp6d_hyperparams.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      140 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/gp6d_kerneltype.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      248 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/loge_xs.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)  1524224 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/pca_eigvec.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     7808 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/yerr.npy
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.312020 dark_emulator-1.1.1/dark_emulator/learned_data/xicross/
+-rw-r--r--   0 nishimichi   (501) staff       (20)     3328 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xicross/coeff_all.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     1008 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xicross/gp6d_hyperparams.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      133 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xicross/gp6d_kerneltype.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      608 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xicross/loge_xs.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)   720848 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xicross/pca_eigvec.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     3328 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xicross/yerr.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)   144272 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xicross/ymeans.npy
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.312716 dark_emulator-1.1.1/dark_emulator/learned_data/xinl/
+-rw-r--r--   0 nishimichi   (501) staff       (20)     3408 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xinl/coeff_all.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     1888 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xinl/gp6d_hyperparams.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)      138 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xinl/gp6d_kerneltype.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)    69008 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xinl/pca_eigvec.npy
+-rw-r--r--   0 nishimichi   (501) staff       (20)     3408 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/dark_emulator/learned_data/xinl/yerr.npy
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.312959 dark_emulator-1.1.1/dark_emulator/model_hod/
+-rw-r--r--   0 nishimichi   (501) staff       (20)       71 2023-04-14 06:04:18.000000 dark_emulator-1.1.1/dark_emulator/model_hod/__init__.py
+-rw-r--r--   0 nishimichi   (501) staff       (20)    84593 2023-04-14 06:27:44.000000 dark_emulator-1.1.1/dark_emulator/model_hod/hod_interface.py
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.301788 dark_emulator-1.1.1/dark_emulator.egg-info/
+-rw-r--r--   0 nishimichi   (501) staff       (20)     2887 2023-04-14 06:46:53.000000 dark_emulator-1.1.1/dark_emulator.egg-info/PKG-INFO
+-rw-r--r--   0 nishimichi   (501) staff       (20)     3570 2023-04-14 06:46:53.000000 dark_emulator-1.1.1/dark_emulator.egg-info/SOURCES.txt
+-rw-r--r--   0 nishimichi   (501) staff       (20)        1 2023-04-14 06:46:53.000000 dark_emulator-1.1.1/dark_emulator.egg-info/dependency_links.txt
+-rw-r--r--   0 nishimichi   (501) staff       (20)       19 2023-04-14 06:46:53.000000 dark_emulator-1.1.1/dark_emulator.egg-info/requires.txt
+-rw-r--r--   0 nishimichi   (501) staff       (20)       85 2023-04-14 06:46:53.000000 dark_emulator-1.1.1/dark_emulator.egg-info/top_level.txt
+drwxr-xr-x   0 nishimichi   (501) staff       (20)        0 2023-04-14 06:46:53.313381 dark_emulator-1.1.1/docs/
+-rw-r--r--   0 nishimichi   (501) staff       (20)   271533 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/docs/tutorial-hod.ipynb
+-rw-r--r--   0 nishimichi   (501) staff       (20)   878432 2022-04-29 07:25:07.000000 dark_emulator-1.1.1/docs/tutorial.ipynb
+-rw-r--r--   0 nishimichi   (501) staff       (20)      113 2023-04-14 06:33:01.000000 dark_emulator-1.1.1/requirements.txt
+-rw-r--r--   0 nishimichi   (501) staff       (20)       38 2023-04-14 06:46:53.314212 dark_emulator-1.1.1/setup.cfg
+-rw-r--r--   0 nishimichi   (501) staff       (20)     1325 2023-04-14 06:46:20.000000 dark_emulator-1.1.1/setup.py
```

### Comparing `dark_emulator-1.0.23/PKG-INFO` & `dark_emulator-1.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 Metadata-Version: 2.1
 Name: dark_emulator
-Version: 1.0.23
+Version: 1.1.1
 Summary: dark emulator package
 Home-page: https://dark-emulator.readthedocs.io
-Author: Takahiro Nishimichi, Hironao Miyatake
+Author: Takahiro Nishimichi, Hironao Miyatake, Sunao Sugiyama
 Author-email: dark_emulator@ipmu.jp
-License: UNKNOWN
-Description: # Dark Emulator
-        [![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/version.svg)](https://anaconda.org/nishimichi/dark_emulator)
-        [![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/latest_release_date.svg)](https://anaconda.org/nishimichi/dark_emulator)
-        [![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/license.svg)](https://anaconda.org/nishimichi/dark_emulator)
-        [![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/downloads.svg)](https://anaconda.org/nishimichi/dark_emulator)
-        
-        A repository for a cosmology tool `dark_emulator` to emulate halo clustering statistics. The code is developed based on Dark Quest simulation suite (https://darkquestcosmology.github.io/). The current version supports the halo mass function and two point correlation function (both halo-halo and halo-matter cross).
-        
-        ## Install
-        In order to install dark emulator package, use pip:
-        ```
-           pip install dark_emulator
-        ```
-        or use conda:
-        ```
-           conda install -c nishimichi dark_emulator
-        ```
-        If the above does not work for you, you may download the source files from this repository and install via
-        ```
-        python -m pip install -e .
-        ```
-        after moving to the top directory of the source tree.
-        In that case, you need to install `pyfftlog`, `george` (a software package for the Gaussian process) and colossus
-        ```
-        conda install -c conda-forge george
-        conda install -c conda-forge pyfftlog
-        pip install colossus
-        ```
-        
-        ## Usage
-        You can then check how Dark Emulator works by running a tutorial notebook at
-        ```
-        docs/tutorial.ipynb
-        docs/tutorial-hod.ipynb
-        ```
-        See also the documentation on [readthedocs](https://dark-emulator.readthedocs.io/en/latest/).
-        
-        ## Code Paper
-        The main reference for our halo emulation strategy is: "Dark Quest. I. Fast and Accurate Emulation of Halo Clustering Statistics and Its Application to Galaxy Clustering", by T. Nishimichi et al., [ApJ 884, 29 (2019)](https://iopscience.iop.org/article/10.3847/1538-4357/ab3719/meta), [arXiv:1811.09504](https://arxiv.org/abs/1811.09504). Please also refer to the paper "Cosmological inference from emulator based halo model I: Validation tests with HSC and SDSS mock catalogs", by H. Miyatake et al.,  [arXiv:2101.00113](https://arxiv.org/abs/2101.00113) for the implementation and performance of the halo-galaxy connection routines.
-        
-        
 Keywords: cosmology,large scale structure,halo,gaussian process,machine learning
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Dark Emulator
+[![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/version.svg)](https://anaconda.org/nishimichi/dark_emulator)
+[![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/latest_release_date.svg)](https://anaconda.org/nishimichi/dark_emulator)
+[![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/license.svg)](https://anaconda.org/nishimichi/dark_emulator)
+[![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/downloads.svg)](https://anaconda.org/nishimichi/dark_emulator)
+
+A repository for a cosmology tool `dark_emulator` to emulate halo clustering statistics. The code is developed based on Dark Quest simulation suite (https://darkquestcosmology.github.io/). The current version supports the halo mass function and two point correlation function (both halo-halo and halo-matter cross).
+
+## Install
+In order to install dark emulator package, use pip:
+```
+   pip install dark_emulator
+```
+or use conda:
+```
+   conda install -c nishimichi dark_emulator
+```
+If the above does not work for you, you may download the source files from this repository and install via
+```
+python -m pip install -e .
+```
+after moving to the top directory of the source tree.
+In that case, you need to install `george` (a software package for the Gaussian process) and colossus
+```
+conda install -c conda-forge george
+pip install colossus
+```
+From version 1.1.0, `dark_emulator` uses FFTLog implementation by [Fang et al (2019); arXiv:1911.11947](https://arxiv.org/abs/1911.11947).
+
+## Usage
+You can then check how Dark Emulator works by running a tutorial notebook at
+```
+docs/tutorial.ipynb
+docs/tutorial-hod.ipynb
+```
+See also the documentation on [readthedocs](https://dark-emulator.readthedocs.io/en/latest/).
+
+## Code Paper
+The main reference for our halo emulation strategy is: "Dark Quest. I. Fast and Accurate Emulation of Halo Clustering Statistics and Its Application to Galaxy Clustering", by T. Nishimichi et al., [ApJ 884, 29 (2019)](https://iopscience.iop.org/article/10.3847/1538-4357/ab3719/meta), [arXiv:1811.09504](https://arxiv.org/abs/1811.09504). Please also refer to the paper "Cosmological inference from emulator based halo model I: Validation tests with HSC and SDSS mock catalogs", by H. Miyatake et al.,  [arXiv:2101.00113](https://arxiv.org/abs/2101.00113) for the implementation and performance of the halo-galaxy connection routines.
+
```

### Comparing `dark_emulator-1.0.23/README.md` & `dark_emulator-1.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,20 @@
    conda install -c nishimichi dark_emulator
 ```
 If the above does not work for you, you may download the source files from this repository and install via
 ```
 python -m pip install -e .
 ```
 after moving to the top directory of the source tree.
-In that case, you need to install `pyfftlog`, `george` (a software package for the Gaussian process) and colossus
+In that case, you need to install `george` (a software package for the Gaussian process) and colossus
 ```
 conda install -c conda-forge george
-conda install -c conda-forge pyfftlog
 pip install colossus
 ```
+From version 1.1.0, `dark_emulator` uses FFTLog implementation by [Fang et al (2019); arXiv:1911.11947](https://arxiv.org/abs/1911.11947).
 
 ## Usage
 You can then check how Dark Emulator works by running a tutorial notebook at
 ```
 docs/tutorial.ipynb
 docs/tutorial-hod.ipynb
 ```
```

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/auto.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import numpy as np
+import logging
 from scipy.interpolate import InterpolatedUnivariateSpline as ius
 from scipy.interpolate import RectBivariateSpline as rbs
 from scipy import ndimage
 from . import gp
 
 
 class auto_gp:
 
     def __init__(self):
-        print('initialize auto-correlation emulator')
+        logging.info('initialize auto-correlation emulator')
         self.logrscale = np.load(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/xiauto/loge_xs.npy')
         self.xdata = np.loadtxt(os.path.dirname(
             os.path.abspath(__file__)) + '/../data/params_80models.dat')
         self.ydata = np.load(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/xiauto/coeff_all.npy')
         self.eigdata = np.load(os.path.dirname(os.path.abspath(
```

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/cosmo_util.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/cosmo_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import numpy as np
+import logging
 from scipy import integrate
 from scipy.misc import derivative
 from collections import OrderedDict
 import logging
 
 cosm_range = OrderedDict((["omegab", [0.0211375, 0.0233625]],
                           ["omegac", [0.10782, 0.13178]],
@@ -63,15 +64,15 @@
 
 class cosmo_class:
     cparam = np.array([0.02225, 0.1198, 0.6844, 3.094,
                        0.9645, -1.]).reshape(1, 6)
     rho_cr = 2.77536627e11  # [M_sun/h] / [Mpc/h]^3\n"
 
     def __init__(self):
-        print('initialize cosmo_class')
+        logging.info('initialize cosmo_class')
         self.cpara_list = np.loadtxt(os.path.dirname(os.path.abspath(
             __file__)) + '/../data/params.dat')[:, [0, 1, 2, 4, 5, 6]]
         self.ascale_list = np.loadtxt(os.path.dirname(
             os.path.abspath(__file__)) + '/../data/scales.dat')
 
     def set_cosmology_predefined(self, i):
         self.set_cosmology(self.cpara_list[i, ])
@@ -89,15 +90,15 @@
         return 1./self.ascale_list[i] - 1.
 
     def set_cosmology(self, cparam_in):
         try:
             test_cosm_range(cparam_in)
             self.cparam = cparam_in.reshape(1, 6)
         except:
-            print('cosmological parameter out of supported range!')
+            logging.info('cosmological parameter out of supported range!')
 
     def get_cosmology(self):
         return self.cparam
 
     def get_comoving_distance(self, z):
         if isinstance(z, np.ndarray) or isinstance(z, list):
             chi = np.zeros(len(z))
```

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/cross.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/cross.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import numpy as np
+import logging
 from scipy.interpolate import InterpolatedUnivariateSpline as ius
 from scipy.interpolate import RectBivariateSpline as rbs
 from scipy import ndimage
 from . import gp
 
 
 class cross_gp:
 
     def __init__(self):
-        print('initialize cross-correlation emulator')
+        logging.info('initialize cross-correlation emulator')
         self.logrscale = np.load(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/xicross/loge_xs.npy')
         self.rscale = np.exp(self.logrscale)
         self.xdata = np.loadtxt(os.path.dirname(
             os.path.abspath(__file__)) + '/../data/params_80models.dat')
         self.ydata = np.load(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/xicross/coeff_all.npy')
```

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/de_interface.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/de_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .cosmo_util import constants
 from .pklin import pklin_gp
 from .xinl import xinl_gp
 from .gamma1 import gamma1_gp
 from .cross import cross_gp
 from .auto import auto_gp
 from .hmf import hmf_gp
-from .. import pyfftlog_interface
+from .. import fftlog
 import numpy as np
 from scipy.interpolate import InterpolatedUnivariateSpline as iuspline
 from scipy import integrate
 
 
 class base_class(object):
     """base_class
@@ -179,19 +179,24 @@
 
             Args:
                 xs (numpy array): Separations in :math:`[h^{-1}\mathrm{Mpc}]`
 
             Returns:
                 numpy array: Correlation function at separations given in the argument xs.
         """
-        ks = np.logspace(-3, 3, 300)
-        return pyfftlog_interface.pk2xi_pyfftlog(iuspline(ks, self.pkL.get(ks)))(xs)
+        ks = np.logspace(-5, 2, 1024)
+        pk = self.pkL.get(ks)
+        r, xi = fftlog.pk2xi(ks, pk, 1.01, N_extrap_low=1024, N_extrap_high=2014)
+        return iuspline(r, xi)(xs)
 
     def _get_xinl_tree(self, xs, redshift):
-        return pyfftlog_interface.pk2xi_pyfftlog(self._get_pkmatter_tree_spline(redshift))(xs)
+        ks = np.logspace(-5, 2, 300)
+        pk = self._get_pkmatter_tree_spline(redshift)(ks)
+        r, xi = fftlog.pk2xi(ks, pk, 1.01)
+        return iuspline(r, xi)(xs)
 
     def _get_xinl_direct(self, xs, z):
         return self.xiNL.get(xs, z)
 
     def get_xinl(self, xs, redshift):
         """get_xinl
 
@@ -218,15 +223,16 @@
                 z (float): redshift
 
             Returns:
                 numpy array: Nonlinear matter power spectrum at wavenumbers given in the argument k.
         """
         xs = np.logspace(-3, 3, 2000)
         xinl = self.get_xinl(xs, z)
-        return pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs, xinl))(k)
+        ks, pk = fftlog.xi2pk(xs, xinl, 1.01, N_extrap_low=1024)
+        return iuspline(ks, pk)(k)
 
     def get_pklin(self, k):
         """get_pklin
 
             Compute the linear matter power spectrum at z=0.
 
             Args:
@@ -258,15 +264,17 @@
 
     def _get_xiauto_tree(self, xs, logdens1, logdens2, redshift):
         ks = np.logspace(-3, 3, 2000)
         g1 = self.g1.get(ks, redshift, logdens1)
         g2 = self.g1.get(ks, redshift, logdens2)
         pm_lin = self.get_pklin(ks)
         ph_tree = g1 * g2 * pm_lin
-        return pyfftlog_interface.pk2xi_pyfftlog(iuspline(ks, ph_tree))(xs)
+        
+        x, xi = fftlog.pk2xi(ks, ph_tree, 1.01, N_extrap_low=1024)
+        return iuspline(x, xi)(xs)
 
     def _get_xiauto_direct(self, xs, logdens1, logdens2, redshift):
         return self.xi_auto.get(xs, redshift, logdens1, logdens2)
 
     def get_xiauto(self, xs, logdens1, logdens2, redshift):
         """get_xiauto
 
@@ -391,15 +399,18 @@
         pm_lin = self.get_pklin(ks)
         ph_tree = g1 * g2 * pm_lin
         return ph_tree
 
     def _get_phh_direct(self,ks,logdens1,logdens2,redshift):
         xs = np.logspace(-3,3,4000)
         xihh = self.xi_auto.get(xs,redshift,logdens1,logdens2)
-        return pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs,xihh))(ks)
+        
+        k, pk = fftlog.xi2pk(xs, xihh, 1.01)
+        
+        return iuspline(k, pk)(ks)
 
     def get_phh(self,ks,logdens1,logdens2,redshift):
         """get_phh
 
             Compute the halo-halo power spectrum :math:`P_{hh}(k;n_1,n_2)` between 2 mass threshold halo samples specified by the corresponding cumulative number densities.
 
             Args:
@@ -422,22 +433,26 @@
                 xi_tot = xi_dir * np.exp(-(xs/rswitch)**4) + xi_tree * (1-np.exp(-(xs/rswitch)**4))
         elif logdens1 < -5.75 and logdens2 >= -5.75:
                 xi_dir = self._get_xiauto_direct(xs,-5.75,logdens2,redshift) * self.g1.bias_ratio(redshift,logdens1)
                 xi_tot = xi_dir * np.exp(-(xs/rswitch)**4) + xi_tree * (1-np.exp(-(xs/rswitch)**4))
         else:
                 xi_dir = self._get_xiauto_direct(xs,-5.75,-5.75,redshift) * self.g1.bias_ratio(redshift,logdens1)*self.g1.bias_ratio(redshift,logdens2)
                 xi_tot = xi_dir * np.exp(-(xs/rswitch)**4) + xi_tree * (1-np.exp(-(xs/rswitch)**4))
-        return pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs,xi_tot))(ks)
+        
+        k, pk = fftlog.xi2pk(xs, xi_tot, 1.01)
+        return iuspline(k, pk)(ks)
 
     def _get_phh_tree_cut(self,ks,logdens1,logdens2,redshift):
         xs = np.logspace(-3,3,4000)
         xi_tree = self._get_xiauto_tree(xs,logdens1,logdens2,redshift)
         rswitch = min(60.,0.5 * self.cosmo.get_BAO_approx())
         xi_tot = xi_tree * (1-np.exp(-(xs/rswitch)**4))
-        return pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs,xi_tot))(ks)
+
+        k, pk = fftlog.xi2pk(xs, xi_tot, 1.01)
+        return iuspline(k, pk)(ks)
 
     def _get_phh_direct_cut(self,ks,logdens1,logdens2,redshift):
         xs = np.logspace(-3,3,4000)
         rswitch = min(60.,0.5 * self.cosmo.get_BAO_approx())
         if logdens1 >= -5.75 and logdens2 >= -5.75:
                 xi_dir = self._get_xiauto_direct(xs,logdens1,logdens2,redshift)
                 xi_tot = xi_dir * np.exp(-(xs/rswitch)**4)
@@ -446,15 +461,16 @@
                 xi_tot = xi_dir * np.exp(-(xs/rswitch)**4)
         elif logdens1 < -5.75 and logdens2 >= -5.75:
                 xi_dir = self._get_xiauto_direct(xs,-5.75,logdens2,redshift) * self.g1.bias_ratio(redshift,logdens1)
                 xi_tot = xi_dir * np.exp(-(xs/rswitch)**4)
         else:
                 xi_dir = self._get_xiauto_direct(xs,-5.75,-5.75,redshift) * self.g1.bias_ratio(redshift,logdens1)*self.g1.bias_ratio(redshift,logdens2)
                 xi_tot = xi_dir * np.exp(-(xs/rswitch)**4)
-        return pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs,xi_tot))(ks)
+        k, pk = fftlog.xi2pk(xs, xi_tot, 1.01)
+        return iuspline(k, pk)(ks)
 
 
     def get_phh_massthreshold(self,ks,Mthre,redshift):
         """get_phh_massthreshold
 
             Compute the halo-halo auto power spectrum :math:`P_{hh}(k;>M_\mathrm{th})` for a mass threshold halo sample.
 
@@ -513,18 +529,21 @@
                 logdens1 (float): Logarithm of the cumulative halo number density of the first halo sample taken from the most massive, :math:`\log_{10}[n_1/(h^{-1}\mathrm{Mpc})^3]`
                 logdens2 (float): Logarithm of the cumulative halo number density of the second halo sample taken from the most massive, :math:`\log_{10}[n_2/(h^{-1}\mathrm{Mpc})^3]`
                 redshift (float): redshift at which the power spectrum is evaluated
 
             Returns:
                 numpy array: projected halo correlation function in :math:`[h^{-1}\mathrm{Mpc}]`
         """
-        xs = np.logspace(-3, 3, 1000)
+        xs = np.logspace(-3, 3.0, 2048)
         xi_auto = self.get_xiauto(xs, logdens1, logdens2, redshift)
-        pk_spl = pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs, xi_auto))
-        return pyfftlog_interface.pk2xiproj_J0_pyfftlog(pk_spl, logkmin=-3.0, logkmax=3.0)(R2d)
+
+        k, pk = fftlog.xi2pk(xs, xi_auto, 1.01, N_extrap_high=1024)
+        
+        rp, wp = fftlog.pk2wp(k, pk, 1.01, N_extrap_low=2024)
+        return iuspline(rp, wp)(R2d)
 
     def get_wauto_cut(self, R2d, logdens1, logdens2, redshift, pimax, integration="quad"):
         """get_wauto_cut
 
             Compute the projected halo-halo correlation function :math:`w_{hh}(R;n_1,n_2)` for 2 mass threshold halo samples specified by the corresponding cumulative number densities.
             Unlike get_wauto, this function considers a finite width for the radial integration, from :math:`-\pi_\mathrm{max}` to :math:`\pi_\mathrm{max}`.
 
@@ -690,17 +709,21 @@
 
     def _get_pkcross_tree_spline(self, logdens, redshift):
         ks = np.logspace(-3, 3, 2000)
         g1 = self.g1.get(ks, redshift, logdens)
         g1_dm = self.g1.get_dm(ks, redshift)
         pm_lin = self.get_pklin(ks)
         return iuspline(ks, g1*g1_dm * pm_lin)
-
+        
     def _get_xicross_tree(self, xs, logdens, redshift):
-        return pyfftlog_interface.pk2xi_pyfftlog(self._get_pkcross_tree_spline(logdens, redshift))(xs)
+        ks = np.logspace(-4, 4, 1024)
+        pk = self._get_pkcross_tree_spline(logdens, redshift)(ks)
+
+        x, xi = fftlog.pk2xi(ks, pk, 1.01, N_extrap_low=1024)
+        return iuspline(x, xi)(xs)
 
     def _get_xicross_direct(self, xs, logdens, redshift):
         return self.xi_cross.get(xs, redshift, logdens)
 
     def get_xicross(self, xs, logdens, redshift):
         """get_xicross
 
@@ -760,15 +783,17 @@
         g1 = self.g1.get(ks,redshift,logdens)
         g1_dm = self.g1.get_dm(ks,redshift)
         pm_lin = self.get_pklin(ks)
         return g1*g1_dm * pm_lin
 
     def _get_phm_direct(self,ks,logdens,redshift):
         xs = np.logspace(-3,3,2000)
-        return pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs,self.xi_cross.get(xs,redshift,logdens)))(ks)
+        xi = self.xi_cross.get(xs,redshift,logdens)
+        k, pk = fftlog.xi2pk(xs, xi, 1.01, N_extrap_low=1024)
+        return iuspline(k, pk)(ks)
 
     def get_phm(self,ks,logdens,redshift):
         """get_phm
 
         Compute the halo-matter cross power spectrum :math:`P_{hm}(k;n_h)` for a mass threshold halo sample specified by the corresponding cumulative number density.
 
         Args:
@@ -780,29 +805,35 @@
             numpy array: Halo-matter cross power spectrum in :math:`[(h^{-1}\mathrm{Mpc})^{3}]`
         """
         xs = np.logspace(-4,3,4000)
         xi_dir = self._get_xicross_direct(xs,logdens,redshift)
         xi_tree = self._get_xicross_tree(xs,logdens,redshift)
         rswitch = min(60.,0.5 * self.cosmo.get_BAO_approx())
         xi = xi_dir * np.exp(-(xs/rswitch)**4) + xi_tree * (1-np.exp(-(xs/rswitch)**4))
-        return pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs,xi),logrmin = -4.0, logrmax = 3.0)(ks)
+
+        k, pk = fftlog.xi2pk(xs, xi, 1.01, N_extrap_high=1024)
+        return iuspline(k, pk)(ks)
 
     def _get_phm_tree_cut(self,ks,logdens,redshift):
         xs = np.logspace(-4,3,4000)
         xi_tree = self._get_xicross_tree(xs,logdens,redshift)
         rswitch = min(60.,0.5 * self.cosmo.get_BAO_approx())
         xi = xi_tree * (1-np.exp(-(xs/rswitch)**4))
-        return pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs,xi),logrmin = -4.0, logrmax = 3.0)(ks)
+
+        k, pk = fftlog.xi2pk(xs, xi, 1.01)
+        return iuspline(k, pk)(ks)
 
     def _get_phm_direct_cut(self,ks,logdens,redshift):
         xs = np.logspace(-4,3,4000)
         xi_dir = self._get_xicross_direct(xs,logdens,redshift)
         rswitch = min(60.,0.5 * self.cosmo.get_BAO_approx())
         xi = xi_dir * np.exp(-(xs/rswitch)**4)
-        return pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs,xi),logrmin = -4.0, logrmax = 3.0)(ks)
+
+        k, pk = fftlog.xi2pk(xs, xi, 1.01)
+        return iuspline(k, pk)(ks)
 
     def get_phm_massthreshold(self,ks,Mthre,redshift):
         """get_phm_massthreshold
 
         Compute the halo-matter cross power spectrum :math:`P_{hm}(k;>M_\mathrm{th})` for a mass threshold halo sample.
 
         Args:
@@ -834,21 +865,26 @@
         logdensp = np.log10(self.mass_to_dens(Mp,redshift))
         logdensm = np.log10(self.mass_to_dens(Mm,redshift))
         pip = self.get_phm(ks,logdensp,redshift)
         pim = self.get_phm(ks,logdensm,redshift)
         return (pim * 10**logdensm - pip * 10**logdensp) / (10**logdensm - 10**logdensp)
 
     def _get_DeltaSigma_tree(self, R2d, logdens, redshift):
-        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * pyfftlog_interface.pk2xiproj_J2_pyfftlog(self._get_pkcross_tree_spline(logdens, redshift))(R2d)
+        k = np.logspace(-5, 5, 1024)
+        pk = self._get_pkcross_tree_spline(logdens, redshift)(k)
+
+        rp, dwp = fftlog.pk2dwp(k, pk, 1.01)
+        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * iuspline(rp, dwp)(R2d)
 
     def _get_DeltaSigma_direct(self, R2d, logdens, redshift):
         xs = np.logspace(-3, 3, 2000)
         xi = self._get_xicross_direct(xs, logdens, redshift)
-        pk_spl = pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs, xi))
-        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * pyfftlog_interface.pk2xiproj_J2_pyfftlog(pk_spl)(R2d)
+        k, pk = fftlog.xi2pk(xs, xi, 1.01)
+        rp, dwp = fftlog.pk2dwp(k, pk, 1.01)
+        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * iuspline(rp, dwp)(R2d)
 
     def get_DeltaSigma(self, R2d, logdens, redshift):
         """get_DeltaSigma
 
         Compute the halo-galaxy lensing signal, the excess surface mass density, :math:`\Delta\Sigma(R;n_h)`, for a mass threshold halo sample specified by the corresponding cumulative number density.
 
 
@@ -858,16 +894,19 @@
             redshift (float): redshift at which the lens halos are located
 
         Returns:
             numpy array: excess surface mass density in :math:`[h M_\odot \mathrm{pc}^{-2}]`
         """
         xs = np.logspace(-3, 3, 2000)
         xi_tot = self.get_xicross(xs, logdens, redshift)
-        pk_spl = pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs, xi_tot))
-        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * pyfftlog_interface.pk2xiproj_J2_pyfftlog(pk_spl)(R2d)
+
+        k, pk = fftlog.xi2pk(xs, xi_tot, 1.01)
+        
+        rp, dwp = fftlog.pk2dwp(k, pk, 1.01)
+        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * iuspline(rp, dwp)(R2d)
 
     def get_DeltaSigma_massthreshold(self, R2d, Mthre, redshift):
         """get_DeltaSigma_massthreshold
 
         Compute the halo-galaxy lensing signal, the excess surface mass density, :math:`\Delta\Sigma(R;>M_\mathrm{th})`, for a mass threshold halo sample.
 
         Args:
@@ -899,21 +938,28 @@
         logdensp = np.log10(self.mass_to_dens(Mp, redshift))
         logdensm = np.log10(self.mass_to_dens(Mm, redshift))
         DSp = self.get_DeltaSigma(R2d, logdensp, redshift)
         DSm = self.get_DeltaSigma(R2d, logdensm, redshift)
         return (DSm * 10**logdensm - DSp * 10**logdensp) / (10**logdensm - 10**logdensp)
 
     def _get_Sigma_tree(self, R2d, logdens, redshift):
-        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * pyfftlog_interface.pk2xiproj_J0_pyfftlog(self._get_pkcross_tree_spline(logdens, redshift))(R2d)
+        k = np.logspace(-5,5,1024)
+        pk = self._get_pkcross_tree_spline(logdens, redshift)(k)
+
+        rp, wp = fftlog.pk2wp(k, pk, 1.01)
+        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * iuspline(rp, wp)(R2d)
 
     def _get_Sigma_direct(self, R2d, logdens, redshift):
-        xs = np.logspace(-3, 3, 2000)
+        xs = np.logspace(-2, 2, 2000)
         xi = self._get_xicross_direct(xs, logdens, redshift)
-        pk_spl = pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs, xi))
-        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * pyfftlog_interface.pk2xiproj_J0_pyfftlog(pk_spl)(R2d)
+
+        k, pk = fftlog.xi2pk(xs, xi, 1.01)
+        
+        rp, wp = fftlog.pk2wp(k, pk, 1.01, N_extrap_low=2048)
+        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * iuspline(rp, wp)(R2d)
 
     def get_Sigma(self, R2d, logdens, redshift):
         """get_Sigma
 
         Compute the surface mass density, :math:`\Sigma(R;n_h)`, for a mass threshold halo sample specified by the corresponding cumulative number density.
 
         Args:
@@ -921,17 +967,20 @@
             logdens (float): Logarithm of the cumulative halo number density taken from the most massive, :math:`\log_{10}[n_h/(h^{-1}\mathrm{Mpc})^3]`
             redshift (float): redshift at which the lens halos are located
 
         Returns:
             numpy array: surface mass density in :math:`[h M_\odot \mathrm{pc}^{-2}]`
         """
         xs = np.logspace(-3, 3, 2000)
-        xi_tot = self._get_xicross(xs, logdens, redshift)
-        pk_spl = pyfftlog_interface.xi2pk_pyfftlog(iuspline(xs, xi_tot))
-        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * pyfftlog_interface.pk2xiproj_J0_pyfftlog(pk_spl)(R2d)
+        xi_tot = self.get_xicross(xs, logdens, redshift)
+        
+        k, pk = fftlog.xi2pk(xs, xi_tot, 1.01, N_extrap_high=1024)
+        
+        rp, wp = fftlog.pk2wp(k, pk, 1.01,N_extrap_low=2048)#,c_window_width=0)#,N_extrap_low=2048,c_window_width=0)#, N_extrap_low=2048, c_window_width=0.3)
+        return self.cosmo.get_Omega0() * self.cosmo.rho_cr / 1e12 * iuspline(rp, wp)(R2d)
 
     def get_Sigma_massthreshold(self, R2d, Mthre, redshift):
         """get_Sigma_massthreshold
 
         Compute the surface mass density, :math:`\Sigma(R;>M_\mathrm{th})`, for a mass threshold halo sample.
 
         Args:
```

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/gamma1.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/gamma1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import numpy as np
+import logging
 from scipy.interpolate import InterpolatedUnivariateSpline as ius
 from scipy.interpolate import RectBivariateSpline as rbs
 from .sigmad import sigmad_gp
 from .import gp
 
 
 class gamma1_gp:
 
     def __init__(self):
-        print('initialize propagator emulator')
+        logging.info('initialize propagator emulator')
         self.xdata = np.loadtxt(os.path.dirname(
             os.path.abspath(__file__)) + '/../data/params_80models.dat')
         self.ydata = np.load(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/gamma1/coeff_all.npy')
         self.eigdata = np.load(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/gamma1/pca_eigvec.npy')
         self.yerr = np.load(os.path.dirname(os.path.abspath(
@@ -34,15 +35,15 @@
         self.ascale_list = np.loadtxt(os.path.dirname(
             os.path.abspath(__file__)) + '/../data/scales.dat')
         self.redshift_list = 1./self.ascale_list-1.
 
         self.sd = sigmad_gp()
 
     # def reload(self):
-    # 	print 'reloading data files for gamma1_gp object...'
+    # 	logging.info("reloading data files for gamma1_gp object...")
     # 	self.dout = np.load(os.path.dirname(__file__) + '/../learned_data/gamma1/gamma1_dm_dout.npy')
     # 	self.gp = joblib.load(os.path.dirname(__file__) + '/../learned_data/gamma1/gamma1_dm_fit_gps.pkl')
     # 	self.dout_h = np.load(os.path.dirname(__file__) + '/../learned_data/gamma1/gamma1_dout.npy')
     # 	self.gp_h = joblib.load(os.path.dirname(__file__) + '/../learned_data/gamma1/gamma1_fit_gps.pkl')
 
     def model_curve(x, a, b, c):
         return (a+b*x**2+c*x**4)*np.exp(-x**2/2.)
```

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/gp/gp6d.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/gp/gp6d.py`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/hmf.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/hmf.py`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/pklin.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/pklin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import numpy as np
+import logging
 from scipy.interpolate import InterpolatedUnivariateSpline as ius
 from scipy import integrate
 import george
 from george import kernels
 
 
 class pklin_gp:
     def __init__(self):
-        print('Initialize pklin emulator')
+        logging.info('Initialize pklin emulator')
         self.klist = np.logspace(-3, 1, 200)
         self.logklist = np.log(self.klist)
         self.cosmos = np.loadtxt(os.path.dirname(
             os.path.abspath(__file__)) + '/../data/cparams_3d.dat')
         self.ydata = np.loadtxt(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/pklin/coeff_all.dat')
         self.eigdata = np.loadtxt(os.path.dirname(os.path.abspath(
@@ -34,15 +35,15 @@
                     kernels.Matern52Kernel(
                         np.ones(3), ndim=3) + kernels.ConstantKernel(1e-4, ndim=3)
             elif self.ktypes[i] == 6:
                 kernel = 1. * \
                     kernels.ExpSquaredKernel(
                         np.ones(3), ndim=3) + kernels.ConstantKernel(1e-4, ndim=3)
             else:
-                print('kernel type 6 and 10 are the only supported types.')
+                logging.info('kernel type 6 and 10 are the only supported types.')
             gp = george.GP(kernel)
             gp.compute(self.cosmos[:800])
             gp.set_parameter_vector(self.gp_params[i])
             self.gps.append(gp)
 
     def set_cosmology(self, cosmo):
         cparams = cosmo.get_cosmology()
```

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/sigmaM.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/sigmaM.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import numpy as np
+import logging
 import george
 from george import kernels
 from scipy import integrate
 
 from scipy.interpolate import InterpolatedUnivariateSpline as ius
 
 
 class sigmaM_gp:
     def __init__(self):
-        print('Initialize sigmaM emulator')
+        logging.info('Initialize sigmaM emulator')
         self.Mlist = np.logspace(10, 16, 601)
         self.load_sigma_gp()
         self.As_fid = np.exp(3.094)
 
     def load_sigma_gp(self):
         self.cosmos = np.loadtxt(os.path.dirname(
             os.path.abspath(__file__)) + '/../data/cparams_4d.dat')
@@ -38,15 +39,15 @@
                     kernels.Matern52Kernel(
                         np.ones(4), ndim=4) + kernels.ConstantKernel(1e-4, ndim=4)
             elif self.ktypes[i] == 6:
                 kernel = 1. * \
                     kernels.ExpSquaredKernel(
                         np.ones(4), ndim=4) + kernels.ConstantKernel(1e-4, ndim=4)
             else:
-                print('kernel type 6 and 10 are the only supported types.')
+                logging.info('kernel type 6 and 10 are the only supported types.')
             gp = george.GP(kernel)
             gp.compute(self.cosmos[:800])
             gp.set_parameter_vector(self.gp_params[i])
             self.gps.append(gp)
 
     def set_cosmology(self, cosmo):
         cparams = cosmo.get_cosmology()
```

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/sigmad.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/sigmad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import numpy as np
+import logging
 import george
 from george import kernels
 from scipy import integrate
 
 
 class sigmad_gp:
     def __init__(self):
-        print('Initialize sigma_d emulator')
+        logging.info('Initialize sigma_d emulator')
         self.cosmos = np.loadtxt(os.path.dirname(
             os.path.abspath(__file__)) + '/../data/cparams_4d.dat')
         self.ydata = np.loadtxt(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/sigmad/coeff_all.dat')
         self.yavg = np.loadtxt(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/sigmad/sigd_avg.dat')
         self.ystd = np.loadtxt(os.path.dirname(os.path.abspath(
@@ -25,15 +26,15 @@
                 kernels.Matern52Kernel(np.ones(4), ndim=4) + \
                 kernels.ConstantKernel(1e-4, ndim=4)
         elif self.ktypes == 6:
             kernel = 1. * \
                 kernels.ExpSquaredKernel(
                     np.ones(4), ndim=4) + kernels.ConstantKernel(1e-4, ndim=4)
         else:
-            print('kernel type 6 and 10 are the only supported types.')
+            logging.info('kernel type 6 and 10 are the only supported types.')
         self.gp = george.GP(kernel)
         self.gp.compute(self.cosmos[:800])
         self.gp.set_parameter_vector(self.gp_params)
         self.As_fid = np.exp(3.094)
 
     def get(self, cosmo):
         cparams = cosmo.get_cosmology()[0]
```

### Comparing `dark_emulator-1.0.23/dark_emulator/darkemu/xinl.py` & `dark_emulator-1.1.1/dark_emulator/darkemu/xinl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import numpy as np
+import logging
 from scipy import interpolate
 from scipy.interpolate import InterpolatedUnivariateSpline as ius
 from scipy.interpolate import RectBivariateSpline as rbs
 from . import gp
 
 
 class xinl_gp:
 
     def __init__(self):
-        print('initialize xinl emulator')
+        logging.info('initialize xinl emulator')
         # self.logxscale = np.log(np.load(os.path.dirname(os.path.abspath(__file__)) + '/../learned_data/ximnl/xs.npy'))
         self.xscale = np.logspace(-2, 2, 41)
         self.logxscale = np.log(self.xscale)
         self.xdata = np.loadtxt(os.path.dirname(os.path.abspath(
             __file__)) + '/../data/params.dat')[list(range(1))+list(range(61, 101))][:, [0, 1, 2, 4, 5, 6]]
         self.ydata = np.load(os.path.dirname(os.path.abspath(
             __file__)) + '/../learned_data/xinl/coeff_all.npy')
```

### Comparing `dark_emulator-1.0.23/dark_emulator/data/cparams_3d.dat` & `dark_emulator-1.1.1/dark_emulator/data/cparams_3d.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/data/cparams_4d.dat` & `dark_emulator-1.1.1/dark_emulator/data/cparams_4d.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/data/params.dat` & `dark_emulator-1.1.1/dark_emulator/data/params.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/data/params_40x10.dat` & `dark_emulator-1.1.1/dark_emulator/data/params_40x10.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/data/params_80models.dat` & `dark_emulator-1.1.1/dark_emulator/data/params_80models.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/coeff_all.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/coeff_all.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/gp6d_hyperparams.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/gp6d_hyperparams.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/pca_eigvec.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/pca_eigvec.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/gamma1/yerr.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/gamma1/yerr.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/gamma1_dm/coeff_all.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/gamma1_dm/coeff_all.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/gamma1_dm/pca_eigvec.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/gamma1_dm/pca_eigvec.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/gamma1_dm/yerr.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/gamma1_dm/yerr.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/hmf/coeff_all.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/hmf/coeff_all.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/hmf/gp6d_hyperparams.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/hmf/gp6d_hyperparams.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/hmf/pca_eigvec.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/hmf/pca_eigvec.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/hmf/yerr.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/hmf/yerr.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/pklin/coeff_all.dat` & `dark_emulator-1.1.1/dark_emulator/learned_data/pklin/coeff_all.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/pklin/gp_params.dat` & `dark_emulator-1.1.1/dark_emulator/learned_data/pklin/gp_params.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/pklin/pca_eigvec.dat` & `dark_emulator-1.1.1/dark_emulator/learned_data/pklin/pca_eigvec.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/pklin/pca_mean.dat` & `dark_emulator-1.1.1/dark_emulator/learned_data/pklin/pca_mean.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/coeff_all.dat` & `dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/coeff_all.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/gp_params.dat` & `dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/gp_params.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/pca_eigvec.dat` & `dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/pca_eigvec.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/sigmaM/pca_mean.dat` & `dark_emulator-1.1.1/dark_emulator/learned_data/sigmaM/pca_mean.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/sigmad/coeff_all.dat` & `dark_emulator-1.1.1/dark_emulator/learned_data/sigmad/coeff_all.dat`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/coeff_all.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/coeff_all.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/gp6d_hyperparams.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/gp6d_hyperparams.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/pca_eigvec.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/pca_eigvec.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xiauto/yerr.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xiauto/yerr.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xicross/coeff_all.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xicross/coeff_all.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xicross/gp6d_hyperparams.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xicross/gp6d_hyperparams.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xicross/loge_xs.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xicross/loge_xs.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xicross/pca_eigvec.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xicross/pca_eigvec.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xicross/yerr.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xicross/yerr.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xicross/ymeans.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xicross/ymeans.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xinl/coeff_all.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xinl/coeff_all.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xinl/gp6d_hyperparams.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xinl/gp6d_hyperparams.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xinl/pca_eigvec.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xinl/pca_eigvec.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/learned_data/xinl/yerr.npy` & `dark_emulator-1.1.1/dark_emulator/learned_data/xinl/yerr.npy`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/dark_emulator/model_hod/hod_interface.py` & `dark_emulator-1.1.1/dark_emulator/model_hod/hod_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 from ..darkemu.cross import cross_gp
 from ..darkemu.gamma1 import gamma1_gp
 from ..darkemu.xinl import xinl_gp
 from ..darkemu.pklin import pklin_gp
 from ..darkemu.cosmo_util import cosmo_class
 from scipy.interpolate import InterpolatedUnivariateSpline as ius
 from scipy.interpolate import RectBivariateSpline as rbs
+from scipy.integrate import simps
+from scipy.special import eval_legendre
 from scipy import integrate
 from scipy import special
 from scipy import ndimage
 from scipy import optimize
-from .. import pyfftlog_interface
+from .. import fftlog
 try:
     from colossus.cosmology import cosmology as colcosmology
     from colossus.halo import concentration
 except:
-    print('colossus is not installed.')
+    logging.warning('colossus is not installed.')
 
 
 path_baryon = os.path.dirname(__file__)
 path_baryon = os.path.join(path_baryon, "..", "baryon")
 sys.path.append(path_baryon)
 try:
     from wk_baryon import return_wk
@@ -59,61 +61,65 @@
        - **M_int_k** (*int*): Sampling in the integration across halo mass which sets :math:`2^{\mathrm{M\_int\_k}}` (default: 5).
        - **c-M_relation** (*str*): Concentration-mass relation used for satellite distribution when NFW is used (see ``set_galaxy()``; default: 'diemer15'). The concentration is internally computed using `colossus <https://bdiemer.bitbucket.io/colossus/>`_, and a user can use a model listed in ``concentration models`` in `this webpage <https://bdiemer.bitbucket.io/colossus/halo_concentration.html>`_.
 
        Args:
            config (dict): a dictionary to specify configurations
     """
     def __init__(self, config=None):
-        logging.basicConfig(level=logging.DEBUG)
+        #logging.basicConfig(level=logging.DEBUG)
         self.redshift = None
 
         # set up default config
         self.config = dict()
-        self.config["fft_num"] = 8 # Sunao : changed from 5 to 8 for fftlog in wp_2hcs, wp_2hss, xi_2hcs and xi_2hss to converge at -1.0 < log10(r) < 1.0.
+        self.config["fft_num"] = 1
+        #self.config["fft_logrmin_1h"] = -5.0
+        #self.config["fft_logrmax_1h"] = 3.0
+        #self.config["fft_logrmin_2h"] = -3.0
+        #self.config["fft_logrmax_2h"] = 3.0
         self.config["fft_logrmin_1h"] = -5.0
         self.config["fft_logrmax_1h"] = 3.0
         self.config["fft_logrmin_2h"] = -3.0
         self.config["fft_logrmax_2h"] = 3.0
         self.config["M_int_logMmin"] = 12.
         self.config["M_int_logMmax"] = 15.9
         self.config["M_int_k"] = 5
         self.config["M_int_algorithm"] = "romberg"
         #self.config["los_int_pi_max"] = None
         #self.config["los_int_algorithm"] = "trapz"
         self.config["c-M_relation"] = "diemer15"
         self.config["p_hm_apodization"] = None # apodization with the scale sigma_k=self.config["p_hm_apodization"]/R200 is applied for satelite distribution computed from emulator. See def _compute_p_hm_satdist_emu() for details
         # override if specified in input
         if config is not None:
-            for key in list(config.keys()):
-                self.config[key] = config[key]
+            self.config.update(config)
 
         # internal config parameters
         self.config["hmf_int_algorithm"] = "trapz"
 
         # set up variables shared with multiple methods
         self.Mh = np.logspace(
             self.config["M_int_logMmin"], self.config["M_int_logMmax"], 2**self.config["M_int_k"]+1)
         self.dlogMh = np.log(self.Mh[1]) - np.log(self.Mh[0])
 
-        self.fftlog_1h = pyfftlog_interface.fftlog(self.config['fft_num'], logrmin=self.config['fft_logrmin_1h'], logrmax=self.config['fft_logrmax_1h'], kr=1)
-        self.fftlog_2h = pyfftlog_interface.fftlog(self.config['fft_num'], logrmin=self.config['fft_logrmin_2h'], logrmax=self.config['fft_logrmax_2h'], kr=1)
+        self.fftlog_1h = fftlog.fftbase(self.config['fft_num'], self.config['fft_logrmin_1h'], self.config['fft_logrmax_1h'], kr=1)
+        self.fftlog_2h = fftlog.fftbase(self.config['fft_num'], self.config['fft_logrmin_2h'], self.config['fft_logrmax_2h'], kr=1)
 
         if self.config["M_int_algorithm"] == "romberg":
             self.do_integration = integrate.romb
         elif self.config["M_int_algorithm"] == "simpson":
             self.do_integration = integrate.simps
 
         self.k_1h_mat = np.tile(self.fftlog_1h.k, (len(self.Mh), 1))
         self.k_2h_mat = np.tile(self.fftlog_2h.k, (len(self.Mh), 1))
+        self.k_2h_mat = np.tile(self.fftlog_2h.k, (len(self.Mh), 1))
         self.Mh_mat = np.tile(self.Mh, (len(self.fftlog_2h.k), 1)).transpose()
 
         self.gparams = None
         self.initialized = False
         self.cparams_orig = np.zeros((1, 6))
-        super(darkemu_x_hod, self).__init__()
+        super().__init__()
 
     # The following flags tell if dndM and power spectrum should be recomputed when cosmology or redshift is varied.
     def _initialize_cosmology_computation_flags(self):
         self.dndM_spl_computed = False
         self.d_to_m_interp_computed = False
         self.dndM_computed = False
         self.p_hh_computed = False
@@ -135,21 +141,21 @@
 
             self.cparams_orig = np.copy(cparams)
             if self.do_linear_correction:
                 cparams = cparams_tmp
                 logging.info("%s is out of the supported range. Instaead use %s and apply linear correction later." % (
                     self.cparams_orig, cparams))
                 # compute pklin for cparams_orig here
-                super(darkemu_x_hod, self).set_cosmology(self.cparams_orig)
+                super().set_cosmology(self.cparams_orig)
                 self.pm_lin_k_1h_out_of_range = self.get_pklin(self.fftlog_1h.k)
                 self.pm_lin_k_2h_out_of_range = self.get_pklin(self.fftlog_2h.k)
                 self.cosmo_orig = copy.deepcopy(self.cosmo)
                 self.massfunc_cosmo_edge = hmf_gp()
                 self.massfunc_cosmo_edge.set_cosmology(self.cosmo)
-            super(darkemu_x_hod, self).set_cosmology(cparams)
+            super().set_cosmology(cparams)
             if self.do_linear_correction:
                 self.massfunc.set_cosmology(self.cosmo_orig)
             self.rho_m = (1. - cparams[0][2])*rho_cr
             self.R200 = (3*self.Mh/(4.*np.pi*self.rho_m)/200.)**(1./3.)
             self.R200_mat = np.tile(self.R200, (len(self.fftlog_2h.k), 1)).transpose()
             self._initialize_cosmology_computation_flags()
             self.initialized = True
@@ -406,15 +412,15 @@
         xi_hh = xi_dir_mass_r_resampled * \
             connection_factor_1 + xi_tree * connection_factor_2
         p_hh = np.zeros((len(logdens_g1), len(logdens_g1), len(self.fftlog_2h.k)))
         for i in range(len(logdens_g1)):
             for j in range(len(logdens_g1)):
                 if logdens_g1[i] < logdens_g1[j]:
                     continue
-                p_hh[i, j] = self.fftlog_2h.xi2pk(xi_hh[i, j])
+                p_hh[i, j] = self.fftlog_2h.xi2pk(xi_hh[i, j])[1]
                 #p_hh[i, j] = fftLog.xi2pk_fftlog_array(
                 #    self.fftlog_2h.r, self.fftlog_2h.k, xi_hh[i, j], self.fftlog_2h.kr, self.fftlog_2h.dlnr)
                 if i != j:
                     p_hh[j, i] = p_hh[i, j]
 
         # interpolate phh along halo mass
         self.p_hh_spl = list()
@@ -498,23 +504,24 @@
                 ph_tree_pm = g_1p * g_2m * pm_lin
                 ph_tree_pp = g_1p * g_2p * pm_lin
                 numer = ph_tree_mm * dens_1m * dens_2m - ph_tree_mp * dens_1m * dens_2p - \
                     ph_tree_pm * dens_1p * dens_2m + ph_tree_pp * dens_1p * dens_2p
                 ph_tree = numer/denom
                 #p_hh_tree[i,j] = ph_tree
 
-                xi_tree = self.fftlog_2h.pk2xi(ph_tree)
+                xi_tree = fftlog.pk2xi(self.fftlog_2h.k, ph_tree, 1.01, N_extrap_low=1024)[1]
+                #xi_tree = self.fftlog_2h.pk2xi(ph_tree, N_extrap_high=0)[1]
                 #xi_tree = fftLog.pk2xi_fftlog_array(
                 #    self.k_2h, self.r_2h, ph_tree, self.kr, self.dlnk_2h)
                 xi_hh = xi_dir * connection_factor_1 + xi_tree * connection_factor_2
 
                 if self.do_linear_correction:
                     xi_hh *= bias_correction[i]*bias_correction[j]
 
-                p_hh[i, j] = self.fftlog_2h.xi2pk(xi_hh)
+                p_hh[i, j] = fftlog.xi2pk(self.fftlog_2h.k, xi_hh, 1.01, N_extrap_high=1024)[1]
                 #p_hh[i, j] = fftLog.xi2pk_fftlog_array(
                 #    self.r_2h, self.k_2h, xi_hh, self.kr, self.dlnr_2h)
                 if i != j:
                     p_hh[j, i] = p_hh[i, j]
                 k += 1
 
                 if self.do_linear_correction:
@@ -639,15 +646,15 @@
             # calculate xicross_tree
             phm_tree_m = g1m * g1_dm * pm_lin
             phm_tree_p = g1p * g1_dm * pm_lin
             phm_tree = (phm_tree_m * 10**logdensm -
                         phm_tree_p * 10**logdensp) / denom
             #import matplotlib.pyplot as plt
             #plt.semilogx(self.k_1h, g1p)
-            xi_hm_tree = self.fftlog_1h.pk2xi(phm_tree)
+            xi_hm_tree = self.fftlog_1h.pk2xi(phm_tree, N_extrap_high=0)[1]
             #xi_hm_tree = fftLog.pk2xi_fftlog_array(
             #    self.k_1h, self.r_1h, phm_tree, self.kr, self.dlnk_1h)
             xi_hm_tmp = xi_hm_dir * np.exp(-(self.fftlog_1h.r/rswitch)**4) + xi_hm_tree * (1-np.exp(-(self.fftlog_1h.r/rswitch)**4))
             if self.do_linear_correction:
                 xi_hm_tmp *= bias_correction[i]
             xi_hm_de.append(xi_hm_tmp)
 
@@ -664,15 +671,15 @@
         logdens = self.logdens
 
         if self.do_linear_correction:
             pm_lin = self.get_pklin(self.fftlog_1h.k)
 
         p_hm = np.zeros((len(logdens), len(self.fftlog_1h.k)))
         for i in range(len(logdens)):
-            p_hm[i] = self.fftlog_1h.xi2pk(self.xi_hm[i])
+            p_hm[i] = self.fftlog_1h.xi2pk(self.xi_hm[i], 1.01, N_extrap_high=1024)[1]
             #p_hm[i] = fftLog.xi2pk_fftlog_array(
             #    self.r_1h, self.k_1h, self.xi_hm[i], self.kr, self.dlnr_1h)
             if "baryon" in list(self.gparams.keys()):
                 baryonic_params = self.gparams["baryon"]
                 Mc = 10**baryonic_params[0]
                 beta = baryonic_params[1]
                 eta = baryonic_params[2]
@@ -701,15 +708,15 @@
             pm_lin = self.get_pklin(self.fftlog_1h.k)
 
         p_hm_dist = list()
         for i, _R200 in enumerate(self.R200):
             sel = (self.fftlog_1h.r > _R200)
             xi_hm_dist = np.copy(self.xi_hm[i])
             xi_hm_dist[sel] = 0.
-            p_hm_dist_tmp = self.fftlog_1h.xi2pk(xi_hm_dist)
+            p_hm_dist_tmp = self.fftlog_1h.xi2pk(xi_hm_dist, N_extrap_high=0)[1]
             #p_hm_dist_tmp = fftLog.xi2pk_fftlog_array(
             #    self.r_1h, self.k_1h, xi_hm_dist, self.kr, self.dlnr_1h)
             if self.do_linear_correction:
                 p_hm_dist_tmp *= (self.pm_lin_k_1h_out_of_range/pm_lin)
 
             # apodization
             if self.config["p_hm_apodization"] is not None:
@@ -725,44 +732,45 @@
                 4.*np.pi*norm_int_r**3*self.rho_m*(1.+xi_hm_dist_spline(norm_int_r)), dx=dlog_norm_int_r)
             p_hm_dist.append(p_hm_dist_tmp * self.rho_m/norm)
 
         self.p_hm_dist_1h = p_hm_dist
         self.p_hm_dist_2h = np.array(
             [ius(self.fftlog_1h.k, p_hm_dist[i], ext=3)(self.fftlog_2h.k) for i in range(len(self.Mh))])
 
-    def _concentration(self, M, z, model='diemer15'):
+    def _concentration(self, cosmo, M, z, model='diemer15'):
+        c200m = concentration.concentration(M, '200m', z, model=model)
+        return c200m
+
+    def _compute_p_hm_satdist_NFW(self, redshift):
+        R200 = (3*self._convert_dens_to_mass(10**np.array(self.xi_cross.logdens_list), redshift,
+                                    integration=self.config["hmf_int_algorithm"])/(4.*np.pi*self.rho_m)/200.)**(1./3.)
+
+        p_hm_dist = list()
+        if "sat_dist_Rc" in list(self.gparams.keys()):
+            Rc = self.gparams["sat_dist_Rc"]
+        else:
+            Rc = 1.0
+
         if self.do_linear_correction:
             cparam = self.cparams_orig[0]
         else:
             cparam = self.cosmo.get_cosmology()[0]
         Om0 = 1. - cparam[2]
         h = np.sqrt((cparam[0] + cparam[1] + 0.00064)/Om0)
         H0 = h*100
         Ob0 = cparam[0]/h**2
         rho_m = (1. - cparam[2])*rho_cr
         M_8mpc = 4.*np.pi/3.*8.**3*rho_m
         sigma8 = self.massfunc.sM.get_sigma(M_8mpc)
         ns = cparam[4]
         params = {'flat': True, 'H0': H0, 'Om0': Om0,
-                  'Ob0': Ob0, 'sigma8': sigma8, 'ns': ns, 'persistence': ''}
-        cosmo = colcosmology.setCosmology('myCosmo', params)
-        c200m = concentration.concentration(M, '200m', z, model=model)
-        return c200m
-
-    def _compute_p_hm_satdist_NFW(self, redshift):
-        R200 = (3*self._convert_dens_to_mass(10**np.array(self.xi_cross.logdens_list), redshift,
-                                    integration=self.config["hmf_int_algorithm"])/(4.*np.pi*self.rho_m)/200.)**(1./3.)
-
-        p_hm_dist = list()
-        if "sat_dist_Rc" in list(self.gparams.keys()):
-            Rc = self.gparams["sat_dist_Rc"]
-        else:
-            Rc = 1.0
+                  'Ob0': Ob0, 'sigma8': sigma8, 'ns': ns}
+        cosmo = colcosmology.setCosmology('myCosmo', params)        
         for i, (_M, _R200) in enumerate(zip(self.Mh, self.R200)):
-            c200 = self._concentration(_M, redshift, self.config["c-M_relation"])  # , model = 'duffy08')
+            c200 = self._concentration(cosmo, _M, redshift, self.config["c-M_relation"])  # , model = 'duffy08')
             if c200 == -1:
                 #raise RuntimeError("concentration cannot be computed at (M,z) = (%e,%e)" % (_M, redshift))
                 if self.do_linear_correction:
                     cparam = self.cparams_orig[0]
                 else:
                     cparam = self.cosmo.get_cosmology()[0]
                 logging.info("Colossus failed in computing concentration when cparams = %s, M=%s, and z=%s. Compute by diemer15 concentration implemented in Dark Emulator.", cparam, _M, redshift)
@@ -905,14 +913,16 @@
             self._compute_dndM(redshift)
         if self.HOD_computed == False:
             self._compute_HOD()
         if self.ng_computed == False:
             self._compute_ng()
         if self.p_hh_computed == False:
             self._compute_p_hh(redshift)
+        if self.p_hm_satdist_computed == False:
+            self._compute_p_hm_satdist(redshift)
 
         poff = self.gparams["poff"]
         Roff = self.gparams["Roff"]
 
         Hc_2h = self.Ncen_mat/self.ng * \
             (1. - poff + poff * np.exp(-0.5 * self.k_2h_mat**2*(Roff*self.R200_mat)**2))
         Hs_2h_mat = np.tile(self.Nsat, (len(self.fftlog_2h.k), 1)
@@ -1064,209 +1074,197 @@
         if self.redshift != redshift:
             self.redshift = redshift
             self._initialize_cosmology_computation_flags()
 
     def _get_effective_bias(self, redshift):
         return self._compute_effective_bias(redshift)
 
-    def _get_wp_rsd(self, rp, redshift, pimax):
-        # calculate xi
-        r_ref = np.logspace(-3, 3, 512)
-        xi = self.get_xi_gg(r_ref, redshift)
-        xi_spl = ius(r_ref, xi)
+    def _get_wp_rsd(self, rp, redshift, pimax, dlnrp = 0.):
+        # get xi, and multipoles, xi2, xi4
+        r = np.logspace(-1, 3.0, 1000)
+        xi0 = self.get_xi_gg(r, redshift)
+
+        p_tot_1h = 2.*self.p_1hcs + self.p_1hss
+        p_tot_2h = self.p_2hcc + 2.*self.p_2hcs + self.p_2hss
+        xi2 =-ius( self.fftlog_1h.r, fftlog.pk2xi(self.fftlog_1h.k, p_tot_1h, N_extrap_high=0, l=2)[1])(r) - ius( self.fftlog_2h.r, fftlog.pk2xi(self.fftlog_2h.k, p_tot_2h, N_extrap_high=0, l=2)[1] )(r)
+        xi4 = ius( self.fftlog_1h.r, fftlog.pk2xi(self.fftlog_1h.k, p_tot_1h, N_extrap_high=0, l=4)[1])(r) + ius( self.fftlog_2h.r, fftlog.pk2xi(self.fftlog_2h.k, p_tot_2h, N_extrap_high=0, l=4)[1] )(r)
 
         # calculate beta
         f = self.f_from_z(redshift)
-        #b = 2.118
         b = self._get_effective_bias(redshift)
         beta = f/b
 
-        n = 3
-        J_n = list()
-        for _r in r_ref:
-            t = np.linspace(1e-10, _r, 1024)
-            dt = t[1]-t[0]
-            J_n.append(1./_r**n*integrate.trapz(t**(n-1.)*xi_spl(t), dx=dt))
-        J_3 = np.array(J_n)
-
-        n = 5
-        J_n = list()
-        for _r in r_ref:
-            t = np.linspace(1e-10, _r, 1024)
-            dt = t[1]-t[0]
-            J_n.append(1./_r**n*integrate.trapz(t**(n-1.)*xi_spl(t), dx=dt))
-        J_5 = np.array(J_n)
-
-        xi_0 = (1.+2./3.*beta+1./5.*beta**2)*xi
-        xi_2 = (4./3.*beta+4./7.*beta**2)*(xi-3.*J_3)
-        xi_4 = 8./35.*beta**2*(xi+15./2.*J_3-35./2.*J_5)
-
-        r_pi = np.logspace(-3, np.log10(pimax), 512)
-        rp, r_pi = np.meshgrid(rp, r_pi, indexing='ij')
-
-        s = np.sqrt(rp**2+r_pi**2)
-
-        mu = r_pi/s
-
-        l0 = special.eval_legendre(0, mu)
-        l2 = special.eval_legendre(2, mu)
-        l4 = special.eval_legendre(4, mu)
-
-        xi_s = ius(r_ref, xi_0)(s)*l0 + ius(r_ref, xi_2)(s) * \
-            l2 + ius(r_ref, xi_4)(s)*l4
-
-        xi_s_spl = rbs(rp[:, 0], r_pi[0], xi_s)
-
-        wp = list()
-        for _r in rp:
-            wp.append(2*integrate.quad(lambda t: xi_s_spl(_r, t)
-                                       [0][0], 0, pimax, epsabs=1e-4)[0])
-        wp = np.array(wp)
-        return wp
+        wp_rsd = _get_wp_aniso(r, xi0, xi2, xi4, beta, pimax, dlnrp = dlnrp)
+
+        return ius(r, wp_rsd)(rp)
 
-    def get_wp(self, rp, redshift, pimax=None, rsd=False):
+    def get_wp(self, rp, redshift, pimax=None, rsd=False, dlnrp=0.0):
         """get_wp
 
         Compute projected galaxy auto-correlation function :math:`w_\mathrm{p}(r_\mathrm{p})`.
 
         Args:
             r_p (numpy array): 2 dimensional separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the galaxies are located
             pi_max (float): The range of line of sight integral :math:`\pi_{\mathrm{max}}` in :math:`h^{-1}\mathrm{Mpc}`. If None, the projection is performed using the zeroth order Bessel function, i.e., :math:`\pi_{\mathrm{max}}=\infty` (default=None).
             rsd (bool): if True, redshift space distortion is incorporated into the model (default=False).
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
 
         Returns:
             numpy array: projected galaxy auto-correlation function in :math:`h^{-1}\mathrm{Mpc}`
         """
 
         # Projected correlation functions should be the same if or not there is redshift space distortions when integrated to infinity.
-        if (pimax == None and rsd == False) or (pimax == None and rsd == True):
+        if (pimax == None and rsd == False):
             self._check_update_redshift(redshift)
             self._compute_p_1hcs(redshift)
             self._compute_p_1hss(redshift)
             self._compute_p_2hcc(redshift)
             self._compute_p_2hcs(redshift)
             self._compute_p_2hss(redshift)
 
             p_tot_1h = 2.*self.p_1hcs + self.p_1hss
             p_tot_2h = self.p_2hcc + 2.*self.p_2hcs + self.p_2hss
-            wp = ius( self.fftlog_1h.r, self.fftlog_1h.pk2wp(p_tot_1h) )(rp) + ius( self.fftlog_2h.r, self.fftlog_2h.pk2wp(p_tot_2h) )(rp)
+            wp = ius( self.fftlog_1h.r, fftlog.pk2wp(self.fftlog_1h.k, p_tot_1h, N_extrap_low=1024, dlnrp=dlnrp)[1])(rp) + ius(self.fftlog_2h.r, fftlog.pk2wp(self.fftlog_2h.k, p_tot_2h, N_extrap_low=2048, dlnrp=dlnrp)[1] )(rp)
+            #wp = ius( self.fftlog_1h.r, self.fftlog_1h.pk2wp(p_tot_1h, N_extrap_high=0, dlnrp=dlnrp)[1] )(rp) + ius( self.fftlog_2h.r, self.fftlog_2h.pk2wp(p_tot_2h, N_extrap_high=0, dlnrp=dlnrp)[1] )(rp)
             #wp = ius(self.fftlog_1h.r, fftLog.pk2xiproj_J0_fftlog_array(self.fftlog_1h.k, self.fftlog_1h.r, p_tot_1h, self.fftlog_1h.kr, self.fftlog_2h.dlnk))(
             #    rp)+ius(self.fftlog_2h.r, fftLog.pk2xiproj_J0_fftlog_array(self.k_2h, self.r_2h, p_tot_2h, self.kr, self.dlnk_2h))(rp)
+        elif (pimax == None and rsd == True):
+            raise RuntimeError("cannot apply Kaiser for pi_max=inf")
         else:
             if not isinstance(pimax, float):
                 raise RuntimeError("pi_max should be None or float")
             if rsd == True:
-                wp = self._get_wp_rsd(rp, redshift, pimax)
+                wp = self._get_wp_rsd(rp, redshift, pimax, dlnrp)
             else:
                 r_ref = np.logspace(np.min([self.config["fft_logrmin_1h"], self.config["fft_logrmin_2h"]]), np.max(
                     [self.config["fft_logrmax_1h"], self.config["fft_logrmax_2h"]]), 1024)
                 xi_gg_spl = ius(r_ref, self.get_xi_gg(r_ref, redshift))
                 t = np.linspace(0, pimax, 1024)
                 dt = t[1]-t[0]
                 wp = list()
-                for rpnow in rp:
-                    wp.append(
-                        2*integrate.trapz(xi_gg_spl(np.sqrt(t**2+rpnow**2)), dx=dt))
-                wp = np.array(wp)
+                
+                if dlnrp > 0.0:
+                    rpi = np.logspace(-3, np.log10(pimax), 300)
+                    rp2d, rpi2d = np.meshgrid(r_ref, rpi)
+                    s = (rp2d**2+rpi2d**2)**0.5
+                    xi2d = xi_gg_spl(s)
+                    wp = 2*integrate.trapz(xi2d, rpi, axis=0)
+                    wp = binave_array(r_ref, wp, dlnrp)
+                    wp = ius(r_ref, wp)(rp)
+                else:
+                    for rpnow in rp:
+                        wp.append(
+                            2*integrate.trapz(xi_gg_spl(np.sqrt(t**2+rpnow**2)), dx=dt))
+                    wp = np.array(wp)
         return wp
 
-    def get_wp_1hcs(self, rp, redshift):
+    def get_wp_1hcs(self, rp, redshift, dlnrp=0.0):
         """get_wp_1hcs
 
         Compute projected 1-halo correlation function between central and satellite galaxies :math:`w_\mathrm{p, cen-sat}^\mathrm{1h}(r_\mathrm{p})`. Note that the line-of-sight integration is performed using the zeroth order Bessel function, i.e., , :math:`\pi_{\mathrm{max}}=\infty`.
 
         Args:
             r_p (numpy array): 2 dimensional separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the galaxies are located
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
 
         Returns:
             numpy array: projected 1-halo correlation function between central and satellite galaxies in :math:`h^{-1}\mathrm{Mpc}`
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_1hcs(redshift)
-        wp1hcs = ius( self.fftlog_1h.r, self.fftlog_1h.pk2wp(self.p_1hcs) )(rp)
+        #x, y, = fftlog.pk2wp(self.fftlog_1h.k, self.p_1hcs, 1.01, N_extrap_low=2048, dlnrp = dlnrp)
+        wp1hcs = ius(self.fftlog_1h.r, fftlog.pk2wp(self.fftlog_1h.k, self.p_1hcs, 1.01, N_extrap_low=2048, dlnrp = dlnrp)[1] )(rp)
         return wp1hcs
 
-    def get_wp_1hss(self, rp, redshift):
+    def get_wp_1hss(self, rp, redshift, dlnrp=0.0):
         """get_wp_1hss
 
         Compute projected 1-halo correlation function between satellite galaxies :math:`w_\mathrm{p, sat-sat}^\mathrm{1h}(r_\mathrm{p})`. Note that the line-of-sight integration is performed using the zeroth order Bessel function, i.e., , :math:`\pi_{\mathrm{max}}=\infty`.
 
         Args:
             r_p (numpy array): 2 dimensional separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the galaxies are located
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
 
         Returns:
             numpy array: projected 1-halo correlation function between satellite galaxies in :math:`h^{-1}\mathrm{Mpc}`
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_1hss(redshift)
-        wp1hss = ius( self.fftlog_1h.r, self.fftlog_1h.pk2wp(self.p_1hss) )(rp)
+        wp1hss = ius( self.fftlog_1h.r, fftlog.pk2wp(self.fftlog_1h.k, self.p_1hss, 1.01, N_extrap_low=2048, dlnrp = dlnrp)[1] )(rp)
+        #wp1hss = ius( self.fftlog_1h.r, self.fftlog_1h.pk2wp(self.p_1hss, N_extrap_low=1024, dlnrp=dlnrp)[1] )(rp)
         return wp1hss
 
-    def get_wp_2hcc(self, rp, redshift):
+    def get_wp_2hcc(self, rp, redshift, dlnrp=0.0):
         """get_wp_2hcc
 
         Compute projected 2-halo correlation function between central galaxies :math:`w_\mathrm{p, cen-cen}^\mathrm{2h}(r_\mathrm{p})`. Note that the line-of-sight integration is performed using the zeroth order Bessel function, i.e., , :math:`\pi_{\mathrm{max}}=\infty`.
 
         Args:
             r_p (numpy array): 2 dimensional separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the galaxies are located
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
 
         Returns:
             numpy array: projected 2-halo correlation function between central galaxies in :math:`h^{-1}\mathrm{Mpc}`
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_2hcc(redshift)
-        wp2hcc = ius( self.fftlog_2h.r, self.fftlog_2h.pk2wp(self.p_2hcc) )(rp)
+        wp2hcc = ius( self.fftlog_2h.r, fftlog.pk2wp(self.fftlog_2h.k, self.p_2hcc, 1.01, N_extrap_low=2048)[1] )(rp)
+        #wp2hcc = ius( self.fftlog_2h.r, self.fftlog_2h.pk2wp(self.p_2hcc, 1.01, N_extrap_low=2048)[1] )(rp)
         return wp2hcc
 
-    def get_wp_2hcs(self, rp, redshift):
+    def get_wp_2hcs(self, rp, redshift, dlnrp=0.0):
         """get_wp_2hcs
 
         Compute projected 2-halo correlation function between central and satellite galaxies :math:`w_\mathrm{p, cen-sat}^\mathrm{2h}(r_\mathrm{p})`. Note that the line-of-sight integration is performed using the zeroth order Bessel function, i.e., , :math:`\pi_{\mathrm{max}}=\infty`.
 
         Args:
             r_p (numpy array): 2 dimensional separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the galaxies are located
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
 
         Returns:
             numpy array: projected 2-halo correlation function between central and satellite galaxies in :math:`h^{-1}\mathrm{Mpc}`
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_2hcs(redshift)
-        wp2hcs = ius( self.fftlog_2h.r, self.fftlog_2h.pk2wp(self.p_2hcs) )(rp)
+        wp2hcs = ius( self.fftlog_2h.r, fftlog.pk2wp(self.fftlog_2h.k, self.p_2hcs, 1.01, N_extrap_low=2048)[1] )(rp)
+        #wp2hcs = ius( self.fftlog_2h.r, self.fftlog_2h.pk2wp(self.p_2hcs, 1.01, N_extrap_low=2048)[1] )(rp)
         return wp2hcs
 
-    def get_wp_2hss(self, rp, redshift):
+    def get_wp_2hss(self, rp, redshift, dlnrp=0.0):
         """get_wp_2hss
 
         Compute projected 2-halo correlation function between satellite galaxies :math:`w_\mathrm{p, sat-sat}^\mathrm{2h}(r_\mathrm{p})`. Note that the line-of-sight integration is performed using the zeroth order Bessel function, i.e., , :math:`\pi_{\mathrm{max}}=\infty`.
 
         Args:
             r_p (numpy array): 2 dimensional separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the galaxies are located
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
 
         Returns:
             numpy array: projected 2-halo correlation function between satellite galaxies in :math:`h^{-1}\mathrm{Mpc}`
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_2hss(redshift)
-        wp2hss = ius( self.fftlog_2h.r, self.fftlog_2h.pk2wp(self.p_2hss) )(rp)
+        wp2hss = ius( self.fftlog_2h.r, fftlog.pk2wp(self.fftlog_2h.k, self.p_2hss, 1.01, N_extrap_low=2048)[1] )(rp)
+        #wp2hss = ius(self.fftlog_2h.r, fftlog.pk2wp(self.fftlog_2h.k, self.p_2hss, 1.01, N_extrap_low=2048)[1] )(rp)
         return wp2hss
 
     def get_xi_gg(self, r, redshift):
         """get_xi_gg
 
         Compute galaxy auto-correlation function :math:`\\xi_\mathrm{gg}(r)`.
 
@@ -1284,15 +1282,16 @@
         self._compute_p_1hss(redshift)
         self._compute_p_2hcc(redshift)
         self._compute_p_2hcs(redshift)
         self._compute_p_2hss(redshift)
 
         p_tot_1h = 2.*self.p_1hcs + self.p_1hss
         p_tot_2h = self.p_2hcc + 2.*self.p_2hcs + self.p_2hss
-        xi_gg = ius( self.fftlog_1h.r, self.fftlog_1h.pk2xi(p_tot_1h) )(r) + ius( self.fftlog_2h.r, self.fftlog_2h.pk2xi(p_tot_2h) )(r)
+        xi_gg = ius( self.fftlog_1h.r, fftlog.pk2xi(self.fftlog_1h.k, p_tot_1h, N_extrap_low=2048)[1])(r) + ius(self.fftlog_2h.r, fftlog.pk2xi(self.fftlog_2h.k, p_tot_2h, N_extrap_low=2048)[1] )(r)
+        #xi_gg = ius( self.fftlog_1h.r, self.fftlog_1h.pk2xi(p_tot_1h, N_extrap_high=0)[1])(r) + ius( self.fftlog_2h.r, self.fftlog_2h.pk2xi(p_tot_2h, N_extrap_high=0)[1] )(r)
         return xi_gg
 
     def get_xi_gg_1hcs(self, r, redshift):
         """get_xi_gg_1hcs
 
         Compute 1-halo correlation function between central and satellite galaxies :math:`\\xi_\mathrm{cen-sat}^\mathrm{1h}(r)`.
 
@@ -1303,15 +1302,15 @@
         Returns:
             numpy array: 1-halo correlation function between central and satellite galaxies
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_1hcs(redshift)
-        xi_gg_1hcs = ius(self.fftlog_1h.r, self.fftlog_1h.pk2xi(self.p_1hcs) )(r)
+        xi_gg_1hcs = ius(self.fftlog_1h.r,fftlog.pk2xi(self.fftlog_1h.k, self.p_1hcs, N_extrap_low=1024)[1] )(r)
         return xi_gg_1hcs
 
     def get_xi_gg_1hss(self, r, redshift):
         """get_xi_gg_1hss
 
         Compute 1-halo correlation function between satellite galaxies :math:`\\xi_\mathrm{sat-sat}^\mathrm{1h}(r)`.
 
@@ -1322,15 +1321,16 @@
         Returns:
             numpy array: 1-halo correlation function between satellite galaxies
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_1hss(redshift)
-        xi_gg_1hss = ius(self.fftlog_1h.r, self.fftlog_1h.pk2xi(self.p_1hss) )(r)
+        xi_gg_1hss = ius(self.fftlog_1h.r,fftlog.pk2xi(self.fftlog_1h.k, self.p_1hss, N_extrap_low=2048)[1] )(r)
+        #xi_gg_1hss = ius(self.fftlog_1h.r, self.fftlog_1h.pk2xi(self.p_1hss)[1] )(r)
         return xi_gg_1hss
 
     def get_xi_gg_2hcc(self, rp, redshift):
         """get_xi_gg_2hcc
 
         Compute 2-halo correlation function between central galaxies :math:`\\xi_\mathrm{cen-cen}^\mathrm{2h}(r)`.
 
@@ -1341,15 +1341,15 @@
         Returns:
             numpy array: 2-halo correlation function between central galaxies
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_2hcc(redshift)
-        xi_gg_2hcc = ius( self.fftlog_2h.r, self.fftlog_2h.pk2xi(self.p_2hcc) )(rp)
+        xi_gg_2hcc = ius(self.fftlog_2h.r,fftlog.pk2xi(self.fftlog_2h.k, self.p_2hcc, N_extrap_low=2048)[1] )(rp)
         #xi_gg_2hcc = ius(self.fftlog_2h.r, fftLog.pk2xi_fftlog_array(
         #    self.k_2h, self.r_2h, self.p_2hcc, self.kr, self.dlnk_2h))(rp)
         return xi_gg_2hcc
 
     def get_xi_gg_2hcs(self, rp, redshift):
         """get_xi_gg_2hcs
 
@@ -1362,15 +1362,16 @@
         Returns:
             numpy array: 2-halo correlation function between central and satellite galaxies
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_2hcs(redshift)
-        xi_gg_2hcs = ius(self.fftlog_2h.r, self.fftlog_2h.pk2xi(self.p_2hcs) )(rp)
+        xi_gg_2hcs = ius(self.fftlog_2h.r,fftlog.pk2xi(self.fftlog_2h.k, self.p_2hcs, N_extrap_low=2048)[1] )(rp)
+        #xi_gg_2hcs = ius(self.fftlog_2h.r, self.fftlog_2h.pk2xi(self.p_2hcs)[1] )(rp)
         #xi_gg_2hcs = ius(self.fftlog_2h.r, fftLog.pk2xi_fftlog_array(
         #    self.k_2h, self.r_2h, self.p_2hcs, self.kr, self.dlnk_2h))(rp)
         return xi_gg_2hcs
 
     def get_xi_gg_2hss(self, rp, redshift):
         """get_xi_gg_2hss
 
@@ -1383,109 +1384,118 @@
         Returns:
             numpy array: 2-halo correlation function between satellite galaxies
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_2hss(redshift)
-        xi_gg_2hss = ius( self.fftlog_2h.r, self.fftlog_2h.pk2xi(self.p_2hss) )(rp)
+        xi_gg_2hss = ius(self.fftlog_2h.r,fftlog.pk2xi(self.fftlog_2h.k, self.p_2hss, N_extrap_low=2048)[1] )(rp)
+        #xi_gg_2hss = ius( self.fftlog_2h.r, self.fftlog_2h.pk2xi(self.p_2hss)[1] )(rp)
         #xi_gg_2hss = ius(self.fftlog_2h.r, fftLog.pk2xi_fftlog_array(
         #    self.k_2h, self.r_2h, self.p_2hss, self.kr, self.dlnk_2h))(rp)
         return xi_gg_2hss
 
-    def get_ds(self, rp, redshift):
+    def get_ds(self, rp, redshift, dlnrp=0.0):
         """get_ds
 
         Compute weak lensing signal :math:`\Delta\Sigma(r_\mathrm{p})`.
 
         Args:
             rp (numpy array): 2 dimensional projected separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the lens galaxies are located
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
 
         Returns:
             numpy array: excess surface density in :math:`h M_\odot \mathrm{pc}^{-2}`
         """
         self._check_update_redshift(redshift)
 
         self._compute_p_cen(redshift)
         self._compute_p_cen_off(redshift)
         self._compute_p_sat(redshift)
 
         p_tot = self.p_cen + self.p_cen_off + self.p_sat
-        ds = self.rho_m/10**12 * ius( self.fftlog_1h.r, self.fftlog_1h.pk2dwp(p_tot) )(rp)
+        ds = self.rho_m/10**12 * ius( self.fftlog_1h.r, fftlog.pk2dwp(self.fftlog_1h.k, p_tot, N_extrap_high=0, dlnrp=dlnrp)[1] )(rp)
+        #ds = self.rho_m/10**12 * ius( self.fftlog_1h.r, self.fftlog_1h.pk2dwp(p_tot, N_extrap_high=0, dlnrp=dlnrp)[1] )(rp)
         #ds = self.rho_m/10**12*ius(self.fftlog_1h.r, fftLog.pk2xiproj_J2_fftlog_array(
         #    self.k_1h, self.r_1h, p_tot, self.kr, self.dlnk_1h))(rp)
         return ds
 
-    def get_ds_cen(self, rp, redshift):
+    def get_ds_cen(self, rp, redshift, dlnrp=0.0):
         """get_ds_cen
 
         Compute weak lensing signal of (centered) central galaxies :math:`\Delta\Sigma_\mathrm{cen}(r_\mathrm{p})`.
 
         Args:
             rp (numpy array): 2 dimensional projected separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the lens galaxies are located
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
+
 
         Returns:
             numpy array: excess surface density of (centered) central galaxies in :math:`h M_\odot \mathrm{pc}^{-2}`
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_cen(redshift)
-        return self.rho_m/10**12 * ius(self.fftlog_1h.r, self.fftlog_1h.pk2dwp(self.p_cen) )(rp)
+        return self.rho_m/10**12 * ius( self.fftlog_1h.r, fftlog.pk2dwp(self.fftlog_1h.k, self.p_cen, N_extrap_high=0, dlnrp=dlnrp)[1] )(rp)
         #return self.rho_m/10**12*ius(self.fftlog_1h.r, fftLog.pk2xiproj_J2_fftlog_array(self.k_1h, self.r_1h, self.p_cen, self.kr, self.dlnk_1h))(rp)
 
-    def get_ds_cen_off(self, rp, redshift):
+    def get_ds_cen_off(self, rp, redshift, dlnrp=0.0):
         """get_ds_cen_off
 
         Compute weak lensing signal of off-centered central galaxies :math:`\Delta\Sigma_\mathrm{off-cen}(r_\mathrm{p})`.
 
         Args:
             rp (numpy array): 2 dimensional projected separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the lens galaxies are located
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
 
         Returns:
             numpy array: excess surface density of off-centered central galaxies in :math:`h M_\odot \mathrm{pc}^{-2}`
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_cen_off(redshift)
-        return self.rho_m/10**12 * ius(self.fftlog_1h.r, self.fftlog_1h.pk2dwp(self.p_cen_off) )(rp)
+        return self.rho_m/10**12 * ius( self.fftlog_1h.r, fftlog.pk2dwp(self.fftlog_1h.k, self.p_cen_off, N_extrap_high=0, dlnrp=dlnrp)[1] )(rp)
+        #return self.rho_m/10**12 * ius(self.fftlog_1h.r, self.fftlog_1h.pk2dwp(self.p_cen_off, dlnrp=dlnrp, N_extrap_high=0)[1] )(rp)
         #return self.rho_m/10**12*ius(self.fftlog_1h.r, fftLog.pk2xiproj_J2_fftlog_array(self.k_1h, self.r_1h, self.p_cen_off, self.kr, self.dlnk_1h))(rp)
 
-    def get_ds_sat(self, rp, redshift):
+    def get_ds_sat(self, rp, redshift, dlnrp=0.0):
         """get_ds_sat
 
         Compute weak lensing signal of satellite galaxies :math:`\Delta\Sigma_\mathrm{sat}(r_\mathrm{p})`.
 
         Args:
             rp (numpy array): 2 dimensional projected separation in :math:`h^{-1}\mathrm{Mpc}`
             redshift (float): redshift at which the lens galaxies are located
+            dlnrp (float): width of bin averaging in logarithmic scale. If dlnrp=0, no bin average.
 
         Returns:
             numpy array: excess surface density of satellite galaxies in :math:`h M_\odot \mathrm{pc}^{-2}`
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_sat(redshift)
-        return self.rho_m/10**12 * ius(self.fftlog_1h.r, self.fftlog_1h.pk2dwp(self.p_sat) )(rp)
+        return self.rho_m/10**12 * ius( self.fftlog_1h.r, fftlog.pk2dwp(self.fftlog_1h.k, self.p_sat, N_extrap_high=0, dlnrp=dlnrp)[1] )(rp)
+        #return self.rho_m/10**12 * ius(self.fftlog_1h.r, self.fftlog_1h.pk2dwp(self.p_sat, dlnrp=dlnrp)[1] )(rp)
         #return self.rho_m/10**12*ius(self.fftlog_1h.r, fftLog.pk2xiproj_J2_fftlog_array(self.k_1h, self.r_1h, self.p_sat, self.kr, self.dlnk_1h))(rp)
 
-    def _get_wp_gm(self, rp, redshift):
+    def _get_wp_gm(self, rp, redshift, dlnrp=0.0):
         self._check_update_redshift(redshift)
 
         self._compute_p_cen(redshift)
         self._compute_p_cen_off(redshift)
         self._compute_p_sat(redshift)
 
         p_tot = self.p_cen + self.p_cen_off + self.p_sat
-        wp = ius( self.fftlog_1h.r, self.fftlog_1h.pk2wp(p_tot) )(rp)
+        wp = ius( self.fftlog_1h.r, self.fftlog_1h.pk2wp(p_tot, dlnrp=dlnrp)[1] )(rp)
         return wp
 
     def _get_sigma_gm(self, rp, redshift):
         wp = self.wp_gm(rp, redshift)
         return self.rho_m/10**12*wp
 
     def get_xi_gm(self, r, redshift):
@@ -1504,15 +1514,16 @@
         self._check_update_redshift(redshift)
 
         self._compute_p_cen(redshift)
         self._compute_p_cen_off(redshift)
         self._compute_p_sat(redshift)
 
         p_tot = self.p_cen + self.p_cen_off + self.p_sat
-        xi_gm = ius( self.fftlog_1h.r, self.fftlog_1h.pk2xi(p_tot) )(r)
+        #xi_gm = ius( self.fftlog_1h.r, self.fftlog_1h.pk2xi(p_tot)[1] )(r)
+        xi_gm = ius( self.fftlog_1h.r, fftlog.pk2xi(self.fftlog_1h.k, p_tot, 1.01, N_extrap_low=2048)[1])(r)
         return xi_gm
 
     def get_xi_gm_cen(self, r, redshift):
         """get_xi_gm_cen
 
         Compute correlation function between (centered) central galaxies and dark matter :math:`\\xi_\mathrm{gm, cen}(r)`.
 
@@ -1523,15 +1534,15 @@
         Returns:
             numpy array: correlation function between (centered) central galaxies and dark matter
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_cen(redshift)
-        return ius( self.fftlog_1h.r, self.fftlog_1h.pk2xi(self.p_cen) )(r)
+        return ius( self.fftlog_1h.r, fftlog.pk2xi(self.fftlog_1h.k, self.p_cen, N_extrap_low=2048)[1])(r)
 
     def get_xi_gm_cen_off(self, r, redshift):
         """get_xi_gm_cen_off
 
         Compute correlation function between off-centered central galaxies and dark matter :math:`\\xi_\mathrm{gm, off-cen}(r)`.
 
         Args:
@@ -1541,15 +1552,15 @@
         Returns:
             numpy array: correlation function between off-centered central galaxies and dark matter
         """
 
         self._check_update_redshift(redshift)
 
         self._compute_p_cen_off(redshift)
-        return ius( self.fftlog_1h.r, self.fftlog_1h.pk2xi(self.p_cen_off) )(r)
+        return ius( self.fftlog_1h.r, fftlog.pk2xi(self.fftlog_1h.k, self.p_cen_off, N_extrap_low=2048)[1])(r)
 
     def get_xi_gm_sat(self, r, redshift):
         """get_xi_gm_sat
 
         Compute correlation function between satellite galaxies and dark matter :math:`\\xi_\mathrm{gm, sat}(r)`.
 
         Args:
@@ -1558,20 +1569,20 @@
 
         Returns:
             numpy array: correlation function between satellite galaxies and dark matter
         """
 
         self._check_update_redshift(redshift)
         self._compute_p_sat(redshift)
-        return ius( self.fftlog_1h.r, self.fftlog_1h.pk2xi(self.p_sat) )(r)
+        return ius( self.fftlog_1h.r, fftlog.pk2xi(self.fftlog_1h.k, self.p_sat, N_extrap_low=2048)[1])(r)
 
-    def _get_wp_mm(self, rp, redshift):
+    def _get_wp_mm(self, rp, redshift, dlnrp=0.0):
         xi = self.get_xinl(self.fftlog_2h.r, redshift)
-        pk = self.fftlog_2h.xi2pk(xi)
-        wp = self.fftlog_2h.pk2wp(pk)
+        pk = self.fftlog_2h.xi2pk(xi)[1]
+        wp = self.fftlog_2h.pk2wp(pk, N_extrap_high=0, dlnrp=dlnrp)[1]
         #pk = fftLog.xi2pk_fftlog_array(
         #    self.r_2h, self.k_2h, xi, self.kr, self.dlnr_2h)
         #wp = ius(self.fftlog_2h.r, fftLog.pk2xiproj_J0_fftlog_array(
         #    self.k_2h, self.r_2h, pk, self.kr, self.dlnk_2h))(rp)
         return wp
 
     def get_ng(self, redshift):
@@ -1647,15 +1658,14 @@
         if target_m_or_c == "m":
             target_rho = self.cosmo.get_Omega0()*(1.+z)**3*rho_cr
         elif target_m_or_c == "c":
             target_rho = self.cosmo.get_Ez(z)**2.*rho_cr
 
         def F(target_c):
             return target_delta*target_c**3*self._get_fNFW(target_c)*target_rho - delta*c**3*self._get_fNFW(c)*rho
-        #print("c", c)
         target_c = optimize.newton(F, c)
         return target_c
 
     def _get_concentration_Bullock01(self, M_200m, z):
         """
         This is the implementation of Eq. (18) at Bullock et al. (2001). Note that this method is not tested yet.
         """
@@ -1674,15 +1684,15 @@
             M_vir = self._get_fNFW(c_200m)/self._get_fNFW(c_vir)*M_200m
             c_vir_bullock01 = c0/(1.+z)*(M_vir/M_star_vir)**-beta
             return c_vir - c_vir_bullock01
         c_200m = optimize.newton(F, c0, args = (M_200m, M_star_vir, c0, beta, delta_vir, z))
         return c_200m
 
     def _get_concentration_Maccio08(self, M_200m, z):
-        print("halo mass", M_200m/10**14.)
+        logging.info("halo mass", M_200m/10**14.)
         K = 3.85
         F = 0.01
 
         l_z = np.linspace(0., 100., 1000)
         D0 = np.array([self.Dgrowth_from_z(_z) for _z in l_z])
         z_of_D0= ius(D0[::-1], l_z[::-1])
         def get_c_200m(c_200m):
@@ -1799,7 +1809,52 @@
     Ode = params[0,2]
     wde = params[0,5]
     growth = _linearGrowth(Ode,wde,redshift)/_linearGrowth(Ode,wde,0.)
     sigM = growth*massfunc.sM.get_sigma(Mh)
     nu = delta_c/sigM
     b = 1.-A*nu**a/(nu**a+delta_c**a) + B*nu**b + C*nu**c
     return b
+
+def _get_wp_aniso(r, xi0, xi2, xi4, beta, pimax, dlnrp = 0.):
+    # Numerator of Eq. (48) of arxiv: 1206.6890 using mutipole expansion of anisotropic xi including Kaiser effect in Eq. (51) of the same paper.
+
+
+    rpi = np.logspace(-3, np.log10(pimax), 300) # Ok binning for 1% accuracy.
+
+    rp2, rpi2 = np.meshgrid(r, rpi)
+
+    s = (rp2**2+rpi2**2)**0.5
+    mu= rpi2/s
+
+    xi0s = (1+2.0/3.0*beta+1.0/5.0*beta**2)*ius(r, xi0)(s)
+    xi2s = (4.0/3.0*beta+4.0/7.0*beta**2)*ius(r, xi2)(s)
+    xi4s = 8.0/35.0*beta**2*ius(r, xi4)(s)
+
+    p0 = 1
+    p2 = eval_legendre(2, mu)
+    p4 = eval_legendre(4, mu)
+
+    xi_aniso = 2*(xi0s*p0+xi2s*p2+xi4s*p4)
+
+    wp_aniso = simps(xi_aniso, rpi, axis=0)
+
+    if dlnrp > 0.0:
+        wp_aniso = binave_array(r, wp_aniso, dlnrp)
+    return wp_aniso
+
+def binave_array(x, y, dlnx, D=2, nbin=100):
+    """
+    Assumes dlnx << np.diff(x).
+    Performs the forward bin average in dimension D.
+    ::math::
+        \\bar{y} = \\frac{1}{d\\ln x} \\int_{\\ln x}^{\\ln x+d\\ln x} x^D y(x)
+    """
+    X = np.linspace(0.0, dlnx, nbin)
+    x2d, X2d = np.meshgrid(x,X)
+    arg = x2d*np.exp(X2d)
+    y2d = ius(x, y)(arg)
+    
+    nom = integrate.simps(arg**D, X, axis=0)
+    
+    ybar = integrate.simps(y2d*arg**D, X, axis=0)/nom
+    
+    return ybar
```

### Comparing `dark_emulator-1.0.23/dark_emulator.egg-info/PKG-INFO` & `dark_emulator-1.1.1/dark_emulator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 Metadata-Version: 2.1
 Name: dark-emulator
-Version: 1.0.23
+Version: 1.1.1
 Summary: dark emulator package
 Home-page: https://dark-emulator.readthedocs.io
-Author: Takahiro Nishimichi, Hironao Miyatake
+Author: Takahiro Nishimichi, Hironao Miyatake, Sunao Sugiyama
 Author-email: dark_emulator@ipmu.jp
-License: UNKNOWN
-Description: # Dark Emulator
-        [![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/version.svg)](https://anaconda.org/nishimichi/dark_emulator)
-        [![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/latest_release_date.svg)](https://anaconda.org/nishimichi/dark_emulator)
-        [![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/license.svg)](https://anaconda.org/nishimichi/dark_emulator)
-        [![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/downloads.svg)](https://anaconda.org/nishimichi/dark_emulator)
-        
-        A repository for a cosmology tool `dark_emulator` to emulate halo clustering statistics. The code is developed based on Dark Quest simulation suite (https://darkquestcosmology.github.io/). The current version supports the halo mass function and two point correlation function (both halo-halo and halo-matter cross).
-        
-        ## Install
-        In order to install dark emulator package, use pip:
-        ```
-           pip install dark_emulator
-        ```
-        or use conda:
-        ```
-           conda install -c nishimichi dark_emulator
-        ```
-        If the above does not work for you, you may download the source files from this repository and install via
-        ```
-        python -m pip install -e .
-        ```
-        after moving to the top directory of the source tree.
-        In that case, you need to install `pyfftlog`, `george` (a software package for the Gaussian process) and colossus
-        ```
-        conda install -c conda-forge george
-        conda install -c conda-forge pyfftlog
-        pip install colossus
-        ```
-        
-        ## Usage
-        You can then check how Dark Emulator works by running a tutorial notebook at
-        ```
-        docs/tutorial.ipynb
-        docs/tutorial-hod.ipynb
-        ```
-        See also the documentation on [readthedocs](https://dark-emulator.readthedocs.io/en/latest/).
-        
-        ## Code Paper
-        The main reference for our halo emulation strategy is: "Dark Quest. I. Fast and Accurate Emulation of Halo Clustering Statistics and Its Application to Galaxy Clustering", by T. Nishimichi et al., [ApJ 884, 29 (2019)](https://iopscience.iop.org/article/10.3847/1538-4357/ab3719/meta), [arXiv:1811.09504](https://arxiv.org/abs/1811.09504). Please also refer to the paper "Cosmological inference from emulator based halo model I: Validation tests with HSC and SDSS mock catalogs", by H. Miyatake et al.,  [arXiv:2101.00113](https://arxiv.org/abs/2101.00113) for the implementation and performance of the halo-galaxy connection routines.
-        
-        
 Keywords: cosmology,large scale structure,halo,gaussian process,machine learning
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Dark Emulator
+[![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/version.svg)](https://anaconda.org/nishimichi/dark_emulator)
+[![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/latest_release_date.svg)](https://anaconda.org/nishimichi/dark_emulator)
+[![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/license.svg)](https://anaconda.org/nishimichi/dark_emulator)
+[![Anaconda-Server Badge](https://anaconda.org/nishimichi/dark_emulator/badges/downloads.svg)](https://anaconda.org/nishimichi/dark_emulator)
+
+A repository for a cosmology tool `dark_emulator` to emulate halo clustering statistics. The code is developed based on Dark Quest simulation suite (https://darkquestcosmology.github.io/). The current version supports the halo mass function and two point correlation function (both halo-halo and halo-matter cross).
+
+## Install
+In order to install dark emulator package, use pip:
+```
+   pip install dark_emulator
+```
+or use conda:
+```
+   conda install -c nishimichi dark_emulator
+```
+If the above does not work for you, you may download the source files from this repository and install via
+```
+python -m pip install -e .
+```
+after moving to the top directory of the source tree.
+In that case, you need to install `george` (a software package for the Gaussian process) and colossus
+```
+conda install -c conda-forge george
+pip install colossus
+```
+From version 1.1.0, `dark_emulator` uses FFTLog implementation by [Fang et al (2019); arXiv:1911.11947](https://arxiv.org/abs/1911.11947).
+
+## Usage
+You can then check how Dark Emulator works by running a tutorial notebook at
+```
+docs/tutorial.ipynb
+docs/tutorial-hod.ipynb
+```
+See also the documentation on [readthedocs](https://dark-emulator.readthedocs.io/en/latest/).
+
+## Code Paper
+The main reference for our halo emulation strategy is: "Dark Quest. I. Fast and Accurate Emulation of Halo Clustering Statistics and Its Application to Galaxy Clustering", by T. Nishimichi et al., [ApJ 884, 29 (2019)](https://iopscience.iop.org/article/10.3847/1538-4357/ab3719/meta), [arXiv:1811.09504](https://arxiv.org/abs/1811.09504). Please also refer to the paper "Cosmological inference from emulator based halo model I: Validation tests with HSC and SDSS mock catalogs", by H. Miyatake et al.,  [arXiv:2101.00113](https://arxiv.org/abs/2101.00113) for the implementation and performance of the halo-galaxy connection routines.
+
```

### Comparing `dark_emulator-1.0.23/dark_emulator.egg-info/SOURCES.txt` & `dark_emulator-1.1.1/dark_emulator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 dark_emulator/__init__.py
 dark_emulator.egg-info/PKG-INFO
 dark_emulator.egg-info/SOURCES.txt
@@ -78,12 +79,9 @@
 dark_emulator/learned_data/xinl/coeff_all.npy
 dark_emulator/learned_data/xinl/gp6d_hyperparams.npy
 dark_emulator/learned_data/xinl/gp6d_kerneltype.npy
 dark_emulator/learned_data/xinl/pca_eigvec.npy
 dark_emulator/learned_data/xinl/yerr.npy
 dark_emulator/model_hod/__init__.py
 dark_emulator/model_hod/hod_interface.py
-dark_emulator/pyfftlog_interface/__init__.py
-dark_emulator/pyfftlog_interface/pyfftlog_class.py
-dark_emulator/pyfftlog_interface/pyfftlog_funcs.py
 docs/tutorial-hod.ipynb
 docs/tutorial.ipynb
```

### Comparing `dark_emulator-1.0.23/docs/tutorial-hod.ipynb` & `dark_emulator-1.1.1/docs/tutorial-hod.ipynb`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/docs/tutorial.ipynb` & `dark_emulator-1.1.1/docs/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dark_emulator-1.0.23/setup.py` & `dark_emulator-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     match = re.search(r"^__%s__ = ['\"]([^'\"]*)['\"]"%(what), f, re.M)
     if match:
         return match.group(1)
     raise RuntimeError("Unable to find %s string."%what)
 
 packages = ['dark_emulator',
             'dark_emulator/darkemu','dark_emulator/darkemu/gp',
-            'dark_emulator/model_hod',
-            'dark_emulator/pyfftlog_interface']
+            'dark_emulator/model_hod']
 
 setup(
     name='dark_emulator',
     version=find_from_doc('version'),
     description='dark emulator package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

