# Comparing `tmp/pyadi-iio-0.0.8.tar.gz` & `tmp/pyadi-iio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyadi-iio-0.0.8.tar", last modified: Fri Jun 25 18:38:59 2021, max compression
+gzip compressed data, was "dist/pyadi-iio-0.0.9.tar", last modified: Tue Sep 21 17:29:47 2021, max compression
```

## Comparing `pyadi-iio-0.0.8.tar` & `pyadi-iio-0.0.9.tar`

### file list

```diff
@@ -1,84 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 18:38:59.000000 pyadi-iio-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-06-25 18:38:59.000000 pyadi-iio-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 18:38:59.000000 pyadi-iio-0.0.8/adi/
--rw-r--r--   0 runner    (1001) docker     (121)     3498 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/obs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3962 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adis16507.py
--rw-r--r--   0 runner    (1001) docker     (121)     9283 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/fmclidar1.py
--rw-r--r--   0 runner    (1001) docker     (121)    10450 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adrv9009.py
--rw-r--r--   0 runner    (1001) docker     (121)    12786 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/dds.py
--rw-r--r--   0 runner    (1001) docker     (121)     8615 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)    14992 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/rx_tx.py
--rw-r--r--   0 runner    (1001) docker     (121)    64898 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adar1000.py
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/cn0532.py
--rw-r--r--   0 runner    (1001) docker     (121)     4801 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adxrs290.py
--rw-r--r--   0 runner    (1001) docker     (121)     3922 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad5627.py
--rw-r--r--   0 runner    (1001) docker     (121)     5819 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad5686.py
--rw-r--r--   0 runner    (1001) docker     (121)     4246 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adxl345.py
--rw-r--r--   0 runner    (1001) docker     (121)     5404 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad7606.py
--rw-r--r--   0 runner    (1001) docker     (121)     4134 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adpd410x.py
--rw-r--r--   0 runner    (1001) docker     (121)     6435 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad7746.py
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adis16460.py
--rw-r--r--   0 runner    (1001) docker     (121)    17137 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adrv9009_zu11eg_multi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5498 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad7124.py
--rw-r--r--   0 runner    (1001) docker     (121)    14044 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad9081_mc.py
--rw-r--r--   0 runner    (1001) docker     (121)    17209 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad9081.py
--rw-r--r--   0 runner    (1001) docker     (121)    14455 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/fmcomms5.py
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad9680.py
--rw-r--r--   0 runner    (1001) docker     (121)     4145 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad7689.py
--rw-r--r--   0 runner    (1001) docker     (121)     3035 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad9136.py
--rw-r--r--   0 runner    (1001) docker     (121)    15125 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adrv9009_zu11eg_fmcomms8.py
--rw-r--r--   0 runner    (1001) docker     (121)     7698 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/cn0540.py
--rw-r--r--   0 runner    (1001) docker     (121)     3166 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad7799.py
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/daq3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3446 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/sshfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ltc2983.py
--rw-r--r--   0 runner    (1001) docker     (121)    14848 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad9371.py
--rw-r--r--   0 runner    (1001) docker     (121)     2751 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad9152.py
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/daq2.py
--rw-r--r--   0 runner    (1001) docker     (121)    10305 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adrv9009_zu11eg.py
--rw-r--r--   0 runner    (1001) docker     (121)     4109 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/jesd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad9094.py
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ltc2314_14.py
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad9144.py
--rw-r--r--   0 runner    (1001) docker     (121)    13556 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/ad936x.py
--rw-r--r--   0 runner    (1001) docker     (121)     4152 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/one_bit_adc_dac.py
--rw-r--r--   0 runner    (1001) docker     (121)    29715 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/adi/adrv9002.py
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     4514 2021-06-25 18:38:59.000000 pyadi-iio-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 18:38:59.000000 pyadi-iio-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad9136_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad7606.py
--rw-r--r--   0 runner    (1001) docker     (121)     5642 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad9364_p.py
--rw-r--r--   0 runner    (1001) docker     (121)     7128 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_adrv9009_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad9144_p.py
--rw-r--r--   0 runner    (1001) docker     (121)     9991 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_fmcomms5_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_adpd410x.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad7799.py
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_stress.py
--rw-r--r--   0 runner    (1001) docker     (121)    11627 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_adrv9009_zu11eg_fmcomms8.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_adrv9002_generic_p.py
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_daq2_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad9680_p.py
--rw-r--r--   0 runner    (1001) docker     (121)     3022 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6021 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_pluto_p.py
--rw-r--r--   0 runner    (1001) docker     (121)    13095 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_adrv9002_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      651 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_adis16507_p.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_sshfs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10910 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_adrv9009_zu11eg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_daq3_p.py
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_map.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_adis16460_p.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad7689.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad9152_p.py
--rw-r--r--   0 runner    (1001) docker     (121)    26984 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad9371.py
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad9361_p.py
--rw-r--r--   0 runner    (1001) docker     (121)    11308 2021-06-25 18:37:00.000000 pyadi-iio-0.0.8/test/test_ad9081.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 18:38:59.000000 pyadi-iio-0.0.8/pyadi_iio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-06-25 18:38:58.000000 pyadi-iio-0.0.8/pyadi_iio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-06-25 18:38:58.000000 pyadi-iio-0.0.8/pyadi_iio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-06-25 18:38:58.000000 pyadi-iio-0.0.8/pyadi_iio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4514 2021-06-25 18:38:58.000000 pyadi-iio-0.0.8/pyadi_iio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-25 18:38:58.000000 pyadi-iio-0.0.8/pyadi_iio.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/adi/
+-rw-r--r--   0 runner    (1001) docker     (121)    65488 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adar1000.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2973 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ltc2314_14.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4246 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adxl345.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9283 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/fmclidar1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14455 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/fmcomms5.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15715 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adrv9009.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3498 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/obs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad9094.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2806 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad9680.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3962 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adis16507.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5404 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad7606.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2751 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad9152.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4152 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/one_bit_adc_dac.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3035 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad9136.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3492 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4109 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/jesd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4801 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adxrs290.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2112 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ltc2983.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/daq3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14848 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad9371.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29715 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adrv9002.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6435 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad7746.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11683 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adis16495.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3166 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad7799.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4145 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad7689.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8615 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15125 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adrv9009_zu11eg_fmcomms8.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/daq2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3335 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adis16460.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12786 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/dds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5498 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad7124.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15865 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/rx_tx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2775 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad9144.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8047 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/cn0540.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13556 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad936x.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17209 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad9081.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17137 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adrv9009_zu11eg_multi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3922 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad5627.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad9083.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3446 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/sshfs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2920 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5819 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad5686.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2969 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/cn0532.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4134 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adpd410x.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14044 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/ad9081_mc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6936 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adf4371.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10305 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adrv9009_zu11eg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4663 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/adi/adpd188.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/pyadi_iio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/pyadi_iio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/pyadi_iio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/pyadi_iio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4514 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/pyadi_iio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/pyadi_iio.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad7799.py
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad9136_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad9144_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5642 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad9364_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13929 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_adrv9002_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1611 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_stress.py
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_adis16460_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26984 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad9371.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad7689.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10910 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_adrv9009_zu11eg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3022 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad7606.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28827 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_adrv9009_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad9680_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_adis16507_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4154 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad9361_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_adrv9002_generic_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1605 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_daq3_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9991 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_fmcomms5_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11627 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_adrv9009_zu11eg_fmcomms8.py
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad9083_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2178 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_adis16495_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2943 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_adpd410x.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6962 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_pluto_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad9152_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_daq2_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11308 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_ad9081.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_sshfs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5984 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/test/test_fmcomms2-3_p.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4514 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-09-21 17:28:23.000000 pyadi-iio-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2021-09-21 17:29:47.000000 pyadi-iio-0.0.9/setup.cfg
```

### Comparing `pyadi-iio-0.0.8/setup.cfg` & `pyadi-iio-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/obs.py` & `pyadi-iio-0.0.9/adi/obs.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/adis16507.py` & `pyadi-iio-0.0.9/adi/adis16507.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/fmclidar1.py` & `pyadi-iio-0.0.9/adi/fmclidar1.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/adrv9009.py` & `pyadi-iio-0.0.9/adi/adis16495.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019 Analog Devices, Inc.
+# Copyright (C) 2020 Analog Devices, Inc.
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #     - Redistributions of source code must retain the above copyright
 #       notice, this list of conditions and the following disclaimer.
@@ -27,239 +27,288 @@
 # IN NO EVENT SHALL ANALOG DEVICES BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, INTELLECTUAL PROPERTY
 # RIGHTS, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF
 # THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import numpy as np
 from adi.context_manager import context_manager
-from adi.rx_tx import rx_tx
+from adi.rx_tx import rx
 
 
-def _import_jesd(uri):
-    try:
-        from adi.jesd import jesd as jesdadi
-    except ImportError:
-        raise Exception("JESD interfaces require fs package")
-    return jesdadi(uri)
-
-
-class adrv9009(rx_tx, context_manager):
-    """ ADRV9009 Transceiver
-
-    parameters:
-        uri: type=string
-            URI of context with ADRV9009
-        jesd_monitor: type=boolean
-            Boolean flag to enable JESD monitoring. jesd input is
-            ignored otherwise.
-        jesd: type=adi.jesd
-            JESD object associated with ADRV9009
-    """
-
-    _complex_data = True
-    _rx_channel_names = ["voltage0_i", "voltage0_q", "voltage1_i", "voltage1_q"]
-    _tx_channel_names = ["voltage0", "voltage1", "voltage2", "voltage3"]
+class adis16495(rx, context_manager):
+    """ADIS16495 Precision, Miniature MEMS IMU."""
+
+    _complex_data = False
+    _rx_channel_names = [
+        "anglvel_x",
+        "anglvel_y",
+        "anglvel_z",
+        "accel_x",
+        "accel_y",
+        "accel_z",
+    ]
     _device_name = ""
+    _rx_data_type = ">i4"
+    _rx_data_si_type = np.float
 
-    def __init__(self, uri="", jesd_monitor=False, jesd=None):
+    def __init__(self, uri="", name="adis16495-3"):
+        """Initialize an adis16495 object.
 
+        parameters:
+            uri: type=string
+                URI of IIO context with adis16495.
+            name: type=string
+                Name of the device. Set to adis16495-3
+                by default.
+        """
+        trigger_name = name + "-dev0"
         context_manager.__init__(self, uri, self._device_name)
 
-        self._ctrl = self._ctx.find_device("adrv9009-phy")
-        self._rxadc = self._ctx.find_device("axi-adrv9009-rx-hpc")
-        self._rxobs = self._ctx.find_device("axi-adrv9009-rx-obs-hpc")
-        self._txdac = self._ctx.find_device("axi-adrv9009-tx-hpc")
-        self._ctx.set_timeout(30000)  # Needed for loading profiles
-        self._jesd = jesd or _import_jesd(uri) if jesd_monitor else None
-        rx_tx.__init__(self)
+        self._ctrl = self._ctx.find_device(name)
+        self._rxadc = self._ctx.find_device(name)
+        # Set default trigger
+        self._trigger = self._ctx.find_device(trigger_name)
+        self._rxadc._set_trigger(self._trigger)
+        rx.__init__(self)
+        self.rx_buffer_size = 16  # Make default buffer smaller
 
+    # device attributes
     @property
-    def profile(self):
-        """Load profile file. Provide path to profile file to attribute"""
-        return self._get_iio_dev_attr("profile_config")
+    def sample_rate(self):
+        """Sample_rate: Sample rate in samples per second."""
+        return self._get_iio_dev_attr("sampling_frequency")
 
-    @profile.setter
-    def profile(self, value):
-        with open(value, "r") as file:
-            data = file.read()
-        # Apply profiles in specific order if multiple phys found
-        phys = [p for p in self.__dict__.keys() if "_ctrl" in p]
-        phys = sorted(phys)
-        for phy in phys[1:] + [phys[0]]:
-            self._set_iio_dev_attr_str("profile_config", data, self.getattr(phy))
+    @sample_rate.setter
+    def sample_rate(self, value):
+        self._set_iio_dev_attr_str("sampling_frequency", value)
 
     @property
-    def frequency_hopping_mode(self):
-        """frequency_hopping_mode: Set Frequency Hopping Mode"""
-        return self._get_iio_attr("TRX_LO", "frequency_hopping_mode", True)
+    def current_timestamp_clock(self):
+        """Current_timestamp_clock: Source clock for timestamps."""
+        return self._get_iio_dev_attr("current_timestamp_clock")
 
-    @frequency_hopping_mode.setter
-    def frequency_hopping_mode(self, value):
-        self._set_iio_attr("TRX_LO", "frequency_hopping_mode", True, value)
+    @current_timestamp_clock.setter
+    def current_timestamp_clock(self, value):
+        self._set_iio_dev_attr_str("current_timestamp_clock", value)
 
-    @property
-    def frequency_hopping_mode_en(self):
-        """frequency_hopping_mode_en: Enable Frequency Hopping Mode"""
-        return self._get_iio_attr("TRX_LO", "frequency_hopping_mode_enable", True)
+    # channel attributes
+    def get_temp(self):
+        """Value returned in millidegrees celsius."""
+        raw = self._get_iio_attr("temp0", "raw", False)
+        off = self._get_iio_attr("temp0", "offset", False)
+        scale = self._get_iio_attr("temp0", "scale", False)
 
-    @frequency_hopping_mode_en.setter
-    def frequency_hopping_mode_en(self, value):
-        self._set_iio_attr("TRX_LO", "frequency_hopping_mode_enable", True, value)
+        return (raw + off) * scale
 
-    @property
-    def calibrate_rx_phase_correction_en(self):
-        """calibrate_rx_phase_correction_en: Enable RX Phase Correction Calibration"""
-        return self._get_iio_dev_attr("calibrate_rx_phase_correction_en")
+    temperature = property(get_temp, None)
 
-    @calibrate_rx_phase_correction_en.setter
-    def calibrate_rx_phase_correction_en(self, value):
-        self._set_iio_dev_attr_str("calibrate_rx_phase_correction_en", value)
+    def __get_scaled_sensor(self, channel_name: str) -> float:
+        raw = self._get_iio_attr(channel_name, "raw", False)
+        scale = self._get_iio_attr(channel_name, "scale", False)
 
-    @property
-    def calibrate_rx_qec_en(self):
-        """calibrate_rx_qec_en: Enable RX QEC Calibration"""
-        return self._get_iio_dev_attr("calibrate_rx_qec_en")
+        return raw * scale
+
+    # get anglvel_x related attributes
+    def get_anglvel_x(self):
+        """Value returned in radians per second."""
+        return self.__get_scaled_sensor("anglvel_x")
 
-    @calibrate_rx_qec_en.setter
-    def calibrate_rx_qec_en(self, value):
-        self._set_iio_dev_attr_str("calibrate_rx_qec_en", value)
+    anglvel_x = property(get_anglvel_x, None)
 
     @property
-    def calibrate_tx_qec_en(self):
-        """calibrate_tx_qec_en: Enable TX QEC Calibration"""
-        return self._get_iio_dev_attr("calibrate_tx_qec_en")
+    def anglvel_x_filter_low_pass_3db_frequency(self):
+        return self._get_iio_attr("anglvel_x", "filter_low_pass_3db_frequency", False)
 
-    @calibrate_tx_qec_en.setter
-    def calibrate_tx_qec_en(self, value):
-        self._set_iio_dev_attr_str("calibrate_tx_qec_en", value)
+    @anglvel_x_filter_low_pass_3db_frequency.setter
+    def anglvel_x_filter_low_pass_3db_frequency(self, value):
+        """Value returned in HZ."""
+        self._set_iio_attr("anglvel_x", "filter_low_pass_3db_frequency", False, value)
 
     @property
-    def calibrate(self):
-        """calibrate: Trigger Calibration"""
-        return self._get_iio_dev_attr("calibrate")
+    def anglvel_x_calibbias(self):
+        """User bias adjustment for the x-axis."""
+        return self._get_iio_attr("anglvel_x", "calibbias", False)
 
-    @calibrate.setter
-    def calibrate(self, value):
-        self._set_iio_dev_attr_str("calibrate", value)
+    @anglvel_x_calibbias.setter
+    def anglvel_x_calibbias(self, value):
+        self._set_iio_attr("anglvel_x", "calibbias", False, value)
 
     @property
-    def gain_control_mode_chan0(self):
-        """gain_control_mode_chan0: Mode of receive path AGC. Options are:
-        slow_attack, manual"""
-        return self._get_iio_attr_str("voltage0", "gain_control_mode", False)
+    def anglvel_x_calibscale(self):
+        """User scale adjustment for the x-axis."""
+        return self._get_iio_attr("anglvel_x", "calibscale", False)
+
+    @anglvel_x_calibscale.setter
+    def anglvel_x_calibscale(self, value):
+        self._set_iio_attr("anglvel_x", "calibscale", False, value)
 
-    @gain_control_mode_chan0.setter
-    def gain_control_mode_chan0(self, value):
-        self._set_iio_attr("voltage0", "gain_control_mode", False, value)
+    # get anglvel_y related attributes
+    def get_anglvel_y(self):
+        """Value returned in radians per second."""
+        return self.__get_scaled_sensor("anglvel_y")
+
+    anglvel_y = property(get_anglvel_y, None)
 
     @property
-    def gain_control_mode_chan1(self):
-        """gain_control_mode_chan1: Mode of receive path AGC. Options are:
-        slow_attack, manual"""
-        return self._get_iio_attr_str("voltage1", "gain_control_mode", False)
+    def anglvel_y_filter_low_pass_3db_frequency(self):
+        """Value returned in HZ."""
+        return self._get_iio_attr("anglvel_y", "filter_low_pass_3db_frequency", False)
 
-    @gain_control_mode_chan1.setter
-    def gain_control_mode_chan1(self, value):
-        self._set_iio_attr("voltage1", "gain_control_mode", False, value)
+    @anglvel_y_filter_low_pass_3db_frequency.setter
+    def anglvel_y_filter_low_pass_3db_frequency(self, value):
+        self._set_iio_attr("anglvel_y", "filter_low_pass_3db_frequency", False, value)
 
     @property
-    def rx_hardwaregain_chan0(self):
-        """rx_hardwaregain: Gain applied to RX path channel 0. Only applicable when
-        gain_control_mode is set to 'manual'"""
-        return self._get_iio_attr("voltage0", "hardwaregain", False)
+    def anglvel_y_calibbias(self):
+        """User bias adjustment for the y-axis."""
+        return self._get_iio_attr("anglvel_y", "calibbias", False)
 
-    @rx_hardwaregain_chan0.setter
-    def rx_hardwaregain_chan0(self, value):
-        if self.gain_control_mode_chan0 == "manual":
-            self._set_iio_attr("voltage0", "hardwaregain", False, value)
+    @anglvel_y_calibbias.setter
+    def anglvel_y_calibbias(self, value):
+        self._set_iio_attr("anglvel_y", "calibbias", False, value)
 
     @property
-    def rx_hardwaregain_chan1(self):
-        """rx_hardwaregain: Gain applied to RX path channel 1. Only applicable when
-        gain_control_mode is set to 'manual'"""
-        return self._get_iio_attr("voltage1", "hardwaregain", False)
+    def anglvel_y_calibscale(self):
+        """User scale adjustment for the y-axis."""
+        return self._get_iio_attr("anglvel_y", "calibscale", False)
+
+    @anglvel_y_calibscale.setter
+    def anglvel_y_calibscale(self, value):
+        self._set_iio_attr("anglvel_y", "calibscale", False, value)
+
+    # get anglvel_z related attributes
+    def get_anglvel_z(self):
+        """Value returned in radians per second."""
+        return self.__get_scaled_sensor("anglvel_z")
 
-    @rx_hardwaregain_chan1.setter
-    def rx_hardwaregain_chan1(self, value):
-        if self.gain_control_mode_chan1 == "manual":
-            self._set_iio_attr("voltage1", "hardwaregain", False, value)
+    anglvel_z = property(get_anglvel_z, None)
 
     @property
-    def tx_hardwaregain_chan0(self):
-        """tx_hardwaregain: Attenuation applied to TX path channel 0"""
-        return self._get_iio_attr("voltage0", "hardwaregain", True)
+    def anglvel_z_filter_low_pass_3db_frequency(self):
+        """Value returned in HZ."""
+        return self._get_iio_attr("anglvel_z", "filter_low_pass_3db_frequency", False)
 
-    @tx_hardwaregain_chan0.setter
-    def tx_hardwaregain_chan0(self, value):
-        self._set_iio_attr("voltage0", "hardwaregain", True, value)
+    @anglvel_z_filter_low_pass_3db_frequency.setter
+    def anglvel_z_filter_low_pass_3db_frequency(self, value):
+        self._set_iio_attr("anglvel_z", "filter_low_pass_3db_frequency", False, value)
 
     @property
-    def tx_hardwaregain_chan1(self):
-        """tx_hardwaregain: Attenuation applied to TX path channel 1"""
-        return self._get_iio_attr("voltage1", "hardwaregain", True)
+    def anglvel_z_calibbias(self):
+        """User bias adjustment for the z-axis."""
+        return self._get_iio_attr("anglvel_z", "calibbias", False)
 
-    @tx_hardwaregain_chan1.setter
-    def tx_hardwaregain_chan1(self, value):
-        self._set_iio_attr("voltage1", "hardwaregain", True, value)
+    @anglvel_z_calibbias.setter
+    def anglvel_z_calibbias(self, value):
+        self._set_iio_attr("anglvel_z", "calibbias", False, value)
 
     @property
-    def rx_rf_bandwidth(self):
-        """rx_rf_bandwidth: Bandwidth of front-end analog filter of RX path"""
-        return self._get_iio_attr("voltage0", "rf_bandwidth", False)
+    def anglvel_z_calibscale(self):
+        """User scale adjustment for the z-axis."""
+        return self._get_iio_attr("anglvel_z", "calibscale", False)
+
+    @anglvel_z_calibscale.setter
+    def anglvel_z_calibscale(self, value):
+        self._set_iio_attr("anglvel_z", "calibscale", False, value)
+
+    # get accel_x related attributes
+    def get_accel_x(self):
+        """Value returned in m/s^2."""
+        return self.__get_scaled_sensor("accel_x")
+
+    accel_x = property(get_accel_x, None)
 
     @property
-    def tx_rf_bandwidth(self):
-        """tx_rf_bandwidth: Bandwidth of front-end analog filter of TX path"""
-        return self._get_iio_attr("voltage0", "rf_bandwidth", True)
+    def accel_x_filter_low_pass_3db_frequency(self):
+        """Value returned in HZ."""
+        return self._get_iio_attr("accel_x", "filter_low_pass_3db_frequency", False)
+
+    @accel_x_filter_low_pass_3db_frequency.setter
+    def accel_x_filter_low_pass_3db_frequency(self, value):
+        self._set_iio_attr("accel_x", "filter_low_pass_3db_frequency", False, value)
 
     @property
-    def rx_sample_rate(self):
-        """rx_sample_rate: Sample rate RX path in samples per second"""
-        return self._get_iio_attr("voltage0", "sampling_frequency", False)
+    def accel_x_calibbias(self):
+        """User bias adjustment for the x-axis."""
+        return self._get_iio_attr("accel_x", "calibbias", False)
+
+    @accel_x_calibbias.setter
+    def accel_x_calibbias(self, value):
+        self._set_iio_attr("accel_x", "calibbias", False, value)
 
     @property
-    def tx_sample_rate(self):
-        """tx_sample_rate: Sample rate TX path in samples per second"""
-        return self._get_iio_attr("voltage0", "sampling_frequency", True)
+    def accel_x_calibscale(self):
+        """User scale adjustment for the x-axis."""
+        return self._get_iio_attr("accel_x", "calibscale", False)
+
+    @accel_x_calibscale.setter
+    def accel_x_calibscale(self, value):
+        self._set_iio_attr("accel_x", "calibscale", False, value)
+
+    # get accel_y related attributes
+    def get_accel_y(self):
+        """Value returned in m/s^2."""
+        return self.__get_scaled_sensor("accel_y")
+
+    accel_y = property(get_accel_y, None)
 
     @property
-    def trx_lo(self):
-        """trx_lo: Carrier frequency of TX and RX path"""
-        return self._get_iio_attr("altvoltage0", "frequency", True)
+    def accel_y_filter_low_pass_3db_frequency(self):
+        """Value returned in HZ."""
+        return self._get_iio_attr("accel_y", "filter_low_pass_3db_frequency", False)
 
-    @trx_lo.setter
-    def trx_lo(self, value):
-        self._set_iio_attr("altvoltage0", "frequency", True, value)
+    @accel_y_filter_low_pass_3db_frequency.setter
+    def accel_y_filter_low_pass_3db_frequency(self, value):
+        self._set_iio_attr("accel_y", "filter_low_pass_3db_frequency", False, value)
 
     @property
-    def jesd204_fsm_ctrl(self):
-        """jesd204_fsm_ctrl: jesd204-fsm control"""
-        return self._get_iio_dev_attr("jesd204_fsm_ctrl")
+    def accel_y_calibbias(self):
+        """User bias adjustment for the y-axis."""
+        return self._get_iio_attr("accel_y", "calibbias", False)
 
-    @jesd204_fsm_ctrl.setter
-    def jesd204_fsm_ctrl(self, value):
-        self._set_iio_dev_attr_str("jesd204_fsm_ctrl", value)
+    @accel_y_calibbias.setter
+    def accel_y_calibbias(self, value):
+        self._set_iio_attr("accel_y", "calibbias", False, value)
 
     @property
-    def jesd204_fsm_resume(self):
-        """jesd204_fsm_resume: jesd204-fsm resume"""
-        return self._get_iio_dev_attr("jesd204_fsm_resume")
+    def accel_y_calibscale(self):
+        """User scale adjustment for the y-axis."""
+        return self._get_iio_attr("accel_y", "calibscale", False)
 
-    @jesd204_fsm_resume.setter
-    def jesd204_fsm_resume(self, value):
-        self._set_iio_dev_attr_str("jesd204_fsm_resume", value)
+    @accel_y_calibscale.setter
+    def accel_y_calibscale(self, value):
+        self._set_iio_attr("accel_y", "calibscale", False, value)
+
+    # get accel_y related attributes
+    def get_accel_z(self):
+        """Value returned in m/s^2."""
+        return self.__get_scaled_sensor("accel_z")
+
+    accel_z = property(get_accel_z, None)
 
     @property
-    def jesd204_fsm_state(self):
-        """jesd204_fsm_state: jesd204-fsm state"""
-        return self._get_iio_dev_attr_str("jesd204_fsm_state")
+    def accel_z_filter_low_pass_3db_frequency(self):
+        """Value returned in HZ."""
+        return self._get_iio_attr("accel_z", "filter_low_pass_3db_frequency", False)
+
+    @accel_z_filter_low_pass_3db_frequency.setter
+    def accel_z_filter_low_pass_3db_frequency(self, value):
+        self._set_iio_attr("accel_z", "filter_low_pass_3db_frequency", False, value)
 
     @property
-    def jesd204_fsm_paused(self):
-        """jesd204_fsm_paused: jesd204-fsm paused"""
-        return self._get_iio_dev_attr("jesd204_fsm_paused")
+    def accel_z_calibbias(self):
+        """User bias adjustment for the z-axis."""
+        return self._get_iio_attr("accel_z", "calibbias", False)
+
+    @accel_z_calibbias.setter
+    def accel_z_calibbias(self, value):
+        self._set_iio_attr("accel_z", "calibbias", False, value)
 
     @property
-    def jesd204_fsm_error(self):
-        """jesd204_fsm_error: jesd204-fsm error"""
-        return self._get_iio_dev_attr("jesd204_fsm_error")
+    def accel_z_calibscale(self):
+        return self._get_iio_attr("accel_z", "calibscale", False)
+
+    @accel_z_calibscale.setter
+    def accel_z_calibscale(self, value):
+        """User scale adjustment for the z-axis."""
+        self._set_iio_attr("accel_z", "calibscale", False, value)
```

### Comparing `pyadi-iio-0.0.8/adi/dds.py` & `pyadi-iio-0.0.9/adi/dds.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/attribute.py` & `pyadi-iio-0.0.9/adi/attribute.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/rx_tx.py` & `pyadi-iio-0.0.9/adi/rx_tx.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     _ctrl: iio.Device = []
 
     def __del__(self):
         self._ctrl = []
 
 
 class rx(attribute):
-    """ Buffer handling for receive devices """
+    """Buffer handling for receive devices"""
 
     _rxadc: iio.Device = []
     _rx_channel_names: List[str] = []
     _complex_data = False
     _rx_data_type = np.int16
     _rx_data_si_type = np.int16
     _rx_mask = 0x0000
@@ -181,19 +181,43 @@
             sig.append(x[indx::stride] + 1j * x[indx + 1 :: stride])
             indx = indx + 2
         # Don't return list if a single channel
         if indx == 2:
             return sig[0]
         return sig
 
+    def __multi_type_rx(self, data):
+        """Process buffers with multiple data types"""
+        # Process each channel at a time
+        channel_bytes = []
+        curated_rx_type = []
+        for en_ch in self.rx_enabled_channels:
+            channel_bytes += [np.dtype(self._rx_data_type[en_ch]).itemsize]
+            curated_rx_type += [self._rx_data_type[en_ch]]
+        offset = 0
+        stride = sum(channel_bytes)
+        sig = []
+        for indx, chan_bytes in enumerate(channel_bytes):
+            bar = bytearray()
+            for bytesI in range(offset, len(data), stride):
+                bar.extend(data[bytesI : bytesI + chan_bytes])
+
+            sig.append(np.frombuffer(bar, dtype=curated_rx_type[indx]))
+            offset += chan_bytes
+        return sig
+
     def __rx_non_complex(self):
         if not self.__rxbuf:
             self._rx_init_channels()
         self.__rxbuf.refill()
         data = self.__rxbuf.read()
+
+        if isinstance(self._rx_data_type, list):
+            return self.__multi_type_rx(data)
+
         x = np.frombuffer(data, dtype=self._rx_data_type)
         if self._rx_mask != 0:
             x = np.bitwise_and(x, self._rx_mask)
         if self._rx_shift > 0:
             x = np.right_shift(x, self._rx_shift)
         elif self._rx_shift < 0:
             x = np.left_shift(x, -(self._rx_shift))
@@ -251,15 +275,15 @@
             if self._complex_data:
                 return self.__rx_complex()
             else:
                 return self.__rx_non_complex()
 
 
 class tx(dds, attribute):
-    """ Buffer handling for transmit devices """
+    """Buffer handling for transmit devices"""
 
     _tx_buffer_size = 1024
     _txdac: iio.Device = []
     _tx_channel_names: List[str] = []
     _complex_data = False
     __txbuf = None
```

### Comparing `pyadi-iio-0.0.8/adi/adar1000.py` & `pyadi-iio-0.0.9/adi/adar1000.py`

 * *Files 1% similar despite different names*

```diff
@@ -1601,34 +1601,14 @@
     @property
     def tx_elevation_phi(self):
         """ Get the Tx elevation phi angle for the array in degrees """
         return self._tx_elevation_phi
 
     """ Private Methods """
 
-    def _calculate_phi(self, azimuth, elevation):
-        """Calculate the Φ angles to steer the array in a particular direction. This method assumes that the entire
-        array is one analog beam.
-        parameters:
-            azimuth: float
-                Desired beam angle in degrees for the horizontal direction.
-            elevation: float
-                Desired beam angle in degrees for the vertical direction.
-        """
-
-        # Convert the input angles to radians
-        az_rads = azimuth * pi / 180
-        el_rads = elevation * pi / 180
-
-        # Calculate the phase increment (Φ) for each element in the array in both directions (in degrees)
-        az_phi = 2 * self.frequency * self.element_spacing * sin(az_rads) * 180 / 3e8
-        el_phi = 2 * self.frequency * self.element_spacing * sin(el_rads) * 180 / 3e8
-
-        return az_phi, el_phi
-
     def _steer(self, rx_or_tx, azimuth, elevation):
         """Steer the array
         parameters:
             rx_or_tx: string
                 Sets which parameters are updated, Rx or Tx.
             azimuth: float
                 Desired beam angle in degrees for the horizontal direction
@@ -1636,15 +1616,15 @@
                 Desired beam angle in degrees for the vertical direction
         """
 
         # Clean up the rx_or_tx variable
         rx_or_tx = rx_or_tx.strip().lower()
 
         # Calculate the Φ angles for each element in both directions (in degrees)
-        azimuth_phi, elevation_phi = self._calculate_phi(azimuth, elevation)
+        azimuth_phi, elevation_phi = self.calculate_phi(azimuth, elevation)
 
         # Update the class variables
         if rx_or_tx == "rx":
             self._rx_azimuth = azimuth
             self._rx_elevation = elevation
             self._rx_azimuth_phi = azimuth_phi
             self._rx_elevation_phi = elevation_phi
@@ -1669,18 +1649,50 @@
         if rx_or_tx == "rx":
             self.latch_rx_settings()
         else:
             self.latch_tx_settings()
 
     """ Public Methods """
 
-    def initialize_devices(self):
-        """ Initialize the ADAR1000s in the array """
+    def calculate_phi(self, azimuth, elevation):
+        """Calculate the Φ angles to steer the array in a particular direction. This method assumes that the entire
+        array is one analog beam.
+        parameters:
+            azimuth: float
+                Desired beam angle in degrees for the horizontal direction.
+            elevation: float
+                Desired beam angle in degrees for the vertical direction.
+        """
+
+        # Convert the input angles to radians
+        az_rads = azimuth * pi / 180
+        el_rads = elevation * pi / 180
+
+        # Calculate the phase increment (Φ) for each element in the array in both directions (in degrees)
+        az_phi = 2 * self.frequency * self.element_spacing * sin(az_rads) * 180 / 3e8
+        el_phi = 2 * self.frequency * self.element_spacing * sin(el_rads) * 180 / 3e8
+
+        return az_phi, el_phi
+
+    def initialize_devices(self, pa_off=-2.5, pa_on=-2.5, lna_off=-2, lna_on=-2):
+        """Suggested initialization routine after powerup
+        parameters:
+            pa_off: float
+                Voltage to set the PA_BIAS_OFF values to during initialization
+            pa_on: float
+                Voltage to set the PA_BIAS_ON values to during initialization
+            lna_off: float
+                Voltage to set the LNA_BIAS_OFF values to during initialization
+            lna_on: float
+                Voltage to set the LNA_BIAS_ON values to during initialization
+        """
         for device in self.devices.values():
-            device.initialize()
+            device.initialize(
+                pa_off=pa_off, pa_on=pa_on, lna_off=lna_off, lna_on=lna_on
+            )
 
     def latch_rx_settings(self):
         """ Latch in new Gain/Phase settings for the Rx """
         for device in self.devices.values():
             device.latch_rx_settings()
 
     def latch_tx_settings(self):
```

### Comparing `pyadi-iio-0.0.8/adi/context_manager.py` & `pyadi-iio-0.0.9/adi/context_manager.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/cn0532.py` & `pyadi-iio-0.0.9/adi/cn0532.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/adxrs290.py` & `pyadi-iio-0.0.9/adi/adxrs290.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad5627.py` & `pyadi-iio-0.0.9/adi/ad5627.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad5686.py` & `pyadi-iio-0.0.9/adi/ad5686.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/adxl345.py` & `pyadi-iio-0.0.9/adi/adxl345.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad7606.py` & `pyadi-iio-0.0.9/adi/ad7606.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/adpd410x.py` & `pyadi-iio-0.0.9/adi/adpd410x.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad7746.py` & `pyadi-iio-0.0.9/adi/ad7746.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/__init__.py` & `pyadi-iio-0.0.9/adi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 
 from adi.adrv9009_zu11eg_fmcomms8 import adrv9009_zu11eg_fmcomms8
 
 from adi.ad9081 import ad9081
 
 from adi.ad9081_mc import ad9081_mc, QuadMxFE
 
+from adi.ad9083 import ad9083
+
 from adi.ad9094 import ad9094
 
 from adi.ad9680 import ad9680
 
 from adi.ad9136 import ad9136
 
 from adi.ad9144 import ad9144
@@ -65,14 +67,16 @@
 
 from adi.daq2 import DAQ2
 
 from adi.daq3 import DAQ3
 
 from adi.adis16460 import adis16460
 
+from adi.adis16495 import adis16495
+
 from adi.adis16507 import adis16507
 
 from adi.ad7124 import ad7124
 
 from adi.adxl345 import adxl345
 
 from adi.adxrs290 import adxrs290
@@ -95,14 +99,18 @@
 
 from adi.ad7746 import ad7746
 
 from adi.adpd410x import adpd410x
 
 from adi.ad7689 import ad7689
 
+from adi.adf4371 import adf4371
+
+from adi.adpd188 import adpd188
+
 try:
     from adi.jesd import jesd
 except ImportError:
     pass
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 name = "Analog Devices Hardware Interfaces"
```

### Comparing `pyadi-iio-0.0.8/adi/adis16460.py` & `pyadi-iio-0.0.9/adi/adis16460.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/adrv9009_zu11eg_multi.py` & `pyadi-iio-0.0.9/adi/adrv9009_zu11eg_multi.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad7124.py` & `pyadi-iio-0.0.9/adi/ad7124.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad9081_mc.py` & `pyadi-iio-0.0.9/adi/ad9081_mc.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad9081.py` & `pyadi-iio-0.0.9/adi/ad9081.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/fmcomms5.py` & `pyadi-iio-0.0.9/adi/fmcomms5.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad9680.py` & `pyadi-iio-0.0.9/adi/ad9680.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad7689.py` & `pyadi-iio-0.0.9/adi/ad7689.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad9136.py` & `pyadi-iio-0.0.9/adi/ad9136.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/adrv9009_zu11eg_fmcomms8.py` & `pyadi-iio-0.0.9/adi/adrv9009_zu11eg_fmcomms8.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/cn0540.py` & `pyadi-iio-0.0.9/adi/cn0540.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,43 +34,58 @@
 import time
 
 import numpy as np
 from adi.context_manager import context_manager
 from adi.rx_tx import rx
 
 
+def reset_buffer(func):
+    """Wrapper for set calls which require the SPI engine.
+    Without disabling the buffer the DMA would block forever
+    """
+
+    def wrapper(*args, **kwargs):
+        if args[0]._reset_on_spi_writes:
+            args[0].rx_destroy_buffer()
+        func(*args, **kwargs)
+
+    return wrapper
+
+
 class cn0540(rx, context_manager):
-    """ CN0540 CBM DAQ Board """
+    """CN0540 CBM DAQ Board"""
 
     _rx_data_type = np.int32
     _rx_data_si_type = np.float
     _complex_data = False
     _rx_channel_names = ["voltage0"]
     _device_name = ""
     _rx_shift = 8
     _fda_mode_options = ["low-power", "full-power"]
     _dac_buffer_gain = 1.22
     _g = 0.3
     _fda_gain = 2.667
     _fda_vocm_mv = 2500
+    _reset_on_spi_writes = True
 
     def __init__(self, uri=""):
 
         context_manager.__init__(self, uri, self._device_name)
 
         self._rxadc = self._ctx.find_device("ad7768-1")
         self._ctrl = self._ctx.find_device("ad7768-1")
         self._ltc2606 = self._ctx.find_device("ltc2606")
         self._gpio = self._ctx.find_device("one-bit-adc-dac")
         self._ltc2308 = self._ctx.find_device("ltc2308")
 
         rx.__init__(self)
 
+    @reset_buffer
     def calibrate(self):
-        """ Tune LTC2606 to make AD7768-1 ADC codes zero mean """
+        """Tune LTC2606 to make AD7768-1 ADC codes zero mean"""
         adc_chan = self._rxadc
         dac_chan = self._ltc2606
         adc_scale = float(self._get_iio_attr("voltage0", "scale", False, adc_chan))
         dac_scale = float(self._get_iio_attr("voltage0", "scale", True, dac_chan))
 
         for _ in range(20):
             raw = self._get_iio_attr("voltage0", "raw", False, adc_chan)
@@ -89,103 +104,105 @@
         """sample_rate: Sample rate in samples per second.
         Valid options are:
         '256000','128000','64000','32000','16000','8000','4000','2000','1000'
         """
         return self._get_iio_dev_attr("sampling_frequency")
 
     @sample_rate.setter
+    @reset_buffer
     def sample_rate(self, value):
         self._set_iio_dev_attr_str("sampling_frequency", value)
 
     @property
     def input_voltage(self):
-        """input_voltage: Input voltage in mV from ADC before shift voltage applied """
+        """input_voltage: Input voltage in mV from ADC before shift voltage applied"""
         adc_chan = self._rxadc
         adc_scale = float(self._get_iio_attr("voltage0", "scale", False, adc_chan))
         raw = self._get_iio_attr("voltage0", "raw", False, adc_chan)
         return raw * adc_scale * self._dac_buffer_gain
 
     @property
     def shift_voltage(self):
-        """shift_voltage: Shift voltage in mV from LTC2606 to bias sensor data """
+        """shift_voltage: Shift voltage in mV from LTC2606 to bias sensor data"""
         dac_chan = self._ltc2606
         dac_scale = float(self._get_iio_attr("voltage0", "scale", True, dac_chan))
         raw = self._get_iio_attr("voltage0", "raw", True, dac_chan)
         return raw * dac_scale * self._dac_buffer_gain
 
     @shift_voltage.setter
+    @reset_buffer
     def shift_voltage(self, value):
         dac_chan = self._ltc2606
         dac_scale = float(self._get_iio_attr("voltage0", "scale", True, dac_chan))
         raw = value / (dac_scale * self._dac_buffer_gain)
         self._set_iio_attr_int("voltage0", "raw", True, int(raw), dac_chan)
 
     @property
     def sensor_voltage(self):
-        """sensor_voltage: Sensor voltage in mV read from ADC after biasing """
+        """sensor_voltage: Sensor voltage in mV read from ADC after biasing"""
         adc_chan = self._rxadc
         adc_scale = float(self._get_iio_attr("voltage0", "scale", False, adc_chan))
         raw = self._get_iio_attr("voltage0", "raw", False, adc_chan)
 
         v1_st = self._fda_vocm_mv - raw * adc_scale / self._fda_gain
         vsensor_mv = (((self._g + 1) * self.shift_voltage) - v1_st) / self._g
 
         raw = self._get_iio_attr("voltage0", "raw", False, adc_chan)
         vsensor_mv -= raw * adc_scale
         return vsensor_mv
 
-    # Not functional with current hardware
-    # @property
-    # def sw_ff_status(self):
-    #     """sw_ff_status: Fault flag status """
-    #     return self._get_iio_attr("voltage0", "raw", False, self._gpio)
+    @property
+    def sw_ff_status(self):
+        """sw_ff_status: Fault flag status"""
+        return self._get_iio_attr("voltage0", "raw", False, self._gpio)
 
     @property
     def monitor_powerup(self):
-        """monitor_powerup: Shutdown pin is tied to active-low inputs """
+        """monitor_powerup: Shutdown pin is tied to active-low inputs"""
         return self._get_iio_attr("voltage2", "raw", True, self._gpio)
 
     @monitor_powerup.setter
     def monitor_powerup(self, value):
         self._set_iio_attr_int("voltage2", "raw", True, value, self._gpio)
 
     @property
     def fda_disable_status(self):
-        """fda_disable_status: Amplifier disable status """
+        """fda_disable_status: Amplifier disable status"""
         return self._get_iio_attr("voltage5", "raw", True, self._gpio)
 
     @fda_disable_status.setter
+    @reset_buffer
     def fda_disable_status(self, value):
         self._set_iio_attr_int("voltage5", "raw", True, value, self._gpio)
 
     @property
     def fda_mode(self):
-        """fda_mode: Amplifier mode. Options are low-power or full-power """
+        """fda_mode: Amplifier mode. Options are low-power or full-power"""
         return self._fda_mode_options[
             int(self._get_iio_attr("voltage6", "raw", True, self._gpio))
         ]
 
     @fda_mode.setter
     def fda_mode(self, value):
         if value not in ["full-power", "low-power"]:
             raise Exception("fda_mode must be low-power or full-power")
         self._set_iio_attr_int(
             "voltage6", "raw", True, int(value == "full-power"), self._gpio
         )
 
     @property
     def red_led_enable(self):
-        """red_led_enable: Enable red LED on board """
+        """red_led_enable: Enable red LED on board"""
         return self._get_iio_attr("voltage1", "raw", True, self._gpio)
 
     @red_led_enable.setter
     def red_led_enable(self, value):
         self._set_iio_attr_int("voltage1", "raw", True, value, self._gpio)
 
     @property
-    def blue_led_enable(self):
-        """blue_led_enable: Enable blue LED on board """
+    def sw_cc(self):
+        """sw_cc: Enable SW_CC. This will also illuminate the blue LED."""
         return self._get_iio_attr("voltage0", "raw", True, self._gpio)
 
-    @blue_led_enable.setter
-    def blue_led_enable(self, value):
+    @sw_cc.setter
+    def sw_cc(self, value):
         self._set_iio_attr_int("voltage0", "raw", True, value, self._gpio)
```

### Comparing `pyadi-iio-0.0.8/adi/ad7799.py` & `pyadi-iio-0.0.9/adi/ad7799.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/daq3.py` & `pyadi-iio-0.0.9/adi/daq3.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/sshfs.py` & `pyadi-iio-0.0.9/adi/sshfs.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ltc2983.py` & `pyadi-iio-0.0.9/adi/ltc2983.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad9371.py` & `pyadi-iio-0.0.9/adi/ad9371.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad9152.py` & `pyadi-iio-0.0.9/adi/ad9152.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/daq2.py` & `pyadi-iio-0.0.9/adi/daq2.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/adrv9009_zu11eg.py` & `pyadi-iio-0.0.9/adi/adrv9009_zu11eg.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/jesd.py` & `pyadi-iio-0.0.9/adi/jesd.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad9094.py` & `pyadi-iio-0.0.9/adi/ad9094.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ltc2314_14.py` & `pyadi-iio-0.0.9/adi/ltc2314_14.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad9144.py` & `pyadi-iio-0.0.9/adi/ad9144.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/ad936x.py` & `pyadi-iio-0.0.9/adi/ad936x.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/one_bit_adc_dac.py` & `pyadi-iio-0.0.9/adi/one_bit_adc_dac.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/adi/adrv9002.py` & `pyadi-iio-0.0.9/adi/adrv9002.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/setup.py` & `pyadi-iio-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,14 @@
     author_email="travis.collins@analog.com",
     description="Interfaces to stream data from ADI hardware",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/analogdevicesinc/pyadi-iio",
     packages=setuptools.find_packages(exclude=["test*"]),
     python_requires=">=3.6",
-    install_requires=["numpy", "pylibiio", "paramiko"],
+    install_requires=["numpy", "pylibiio<=0.21", "paramiko"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `pyadi-iio-0.0.8/PKG-INFO` & `pyadi-iio-0.0.9/pyadi_iio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyadi-iio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interfaces to stream data from ADI hardware
 Home-page: https://github.com/analogdevicesinc/pyadi-iio
 Author: Travis Collins
 Author-email: travis.collins@analog.com
 License: UNKNOWN
 Description: <!-- PYADI-IIO README -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyadi-iio Version: 0.0.8 Summary: Interfaces to
+Metadata-Version: 2.1 Name: pyadi-iio Version: 0.0.9 Summary: Interfaces to
 stream data from ADI hardware Home-page: https://github.com/analogdevicesinc/
 pyadi-iio Author: Travis Collins Author-email: travis.collins@analog.com
 License: UNKNOWN Description:
                                [PyADI-IIO Logo]
          [Build_Status] [PyPI_version] [Codacy_Badge] [Python_Version]
                   [GitHub_Pages] [EngineerZone] [Analog_Wiki]
 --- ### pyadi-iio: Analog Devices python interfaces for hardware with
```

### Comparing `pyadi-iio-0.0.8/README.md` & `pyadi-iio-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_ad7606.py` & `pyadi-iio-0.0.9/test/test_ad7606.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_ad9364_p.py` & `pyadi-iio-0.0.9/test/test_ad9364_p.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_adrv9009_p.py` & `pyadi-iio-0.0.9/test/test_pluto_p.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,244 +1,231 @@
 import pytest
 
-try:
-    import adi.jesd
-
-    skip_jesd = False
-except:
-    skip_jesd = True
-
-
-hardware = "adrv9009"
-classname = "adi.adrv9009"
+hardware = ["pluto", "adrv9361", "fmcomms2"]
+classname = "adi.Pluto"
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize(
-    "attr, start, stop, step, tol",
+    "attr, start, stop, step, tol, repeats",
     [
-        ("tx_hardwaregain_chan0", -41.95, 0.0, 0.05, 0.05),
-        ("tx_hardwaregain_chan1", -41.95, 0.0, 0.05, 0.05),
-        ("trx_lo", 70000000, 6000000000, 1000, 0),
+        ("tx_hardwaregain_chan0", -89.75, 0.0, 0.25, 0, 100),
+        ("rx_lo", 325000000, 3800000000, 1, 8, 100),
+        ("tx_lo", 325000000, 3800000000, 1, 8, 100),
+        ("sample_rate", 2084000, 61440000, 1, 4, 100),
     ],
 )
-def test_adrv9009_attr(
-    test_attribute_single_value, iio_uri, classname, attr, start, stop, step, tol
+def test_pluto_attr(
+    test_attribute_single_value,
+    iio_uri,
+    classname,
+    attr,
+    start,
+    stop,
+    step,
+    tol,
+    repeats,
 ):
-    test_attribute_single_value(iio_uri, classname, attr, start, stop, step, tol)
+    test_attribute_single_value(
+        iio_uri, classname, attr, start, stop, step, tol, repeats
+    )
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", range(2))
-def test_adrv9009_rx_data(test_dma_rx, iio_uri, classname, channel):
+@pytest.mark.parametrize("attr, tol", [("loopback", 0)])
+@pytest.mark.parametrize("val", [0, 1, 2])
+def test_pluto_loopback_attr(
+    test_attribute_single_value_str, iio_uri, classname, attr, val, tol
+):
+    test_attribute_single_value_str(iio_uri, classname, attr, val, tol)
+
+
+#########################################
+@pytest.mark.iio_hardware(hardware)
+@pytest.mark.parametrize("classname", [(classname)])
+@pytest.mark.parametrize("channel", [0])
+def test_pluto_rx_data(test_dma_rx, iio_uri, classname, channel):
     test_dma_rx(iio_uri, classname, channel)
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0, 1])
+@pytest.mark.parametrize("channel", [0])
+def test_pluto_tx_data(test_dma_tx, iio_uri, classname, channel):
+    test_dma_tx(iio_uri, classname, channel)
+
+
+#########################################
+@pytest.mark.iio_hardware(hardware)
+@pytest.mark.parametrize("classname", [(classname)])
+@pytest.mark.parametrize("channel", [0])
 @pytest.mark.parametrize(
     "param_set",
     [
         dict(
-            trx_lo=1000000000,
-            gain_control_mode_chan0="slow_attack",
-            gain_control_mode_chan1="slow_attack",
-            tx_hardwaregain_chan0=-10,
-            tx_hardwaregain_chan1=-10,
-            calibrate_rx_qec_en=1,
-            calibrate_tx_qec_en=1,
-            calibrate=1,
-        ),
-        dict(
-            trx_lo=3000000000,
+            tx_lo=1000000000,
+            rx_lo=1000000000,
             gain_control_mode_chan0="slow_attack",
-            gain_control_mode_chan1="slow_attack",
-            tx_hardwaregain_chan0=-10,
-            tx_hardwaregain_chan1=-10,
-            calibrate_rx_qec_en=1,
-            calibrate_tx_qec_en=1,
-            calibrate=1,
-        ),
-        dict(
-            trx_lo=5000000000,
-            gain_control_mode_chan0="slow_attack",
-            gain_control_mode_chan1="slow_attack",
-            tx_hardwaregain_chan0=-10,
-            tx_hardwaregain_chan1=-10,
-            calibrate_rx_qec_en=1,
-            calibrate_tx_qec_en=1,
-            calibrate=1,
-        ),
+            tx_hardwaregain_chan0=-20,
+            sample_rate=4000000,
+        )
     ],
 )
-@pytest.mark.parametrize("sfdr_min", [45])
-def test_adrv9009_sfdr(test_sfdr, iio_uri, classname, channel, param_set, sfdr_min):
-    test_sfdr(iio_uri, classname, channel, param_set, sfdr_min)
+def test_pluto_cyclic_buffers(
+    test_cyclic_buffer, iio_uri, classname, channel, param_set
+):
+    test_cyclic_buffer(iio_uri, classname, channel, param_set)
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0, 1])
+@pytest.mark.parametrize("channel", [0])
 @pytest.mark.parametrize(
     "param_set",
     [
         dict(
-            trx_lo=1000000000,
+            tx_lo=1000000000,
+            rx_lo=1000000000,
             gain_control_mode_chan0="slow_attack",
-            gain_control_mode_chan1="slow_attack",
-            tx_hardwaregain_chan0=-10,
-            tx_hardwaregain_chan1=-10,
-            calibrate_rx_qec_en=1,
-            calibrate_tx_qec_en=1,
-            calibrate=1,
-        ),
-        dict(
-            trx_lo=3000000000,
-            gain_control_mode_chan0="slow_attack",
-            gain_control_mode_chan1="slow_attack",
-            tx_hardwaregain_chan0=-10,
-            tx_hardwaregain_chan1=-10,
-            calibrate_rx_qec_en=1,
-            calibrate_tx_qec_en=1,
-            calibrate=1,
-        ),
+            tx_hardwaregain_chan0=-20,
+            sample_rate=4000000,
+        )
+    ],
+)
+def test_pluto_cyclic_buffers_exception(
+    test_cyclic_buffer_exception, iio_uri, classname, channel, param_set
+):
+    test_cyclic_buffer_exception(iio_uri, classname, channel, param_set)
+
+
+#########################################
+@pytest.mark.iio_hardware(hardware)
+@pytest.mark.parametrize("classname", [(classname)])
+@pytest.mark.parametrize("channel", [0])
+def test_pluto_loopback(test_dma_loopback, iio_uri, classname, channel):
+    test_dma_loopback(iio_uri, classname, channel)
+
+
+#########################################
+@pytest.mark.iio_hardware(hardware)
+@pytest.mark.parametrize("classname", [(classname)])
+@pytest.mark.parametrize("channel", [0])
+@pytest.mark.parametrize(
+    "param_set",
+    [
         dict(
-            trx_lo=5000000000,
+            tx_lo=1000000000,
+            rx_lo=1000000000,
             gain_control_mode_chan0="slow_attack",
-            gain_control_mode_chan1="slow_attack",
-            tx_hardwaregain_chan0=-10,
-            tx_hardwaregain_chan1=-10,
-            calibrate_rx_qec_en=1,
-            calibrate_tx_qec_en=1,
-            calibrate=1,
-        ),
+            tx_hardwaregain_chan0=-20,
+            sample_rate=4000000,
+        )
     ],
 )
-@pytest.mark.parametrize("dds_scale, min_rssi, max_rssi", [(0, 35, 60), (0.9, 0, 22)])
-def test_adrv9009_dds_gain_check_agc(
-    test_gain_check,
-    iio_uri,
-    classname,
-    channel,
-    param_set,
-    dds_scale,
-    min_rssi,
-    max_rssi,
-):
-    test_gain_check(
-        iio_uri, classname, channel, param_set, dds_scale, min_rssi, max_rssi
-    )
+@pytest.mark.parametrize("sfdr_min", [40])
+def test_pluto_sfdr(test_sfdr, iio_uri, classname, channel, param_set, sfdr_min):
+    test_sfdr(iio_uri, classname, channel, param_set, sfdr_min)
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0, 1, 2, 3])
+@pytest.mark.parametrize("channel", [0])
+@pytest.mark.parametrize("frequency, scale", [(1000000, 1)])
 @pytest.mark.parametrize(
-    "param_set, dds_scale, min_rssi, max_rssi",
+    "param_set",
     [
-        (
-            dict(
-                trx_lo=1000000000,
-                gain_control_mode_chan0="manual",
-                gain_control_mode_chan1="manual",
-                rx_hardwaregain_chan0=0,
-                rx_hardwaregain_chan1=0,
-                tx_hardwaregain_chan0=-10,
-                tx_hardwaregain_chan1=-10,
-                calibrate_tx_qec_en=1,
-                calibrate=1,
-            ),
-            0.5,
-            20,
-            60,
-        ),
-        (
-            dict(
-                trx_lo=1000000000,
-                gain_control_mode_chan0="manual",
-                gain_control_mode_chan1="manual",
-                rx_hardwaregain_chan0=30,
-                rx_hardwaregain_chan1=30,
-                tx_hardwaregain_chan0=-10,
-                tx_hardwaregain_chan1=-10,
-                calibrate_tx_qec_en=1,
-                calibrate=1,
-            ),
-            0.5,
-            0,
-            15,
-        ),
+        dict(
+            tx_lo=1000000000,
+            rx_lo=1000000000,
+            gain_control_mode_chan0="slow_attack",
+            tx_hardwaregain_chan0=-30,
+            sample_rate=4000000,
+        )
     ],
 )
-def test_adrv9009_dds_gain_check_vary_power(
-    test_gain_check,
+@pytest.mark.parametrize("peak_min", [-40])
+def test_pluto_dds_loopback(
+    test_dds_loopback,
     iio_uri,
     classname,
-    channel,
     param_set,
-    dds_scale,
-    min_rssi,
-    max_rssi,
+    channel,
+    frequency,
+    scale,
+    peak_min,
 ):
-    test_gain_check(
-        iio_uri, classname, channel, param_set, dds_scale, min_rssi, max_rssi
+    test_dds_loopback(
+        iio_uri, classname, param_set, channel, frequency, scale, peak_min
     )
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0, 1, 2, 3])
+@pytest.mark.parametrize("channel", [0])
 @pytest.mark.parametrize(
     "param_set",
     [
         dict(
-            trx_lo=1000000000,
+            tx_lo=1000000000,
+            rx_lo=1000000000,
             gain_control_mode_chan0="slow_attack",
-            gain_control_mode_chan1="slow_attack",
             tx_hardwaregain_chan0=-20,
-            tx_hardwaregain_chan1=-20,
-            calibrate_tx_qec_en=1,
-            calibrate=1,
+            sample_rate=4000000,
         ),
         dict(
-            trx_lo=3000000000,
+            tx_lo=2000000000,
+            rx_lo=2000000000,
             gain_control_mode_chan0="slow_attack",
-            gain_control_mode_chan1="slow_attack",
             tx_hardwaregain_chan0=-20,
-            tx_hardwaregain_chan1=-20,
-            calibrate_tx_qec_en=1,
-            calibrate=1,
+            sample_rate=4000000,
         ),
         dict(
-            trx_lo=5000000000,
-            trx_lo_chip_b=1000000000,
+            tx_lo=3000000000,
+            rx_lo=3000000000,
             gain_control_mode_chan0="slow_attack",
-            gain_control_mode_chan1="slow_attack",
             tx_hardwaregain_chan0=-20,
-            tx_hardwaregain_chan1=-20,
-            calibrate_tx_qec_en=1,
-            calibrate=1,
+            sample_rate=4000000,
         ),
     ],
 )
-def test_adrv9009_iq_loopback(test_iq_loopback, iio_uri, classname, channel, param_set):
+def test_pluto_iq_loopback(test_iq_loopback, iio_uri, classname, channel, param_set):
     test_iq_loopback(iio_uri, classname, channel, param_set)
 
 
 #########################################
-@pytest.mark.skipif(skip_jesd, reason="JESD module not importable")
 @pytest.mark.iio_hardware(hardware)
-def test_adrv9009_jesd(iio_uri):
-    import adi
+@pytest.mark.parametrize("classname", [(classname)])
+@pytest.mark.parametrize("channel", [0])
+def test_pluto_loopback_zeros(test_dma_dac_zeros, iio_uri, classname, channel):
+    test_dma_dac_zeros(iio_uri, classname, channel)
 
-    sdr = adi.adrv9009(uri=iio_uri, jesd_monitor=True)
-    info = sdr._jesd.get_all_statuses()
-    assert info
+
+#########################################
+@pytest.mark.iio_hardware(hardware)
+@pytest.mark.parametrize("classname", [(classname)])
+@pytest.mark.parametrize("channel", [0])
+@pytest.mark.parametrize("buffer_size", [2 ** 20])
+@pytest.mark.parametrize("sample_rate", [600e3])
+def test_pluto_verify_overflow(
+    test_verify_overflow, iio_uri, classname, channel, buffer_size, sample_rate
+):
+    test_verify_overflow(iio_uri, classname, channel, buffer_size, sample_rate)
+
+
+#########################################
+@pytest.mark.iio_hardware(hardware)
+@pytest.mark.parametrize("classname", [(classname)])
+@pytest.mark.parametrize("channel", [0])
+@pytest.mark.parametrize("buffer_size", [2 ** 20])
+@pytest.mark.parametrize("sample_rate", [600e3])
+def test_pluto_verify_underflow(
+    test_verify_underflow, iio_uri, classname, channel, buffer_size, sample_rate
+):
+    test_verify_underflow(iio_uri, classname, channel, buffer_size, sample_rate)
```

### Comparing `pyadi-iio-0.0.8/test/test_fmcomms5_p.py` & `pyadi-iio-0.0.9/test/test_fmcomms5_p.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_ad7799.py` & `pyadi-iio-0.0.9/test/test_ad7799.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_stress.py` & `pyadi-iio-0.0.9/test/test_stress.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_adrv9009_zu11eg_fmcomms8.py` & `pyadi-iio-0.0.9/test/test_adrv9009_zu11eg_fmcomms8.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_adrv9002_generic_p.py` & `pyadi-iio-0.0.9/test/test_adrv9002_generic_p.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_daq2_p.py` & `pyadi-iio-0.0.9/test/test_daq2_p.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_generic.py` & `pyadi-iio-0.0.9/test/test_generic.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_pluto_p.py` & `pyadi-iio-0.0.9/test/test_ad9361_p.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import pytest
 
-hardware = ["pluto", "adrv9361", "fmcomms2"]
-classname = "adi.Pluto"
+hardware = ["packrf", "adrv9361", "fmcomms2", "ad9361"]
+classname = "adi.ad9361"
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize(
     "attr, start, stop, step, tol, repeats",
     [
         ("tx_hardwaregain_chan0", -89.75, 0.0, 0.25, 0, 100),
-        ("rx_lo", 325000000, 3800000000, 1, 8, 100),
-        ("tx_lo", 325000000, 3800000000, 1, 8, 100),
-        ("sample_rate", 2084000, 61440000, 1, 4, 100),
+        ("tx_hardwaregain_chan1", -89.75, 0.0, 0.25, 0, 100),
+        ("rx_lo", 70000000, 6000000000, 1, 8, 100),
+        ("tx_lo", 47000000, 6000000000, 1, 8, 100),
+        ("sample_rate", 2084000, 61440000, 1, 4, 20),
     ],
 )
-def test_pluto_attr(
+def test_ad9361_attr(
     test_attribute_single_value,
     iio_uri,
     classname,
     attr,
     start,
     stop,
     step,
@@ -33,175 +34,98 @@
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize("attr, tol", [("loopback", 0)])
 @pytest.mark.parametrize("val", [0, 1, 2])
-def test_pluto_loopback_attr(
+def test_ad9361_loopback_attr(
     test_attribute_single_value_str, iio_uri, classname, attr, val, tol
 ):
     test_attribute_single_value_str(iio_uri, classname, attr, val, tol)
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0])
-def test_pluto_rx_data(test_dma_rx, iio_uri, classname, channel):
+@pytest.mark.parametrize("channel", [0, 1, [0, 1]])
+def test_ad9361_rx_data(test_dma_rx, iio_uri, classname, channel):
     test_dma_rx(iio_uri, classname, channel)
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0])
-def test_pluto_tx_data(test_dma_tx, iio_uri, classname, channel):
+@pytest.mark.parametrize("channel", [0, 1, [0, 1]])
+def test_ad9361_tx_data(test_dma_tx, iio_uri, classname, channel):
     test_dma_tx(iio_uri, classname, channel)
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0])
-@pytest.mark.parametrize(
-    "param_set",
-    [
-        dict(
-            tx_lo=1000000000,
-            rx_lo=1000000000,
-            gain_control_mode_chan0="slow_attack",
-            tx_hardwaregain_chan0=-20,
-            sample_rate=4000000,
-        )
-    ],
-)
-def test_pluto_cyclic_buffers(
-    test_cyclic_buffer, iio_uri, classname, channel, param_set
-):
-    test_cyclic_buffer(iio_uri, classname, channel, param_set)
-
-
-#########################################
-@pytest.mark.iio_hardware(hardware)
-@pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0])
-@pytest.mark.parametrize(
-    "param_set",
-    [
-        dict(
-            tx_lo=1000000000,
-            rx_lo=1000000000,
-            gain_control_mode_chan0="slow_attack",
-            tx_hardwaregain_chan0=-20,
-            sample_rate=4000000,
-        )
-    ],
-)
-def test_pluto_cyclic_buffers_exception(
-    test_cyclic_buffer_exception, iio_uri, classname, channel, param_set
-):
-    test_cyclic_buffer_exception(iio_uri, classname, channel, param_set)
-
-
-#########################################
-@pytest.mark.iio_hardware(hardware)
-@pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0])
-def test_pluto_loopback(test_dma_loopback, iio_uri, classname, channel):
+@pytest.mark.parametrize("channel", [0, 1])
+def test_ad9361_loopback(test_dma_loopback, iio_uri, classname, channel):
     test_dma_loopback(iio_uri, classname, channel)
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize("channel", [0])
 @pytest.mark.parametrize(
     "param_set",
     [
         dict(
+            sample_rate=4000000,
             tx_lo=1000000000,
             rx_lo=1000000000,
             gain_control_mode_chan0="slow_attack",
             tx_hardwaregain_chan0=-20,
-            sample_rate=4000000,
+            gain_control_mode_chan1="slow_attack",
+            tx_hardwaregain_chan1=-20,
         )
     ],
 )
 @pytest.mark.parametrize("sfdr_min", [40])
-def test_pluto_sfdr(test_sfdr, iio_uri, classname, channel, param_set, sfdr_min):
+def test_ad9361_sfdr(test_sfdr, iio_uri, classname, channel, param_set, sfdr_min):
     test_sfdr(iio_uri, classname, channel, param_set, sfdr_min)
 
 
 #########################################
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0])
-@pytest.mark.parametrize("frequency, scale", [(1000000, 1)])
+@pytest.mark.parametrize("channel", [0, 1])
 @pytest.mark.parametrize(
     "param_set",
     [
         dict(
-            tx_lo=1000000000,
-            rx_lo=1000000000,
-            gain_control_mode_chan0="slow_attack",
-            tx_hardwaregain_chan0=-30,
             sample_rate=4000000,
-        )
-    ],
-)
-@pytest.mark.parametrize("peak_min", [-40])
-def test_pluto_dds_loopback(
-    test_dds_loopback,
-    iio_uri,
-    classname,
-    param_set,
-    channel,
-    frequency,
-    scale,
-    peak_min,
-):
-    test_dds_loopback(
-        iio_uri, classname, param_set, channel, frequency, scale, peak_min
-    )
-
-
-#########################################
-@pytest.mark.iio_hardware(hardware)
-@pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0])
-@pytest.mark.parametrize(
-    "param_set",
-    [
-        dict(
             tx_lo=1000000000,
             rx_lo=1000000000,
             gain_control_mode_chan0="slow_attack",
             tx_hardwaregain_chan0=-20,
-            sample_rate=4000000,
+            gain_control_mode_chan1="slow_attack",
+            tx_hardwaregain_chan1=-20,
         ),
         dict(
+            sample_rate=4000000,
             tx_lo=2000000000,
             rx_lo=2000000000,
             gain_control_mode_chan0="slow_attack",
             tx_hardwaregain_chan0=-20,
-            sample_rate=4000000,
+            gain_control_mode_chan1="slow_attack",
+            tx_hardwaregain_chan1=-20,
         ),
         dict(
+            sample_rate=4000000,
             tx_lo=3000000000,
             rx_lo=3000000000,
             gain_control_mode_chan0="slow_attack",
             tx_hardwaregain_chan0=-20,
-            sample_rate=4000000,
+            gain_control_mode_chan1="slow_attack",
+            tx_hardwaregain_chan1=-20,
         ),
     ],
 )
-def test_pluto_iq_loopback(test_iq_loopback, iio_uri, classname, channel, param_set):
+def test_ad9361_iq_loopback(test_iq_loopback, iio_uri, classname, channel, param_set):
     test_iq_loopback(iio_uri, classname, channel, param_set)
-
-
-#########################################
-@pytest.mark.iio_hardware(hardware)
-@pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0])
-def test_pluto_loopback_zeros(test_dma_dac_zeros, iio_uri, classname, channel):
-    test_dma_dac_zeros(iio_uri, classname, channel)
```

### Comparing `pyadi-iio-0.0.8/test/test_adrv9002_p.py` & `pyadi-iio-0.0.9/test/test_adrv9002_p.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import listdir
 from os.path import dirname, join, realpath
 
 import pytest
 
-hardware = "adrv9002"
+hardware = ["adrv9002-rx1tx1", "adrv9002-rx2tx2"]
 classname = "adi.adrv9002"
 profile_path = dirname(realpath(__file__)) + "/adrv9002_profiles/"
 nco_test_profile = profile_path + "lte_10_lvds_nco_api_48_8_7.json"
 nco_test_stream = profile_path + "lte_10_lvds_nco_api_48_8_7.stream"
 lte_20_lvds_profile = profile_path + "lte_20_lvds_api_48_8_7.json"
 lte_20_lvds_stream = profile_path + "lte_20_lvds_api_48_8_7.stream"
 lte_40_lvds_profile = profile_path + "lte_40_lvds_api_48_8_7.json"
@@ -228,14 +228,15 @@
 ):
     test_attribute_multipe_values_with_depends(
         iio_uri, classname, attr, depends, val, 0
     )
 
 
 #########################################
+@pytest.mark.lvds_test
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize("attr", ["profile"])
 @pytest.mark.parametrize(
     "profile_file, depends",
     [
         (lte_40_lvds_profile, {"write_stream": lte_40_lvds_stream}),
@@ -252,14 +253,15 @@
 ):
     test_attribute_write_only_str_with_depends(
         iio_uri, classname, attr, profile_file, depends
     )
 
 
 #########################################
+@pytest.mark.lvds_test
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize("attr", ["profile"])
 @pytest.mark.parametrize(
     "profile_file, depends", [(nco_test_profile, {"write_stream": nco_test_stream})]
 )
 def test_adrv9002_nco_write_profile(
@@ -272,14 +274,15 @@
 ):
     test_attribute_write_only_str_with_depends(
         iio_uri, classname, attr, profile_file, depends
     )
 
 
 #########################################
+@pytest.mark.cmos_test
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize("attr", ["profile"])
 @pytest.mark.parametrize(
     "profile_file, depends", [(lte_5_cmos_profile, {"write_stream": lte_5_cmos_stream})]
 )
 def test_adrv9002_stream_profile_write(
@@ -292,25 +295,27 @@
 ):
     test_attribute_write_only_str_with_depends(
         iio_uri, classname, attr, profile_file, depends
     )
 
 
 #########################################
+@pytest.mark.cmos_test
 @pytest.mark.iio_hardware(hardware)
 def test_adrv9002_stream_profile_write_both(iio_uri):
     import adi
 
     sdr = adi.adrv9002(iio_uri)
     sdr.write_stream_profile(lte_5_cmos_stream, lte_5_cmos_profile)
 
 
 #########################################
 # It depends on test_adrv9002_nco_write_profile to be run first.
 # Maybe we should think in adding something like pytest-dependency
+@pytest.mark.lvds_test
 @pytest.mark.iio_hardware(hardware)
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize(
     "attr, start, stop, step, tol",
     [
         ("rx0_nco_frequency", -20000, 20000, 1, 0),
         ("rx1_nco_frequency", -20000, 20000, 1, 0),
@@ -321,34 +326,51 @@
 def test_adrv9002_nco(
     test_attribute_single_value, iio_uri, classname, attr, start, stop, step, tol
 ):
     test_attribute_single_value(iio_uri, classname, attr, start, stop, step, tol)
 
 
 #########################################
-@pytest.mark.iio_hardware(hardware)
+@pytest.mark.iio_hardware(hardware[0])
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0, 1])
-def test_adrv9002_tx_data(test_dma_tx, iio_uri, classname, channel):
+@pytest.mark.parametrize("channel", [0])
+def test_adrv9002_tx_data_rx1tx1(test_dma_tx, iio_uri, classname, channel):
     test_dma_tx(iio_uri, classname, channel)
 
 
 #########################################
-@pytest.mark.iio_hardware(hardware)
+@pytest.mark.iio_hardware(hardware[1])
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize("channel", [0, 1])
-def test_adrv9002_rx_data(test_dma_rx, iio_uri, classname, channel):
+@pytest.mark.parametrize("use_tx2", [True])
+def test_adrv9002_tx_data_rx2tx2(test_dma_tx, iio_uri, classname, channel, use_tx2):
+    test_dma_tx(iio_uri, classname, channel, use_tx2)
+
+
+#########################################
+@pytest.mark.iio_hardware(hardware[0])
+@pytest.mark.parametrize("classname", [(classname)])
+@pytest.mark.parametrize("channel", [0])
+def test_adrv9002_rx_data_rx1tx1(test_dma_rx, iio_uri, classname, channel):
     test_dma_rx(iio_uri, classname, channel)
 
 
 #########################################
-@pytest.mark.iio_hardware(hardware)
-@pytest.mark.skip(reason="Test still fails on chan1")
+@pytest.mark.iio_hardware(hardware[1])
 @pytest.mark.parametrize("classname", [(classname)])
 @pytest.mark.parametrize("channel", [0, 1])
+@pytest.mark.parametrize("use_rx2", [True])
+def test_adrv9002_rx_data_rx2tx2(test_dma_rx, iio_uri, classname, channel, use_rx2):
+    test_dma_rx(iio_uri, classname, channel, use_rx2)
+
+
+########################################
+@pytest.mark.iio_hardware(hardware[0])
+@pytest.mark.parametrize("classname", [(classname)])
+@pytest.mark.parametrize("channel", [0])
 @pytest.mark.parametrize(
     "param_set",
     [
         dict(
             tx0_lo=1000000000,
             rx0_lo=1000000000,
             tx1_lo=1000000000,
@@ -363,17 +385,17 @@
     ],
 )
 def test_adrv9002_cw_loopback(test_cw_loopback, iio_uri, classname, channel, param_set):
     test_cw_loopback(iio_uri, classname, channel, param_set)
 
 
 #########################################
-@pytest.mark.iio_hardware(hardware)
+@pytest.mark.iio_hardware(hardware[1])
 @pytest.mark.parametrize("classname", [(classname)])
-@pytest.mark.parametrize("channel", [0])
+@pytest.mark.parametrize("channel", [0, 1])
 @pytest.mark.parametrize(
     "param_set",
     [
         dict(
             tx0_lo=1000000000,
             rx0_lo=1000000000,
             tx1_lo=1000000000,
```

### Comparing `pyadi-iio-0.0.8/test/test_adis16507_p.py` & `pyadi-iio-0.0.9/test/test_adis16507_p.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_sshfs.py` & `pyadi-iio-0.0.9/test/test_sshfs.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_adrv9009_zu11eg.py` & `pyadi-iio-0.0.9/test/test_adrv9009_zu11eg.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_daq3_p.py` & `pyadi-iio-0.0.9/test/test_daq3_p.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_map.py` & `pyadi-iio-0.0.9/test/test_map.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from os import sendfile
+
+
 def get_test_map():
     # Keys are substrings of test function names (and usually filenames)
     # Any board-fmc name will run a specific tests with key as name
 
     # NO TESTS YET
     # zynq-zc702-adv7511
     # zynq-zc706-adv7511-fmcadc4
@@ -66,9 +69,17 @@
         "zynq-zc706-adv7511-ad9364-fmcomms4",
         "zynqmp-zcu102-rev10-ad9364-fmcomms4",
         "zynq-adrv9364-z7020-box",
         "zynq-adrv9364-z7020-bob",
         "zynq-adrv9364-z7020-bob-cmos",
         "zynq-zed-adv7511-ad9364-fmcomms4",
     ]
+    test_map["adrv9002"] = [
+        "zynq-zc706-adv7511-adrv9002",
+        "zynq-zc706-adv7511-adrv9002-rx2tx2",
+        "zynq-zed-adv7511-adrv9002",
+        "zynq-zed-adv7511-adrv9002-rx2tx2",
+        "zynqmp-zcu102-rev10-adrv9002",
+        "zynqmp-zcu102-rev10-adrv9002-rx2tx2",
+    ]
 
     return test_map
```

### Comparing `pyadi-iio-0.0.8/test/test_adis16460_p.py` & `pyadi-iio-0.0.9/test/test_adis16460_p.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_ad9371.py` & `pyadi-iio-0.0.9/test/test_ad9371.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/test/test_ad9081.py` & `pyadi-iio-0.0.9/test/test_ad9081.py`

 * *Files identical despite different names*

### Comparing `pyadi-iio-0.0.8/pyadi_iio.egg-info/SOURCES.txt` & `pyadi-iio-0.0.9/pyadi_iio.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 adi/ad7124.py
 adi/ad7606.py
 adi/ad7689.py
 adi/ad7746.py
 adi/ad7799.py
 adi/ad9081.py
 adi/ad9081_mc.py
+adi/ad9083.py
 adi/ad9094.py
 adi/ad9136.py
 adi/ad9144.py
 adi/ad9152.py
 adi/ad936x.py
 adi/ad9371.py
 adi/ad9680.py
 adi/adar1000.py
+adi/adf4371.py
 adi/adis16460.py
+adi/adis16495.py
 adi/adis16507.py
+adi/adpd188.py
 adi/adpd410x.py
 adi/adrv9002.py
 adi/adrv9009.py
 adi/adrv9009_zu11eg.py
 adi/adrv9009_zu11eg_fmcomms8.py
 adi/adrv9009_zu11eg_multi.py
 adi/adxl345.py
@@ -50,30 +54,33 @@
 pyadi_iio.egg-info/dependency_links.txt
 pyadi_iio.egg-info/requires.txt
 pyadi_iio.egg-info/top_level.txt
 test/test_ad7606.py
 test/test_ad7689.py
 test/test_ad7799.py
 test/test_ad9081.py
+test/test_ad9083_p.py
 test/test_ad9136_p.py
 test/test_ad9144_p.py
 test/test_ad9152_p.py
 test/test_ad9361_p.py
 test/test_ad9364_p.py
 test/test_ad9371.py
 test/test_ad9680_p.py
 test/test_adis16460_p.py
+test/test_adis16495_p.py
 test/test_adis16507_p.py
 test/test_adpd410x.py
 test/test_adrv9002_generic_p.py
 test/test_adrv9002_p.py
 test/test_adrv9009_p.py
 test/test_adrv9009_zu11eg.py
 test/test_adrv9009_zu11eg_fmcomms8.py
 test/test_daq2_p.py
 test/test_daq3_p.py
+test/test_fmcomms2-3_p.py
 test/test_fmcomms5_p.py
 test/test_generic.py
 test/test_map.py
 test/test_pluto_p.py
 test/test_sshfs.py
 test/test_stress.py
```

### Comparing `pyadi-iio-0.0.8/pyadi_iio.egg-info/PKG-INFO` & `pyadi-iio-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyadi-iio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Interfaces to stream data from ADI hardware
 Home-page: https://github.com/analogdevicesinc/pyadi-iio
 Author: Travis Collins
 Author-email: travis.collins@analog.com
 License: UNKNOWN
 Description: <!-- PYADI-IIO README -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyadi-iio Version: 0.0.8 Summary: Interfaces to
+Metadata-Version: 2.1 Name: pyadi-iio Version: 0.0.9 Summary: Interfaces to
 stream data from ADI hardware Home-page: https://github.com/analogdevicesinc/
 pyadi-iio Author: Travis Collins Author-email: travis.collins@analog.com
 License: UNKNOWN Description:
                                [PyADI-IIO Logo]
          [Build_Status] [PyPI_version] [Codacy_Badge] [Python_Version]
                   [GitHub_Pages] [EngineerZone] [Analog_Wiki]
 --- ### pyadi-iio: Analog Devices python interfaces for hardware with
```

