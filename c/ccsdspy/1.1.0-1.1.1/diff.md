# Comparing `tmp/ccsdspy-1.1.0-r1.tar.gz` & `tmp/ccsdspy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccsdspy-1.1.0.tar", last modified: Tue Apr 11 15:21:25 2023, max compression
+gzip compressed data, was "ccsdspy-1.1.1.tar", last modified: Thu Apr 13 23:44:24 2023, max compression
```

## Comparing `ccsdspy-1.1.0-r1.tar` & `ccsdspy-1.1.1.tar`

### file list

```diff
@@ -1,182 +1,184 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.975703 ccsdspy-1.1.0/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.260404 ccsdspy-1.1.0/.github/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.500154 ccsdspy-1.1.0/.github/workflows/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1077 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/.github/workflows/ccsdspy-ci.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)      803 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/.github/workflows/doc-build.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1237 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/.gitignore
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2618 2023-04-11 15:19:43.000000 ccsdspy-1.1.0/CHANGELOG.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1490 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/LICENSE.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5085 2023-04-11 15:21:25.977696 ccsdspy-1.1.0/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2546 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.563958 ccsdspy-1.1.0/ccsdspy/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      526 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1703 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/__main__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      160 2023-04-11 15:21:23.000000 ccsdspy-1.1.0/ccsdspy/_version.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      166 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/constants.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     9270 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/converters.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    19073 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/decode.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6540 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/packet_fields.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    24216 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/packet_types.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.686702 ccsdspy-1.1.0/ccsdspy/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/__init__.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.385320 ccsdspy-1.1.0/ccsdspy/tests/data/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.692881 ccsdspy-1.1.0/ccsdspy/tests/data/hs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      232 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.717083 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    73848 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      727 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.738606 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   179163 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1524 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.754085 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   367200 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1159 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.784064 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid130/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   559689 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      390 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid130/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.813451 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid251/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  1008000 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      422 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid251/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.858480 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid895/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  2446980 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      440 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid895/defs.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.868169 ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    17668 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2116 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.901722 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      111 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/simple_csv_3col.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/simple_csv_3col_with_array.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/simple_csv_4col.csv
--rw-r--r--   0 daniel    (1000) daniel    (1000)      149 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/packet_def/simple_csv_4col_with_array.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.984158 ccsdspy-1.1.0/ccsdspy/tests/data/split/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14820 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1040 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00384.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      416 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00386.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1680 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00391.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)      672 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00392.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5600 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00393.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2964 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00394.tlm
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2448 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/apid01313.tlm
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.611159 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1443 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Conventions.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2025 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2024 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2028 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2334 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3181 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2954 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3169 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3264 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3193 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11574 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4383 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4673 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11049 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4339 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11742 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3521 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5569 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3874 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3373 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8213 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11728 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9803 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6597 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9974 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3052 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2812 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4689 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3067 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3875 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1672 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2233 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    13104 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8921 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14772 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ADCS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10135 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   150107 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_BOOT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4122 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DDMI.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1935 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1662 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    42952 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9093 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1562 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_FILL.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    12767 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_HI.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    28801 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_LOW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    31990 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_LZ.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    17290 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_PASS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3652 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_PVT.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8744 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_SSV.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)       45 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/LIMITS.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9201 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Overview.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    24277 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Revision History.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6540 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4905 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5124 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6725 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6856 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_FULL.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5878 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_META.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6120 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_META_V2.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2016 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_RAW.csv
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1384 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SUPER_NOM.csv
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.660620 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      634 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/README.md
--rw-r--r--   0 daniel    (1000) daniel    (1000)      318 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets.bin
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1213 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2015 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      590 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin
--rw-r--r--   0 daniel    (1000) daniel    (1000)      338 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets_with_footer.bin
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11320 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/tests/test_converters.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4837 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_hs.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3103 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_packet_fields.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7600 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_packet_types.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8837 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/tests/test_primary_header.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4480 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_split.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4756 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_utils.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4182 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/ccsdspy/tests/test_var_length.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7887 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/ccsdspy/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:24.600102 ccsdspy-1.1.0/ccsdspy.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5085 2023-04-11 15:21:23.000000 ccsdspy-1.1.0/ccsdspy.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6402 2023-04-11 15:21:24.000000 ccsdspy-1.1.0/ccsdspy.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-11 15:21:23.000000 ccsdspy-1.1.0/ccsdspy.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      194 2023-04-11 15:21:23.000000 ccsdspy-1.1.0/ccsdspy.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-04-11 15:21:23.000000 ccsdspy-1.1.0/ccsdspy.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.714146 ccsdspy-1.1.0/docs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8399 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/Makefile
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.720351 ccsdspy-1.1.0/docs/_static/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    36033 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/logo.png
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.791345 ccsdspy-1.1.0/docs/_static/used-by/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)  1343999 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/goes-r.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    74095 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/hermes.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   240058 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/mms.jpg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)   152642 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/punch.png
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      106 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/resize.sh
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.828406 ccsdspy-1.1.0/docs/_static/used-by/small/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20111 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/small/goes-r.png
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14174 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/small/hermes.png
--rw-r--r--   0 daniel    (1000) daniel    (1000)    41871 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/small/mms.jpg
--rw-r--r--   0 daniel    (1000) daniel    (1000)    13675 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_static/used-by/small/punch.png
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.842482 ccsdspy-1.1.0/docs/_templates/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      463 2023-03-18 01:24:52.000000 ccsdspy-1.1.0/docs/_templates/github.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)       80 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/_templates/logo.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      134 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/api.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7670 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/conf.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.855471 ccsdspy-1.1.0/docs/dev-guide/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7281 2023-03-18 01:25:20.000000 ccsdspy-1.1.0/docs/dev-guide/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2830 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7768 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/make.bat
--rw-r--r--   0 daniel    (1000) daniel    (1000)       34 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.949122 ccsdspy-1.1.0/docs/user-guide/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3411 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/ccsds.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3995 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/user-guide/converters.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3253 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/fixedlength.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)      243 2023-04-11 15:15:13.000000 ccsdspy-1.1.0/docs/user-guide/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1853 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/packetfields.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4672 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/utils.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3777 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/user-guide/variablelength.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-11 15:21:25.962087 ccsdspy-1.1.0/docs/whatsnew/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       95 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/whatsnew/changelog.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)      110 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/docs/whatsnew/index.rst
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2716 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)      542 2023-03-18 01:23:55.000000 ccsdspy-1.1.0/readthedocs.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)      162 2023-04-11 15:21:25.982073 ccsdspy-1.1.0/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.741839 ccsdspy-1.1.1/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.394235 ccsdspy-1.1.1/.github/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.420456 ccsdspy-1.1.1/.github/workflows/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1077 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/.github/workflows/ccsdspy-ci.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      803 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/.github/workflows/doc-build.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1237 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/.gitignore
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2618 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/CHANGELOG.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1490 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/LICENSE.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5085 2023-04-13 23:44:24.742868 ccsdspy-1.1.1/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2546 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.435691 ccsdspy-1.1.1/ccsdspy/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      526 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1703 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/__main__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      160 2023-04-13 23:44:24.000000 ccsdspy-1.1.1/ccsdspy/_version.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      166 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/constants.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     9270 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/converters.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    19073 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/decode.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6540 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/packet_fields.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    24216 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/packet_types.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.461055 ccsdspy-1.1.1/ccsdspy/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/__init__.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.403513 ccsdspy-1.1.1/ccsdspy/tests/data/
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.462349 ccsdspy-1.1.1/ccsdspy/tests/data/hs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      232 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.466472 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid001/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    73848 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      727 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid001/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.471624 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid010/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   179163 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1524 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid010/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.476584 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid035/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   367200 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1159 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid035/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.482466 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid130/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   559689 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      390 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid130/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.490437 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid251/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  1008000 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      422 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid251/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.501402 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid895/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2446980 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      440 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid895/defs.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.505435 ccsdspy-1.1.1/ccsdspy/tests/data/hs/attic/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    17668 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2116 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.512719 ccsdspy-1.1.1/ccsdspy/tests/data/packet_def/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      111 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/packet_def/simple_csv_3col.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/packet_def/simple_csv_3col_with_array.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/packet_def/simple_csv_4col.csv
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      149 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/packet_def/simple_csv_4col_with_array.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.529689 ccsdspy-1.1.1/ccsdspy/tests/data/split/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14820 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1040 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00384.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      416 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00386.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1680 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00391.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      672 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00392.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5600 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00393.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2964 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00394.tlm
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2448 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/apid01313.tlm
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.665087 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1443 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/Conventions.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2025 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2024 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2028 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2334 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3181 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2954 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3169 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3264 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3193 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11574 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4383 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4673 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11049 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4339 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11742 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3521 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5569 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3874 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3373 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8213 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    11728 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9803 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6597 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9974 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3052 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2812 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4689 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3067 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3875 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1672 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2233 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    13104 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8921 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14772 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_ADCS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10135 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   150107 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_BOOT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4122 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_DDMI.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1935 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_DNLD.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1662 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    42952 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9093 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1562 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_FILL.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    12767 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_HI.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    28801 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_LOW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    31990 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_LZ.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    17290 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_PASS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3652 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_PVT.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8744 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_SSV.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)       45 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/LIMITS.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     9201 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/Overview.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    24277 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/Revision History.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6540 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4905 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5124 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6725 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6856 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_FULL.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     5878 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_META.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6120 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_META_V2.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2016 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_RAW.csv
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1384 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SUPER_NOM.csv
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.675916 ccsdspy-1.1.1/ccsdspy/tests/data/var_length/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      634 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/var_length/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      318 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/var_length/var_length_packets.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1213 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/var_length/var_length_packets.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2015 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      590 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      338 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/data/var_length/var_length_packets_with_footer.bin
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11320 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/test_converters.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4837 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/test_hs.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3103 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/test_packet_fields.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7600 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/test_packet_types.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8837 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/test_primary_header.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4480 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/test_split.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4756 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/test_utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4182 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/tests/test_var_length.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7887 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/ccsdspy/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.443684 ccsdspy-1.1.1/ccsdspy.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5085 2023-04-13 23:44:24.000000 ccsdspy-1.1.1/ccsdspy.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6470 2023-04-13 23:44:24.000000 ccsdspy-1.1.1/ccsdspy.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-13 23:44:24.000000 ccsdspy-1.1.1/ccsdspy.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      194 2023-04-13 23:44:24.000000 ccsdspy-1.1.1/ccsdspy.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-04-13 23:44:24.000000 ccsdspy-1.1.1/ccsdspy.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.687203 ccsdspy-1.1.1/docs/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8399 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/Makefile
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.688223 ccsdspy-1.1.1/docs/_static/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    36033 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/_static/logo.png
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.708307 ccsdspy-1.1.1/docs/_static/used-by/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   281290 2023-04-11 18:15:35.000000 ccsdspy-1.1.1/docs/_static/used-by/elfin.jpg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)  1343999 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/_static/used-by/goes-r.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    74095 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/_static/used-by/hermes.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   240058 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/_static/used-by/mms.jpg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)   152642 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/_static/used-by/punch.png
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      106 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/_static/used-by/resize.sh
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.720004 ccsdspy-1.1.1/docs/_static/used-by/small/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    16916 2023-04-11 18:15:37.000000 ccsdspy-1.1.1/docs/_static/used-by/small/elfin.jpg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    20111 2023-04-11 18:15:56.000000 ccsdspy-1.1.1/docs/_static/used-by/small/goes-r.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    14174 2023-04-11 18:16:06.000000 ccsdspy-1.1.1/docs/_static/used-by/small/hermes.png
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    41871 2023-04-11 18:15:37.000000 ccsdspy-1.1.1/docs/_static/used-by/small/mms.jpg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    13675 2023-04-11 18:15:56.000000 ccsdspy-1.1.1/docs/_static/used-by/small/punch.png
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.723986 ccsdspy-1.1.1/docs/_templates/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      463 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/_templates/github.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       80 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/_templates/logo.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      134 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/api.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7670 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/conf.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.725071 ccsdspy-1.1.1/docs/dev-guide/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7281 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/dev-guide/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2915 2023-04-11 18:16:13.000000 ccsdspy-1.1.1/docs/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7768 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/make.bat
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       34 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.738492 ccsdspy-1.1.1/docs/user-guide/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3411 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/user-guide/ccsds.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3995 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/user-guide/converters.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3253 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/user-guide/fixedlength.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      243 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/user-guide/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1853 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/user-guide/packetfields.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4672 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/user-guide/utils.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3777 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/user-guide/variablelength.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-13 23:44:24.740881 ccsdspy-1.1.1/docs/whatsnew/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       95 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/whatsnew/changelog.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      110 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/docs/whatsnew/index.rst
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2716 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      542 2023-04-11 18:14:59.000000 ccsdspy-1.1.1/readthedocs.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      162 2023-04-13 23:44:24.743799 ccsdspy-1.1.1/setup.cfg
```

### Comparing `ccsdspy-1.1.0/.github/workflows/ccsdspy-ci.yml` & `ccsdspy-1.1.1/.github/workflows/ccsdspy-ci.yml`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/.github/workflows/doc-build.yml` & `ccsdspy-1.1.1/.github/workflows/doc-build.yml`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/.gitignore` & `ccsdspy-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/CHANGELOG.rst` & `ccsdspy-1.1.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/LICENSE.rst` & `ccsdspy-1.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/PKG-INFO` & `ccsdspy-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsdspy
-Version: 1.1.0
+Version: 1.1.1
 Summary: IO Interface for Reading CCSDS Data in Python.
 Author-email: Daniel da Silva <mail@danieldasilva.org>, Steven Christe <steven.d.christe@nasa.gov>
 License: Copyright (c) 2018, Daniel da Silva
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `ccsdspy-1.1.0/README.rst` & `ccsdspy-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/__init__.py` & `ccsdspy-1.1.1/ccsdspy/__init__.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/__main__.py` & `ccsdspy-1.1.1/ccsdspy/__main__.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/converters.py` & `ccsdspy-1.1.1/ccsdspy/converters.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/decode.py` & `ccsdspy-1.1.1/ccsdspy/decode.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/packet_fields.py` & `ccsdspy-1.1.1/ccsdspy/packet_fields.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/packet_types.py` & `ccsdspy-1.1.1/ccsdspy/packet_types.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid001/SSAT1_2015-180-00-00-00_2015-180-01-59-58_1_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid001/defs.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid001/defs.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid010/SSAT1_2015-180-00-00-00_2015-180-00-59-59_10_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid010/defs.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid010/defs.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid035/SSAT1_2015-180-00-00-00_2015-180-01-59-59_35_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid035/defs.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid035/defs.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid130/SSAT1_2015-180-00-00-00_2015-180-01-59-35_130_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid251/SSAT1_2015-180-00-00-00_2015-180-01-59-59_251_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/apid895/SSAT1_2015-180-00-00-00_2015-180-01-59-56_895_1_sim.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/attic/SSAT_Mnemonics.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py` & `ccsdspy-1.1.1/ccsdspy/tests/data/hs/attic/_expand_mnemnonics.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/CYGNSS_F7_L0_2022_086_10_15_V01_F__first101pkts.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00384.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00384.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00392.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00392.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00393.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00393.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid00394.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/apid00394.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/apid01313.tlm` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/apid01313.tlm`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Conventions.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/Conventions.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_INP.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_OUT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_ADCS_BUS_FSW_TLM.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_ACK.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_AD_RESP.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_AUTOLOAD.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_ERASEFLASH.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_DUMP.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_BOOTLOADER_MEM_LOAD.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_PWR.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CHAN_TRACK_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_COMM_DIAG.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_CYGNSS_PKT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_DATA_LOGGER_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_FRONT_END_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_NAV_INFO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_OP_SETTINGS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_ORBITAL_ELEMENTS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PPS_TABLE.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PROCESSED_DATA.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_PVT_INFO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_RAW_DATA.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_CHAN_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_LIST.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_REFL_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_SPW_DDM_TH.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_STATUS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_DDMI_STREAM_ROUTER_STAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_ECHO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_MAG_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_NST_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/DIAG_RWA_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ADCS.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_ADCS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_ADCSIO.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_BOOT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_BOOT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DDMI.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_DDMI.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_DNLD.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_DNLD_FAT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_DNLD_FPT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_ERREVT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_FILL.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_FILL.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_HI.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_HI.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_LOW.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_LOW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_LZ.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_LZ.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_PASS.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_PASS.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_PVT.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_PVT.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/ENG_SSV.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/ENG_SSV.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Overview.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/Overview.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/Revision History.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/Revision History.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_DDM_BB_X8.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_DDM_X10.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_DDM_X11.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_DDM_X8.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_FULL.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_FULL.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_META.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_META.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_META_V2.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_META_V2.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SCI_RAW.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SCI_RAW.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/split/defs/SUPER_NOM.csv` & `ccsdspy-1.1.1/ccsdspy/tests/data/split/defs/SUPER_NOM.csv`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/var_length/README.md` & `ccsdspy-1.1.1/ccsdspy/tests/data/var_length/README.md`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets.py` & `ccsdspy-1.1.1/ccsdspy/tests/data/var_length/var_length_packets.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py` & `ccsdspy-1.1.1/ccsdspy/tests/data/var_length/var_length_packets_double_varfield.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin` & `ccsdspy-1.1.1/ccsdspy/tests/data/var_length/var_length_packets_double_varfield_with_footer.bin`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/test_converters.py` & `ccsdspy-1.1.1/ccsdspy/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/test_hs.py` & `ccsdspy-1.1.1/ccsdspy/tests/test_hs.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/test_packet_fields.py` & `ccsdspy-1.1.1/ccsdspy/tests/test_packet_fields.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/test_packet_types.py` & `ccsdspy-1.1.1/ccsdspy/tests/test_packet_types.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/test_primary_header.py` & `ccsdspy-1.1.1/ccsdspy/tests/test_primary_header.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/test_split.py` & `ccsdspy-1.1.1/ccsdspy/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/test_utils.py` & `ccsdspy-1.1.1/ccsdspy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/tests/test_var_length.py` & `ccsdspy-1.1.1/ccsdspy/tests/test_var_length.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy/utils.py` & `ccsdspy-1.1.1/ccsdspy/utils.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/ccsdspy.egg-info/PKG-INFO` & `ccsdspy-1.1.1/ccsdspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsdspy
-Version: 1.1.0
+Version: 1.1.1
 Summary: IO Interface for Reading CCSDS Data in Python.
 Author-email: Daniel da Silva <mail@danieldasilva.org>, Steven Christe <steven.d.christe@nasa.gov>
 License: Copyright (c) 2018, Daniel da Silva
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `ccsdspy-1.1.0/ccsdspy.egg-info/SOURCES.txt` & `ccsdspy-1.1.1/ccsdspy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -127,19 +127,21 @@
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/requirements.txt
 docs/_static/logo.png
+docs/_static/used-by/elfin.jpg
 docs/_static/used-by/goes-r.png
 docs/_static/used-by/hermes.png
 docs/_static/used-by/mms.jpg
 docs/_static/used-by/punch.png
 docs/_static/used-by/resize.sh
+docs/_static/used-by/small/elfin.jpg
 docs/_static/used-by/small/goes-r.png
 docs/_static/used-by/small/hermes.png
 docs/_static/used-by/small/mms.jpg
 docs/_static/used-by/small/punch.png
 docs/_templates/github.html
 docs/_templates/logo.html
 docs/dev-guide/index.rst
```

### Comparing `ccsdspy-1.1.0/docs/Makefile` & `ccsdspy-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/_static/logo.png` & `ccsdspy-1.1.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/_static/used-by/goes-r.png` & `ccsdspy-1.1.1/docs/_static/used-by/goes-r.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/_static/used-by/hermes.png` & `ccsdspy-1.1.1/docs/_static/used-by/hermes.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/_static/used-by/mms.jpg` & `ccsdspy-1.1.1/docs/_static/used-by/mms.jpg`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/_static/used-by/punch.png` & `ccsdspy-1.1.1/docs/_static/used-by/punch.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/_static/used-by/small/goes-r.png` & `ccsdspy-1.1.1/docs/_static/used-by/small/goes-r.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/_static/used-by/small/hermes.png` & `ccsdspy-1.1.1/docs/_static/used-by/small/hermes.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/_static/used-by/small/mms.jpg` & `ccsdspy-1.1.1/docs/_static/used-by/small/mms.jpg`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/_static/used-by/small/punch.png` & `ccsdspy-1.1.1/docs/_static/used-by/small/punch.png`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/conf.py` & `ccsdspy-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/dev-guide/index.rst` & `ccsdspy-1.1.1/docs/dev-guide/index.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/index.rst` & `ccsdspy-1.1.1/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     :target: https://www.goes-r.gov/
 .. image:: _static/used-by/small/hermes.png
     :target: https://science.nasa.gov/missions/hermes
 .. image:: _static/used-by/small/punch.png
     :target: https://punch.space.swri.edu/
 .. image:: _static/used-by/small/mms.jpg
     :target: https://mms.gsfc.nasa.gov/
+.. image:: _static/used-by/small/elfin.jpg
+    :target: https://elfin.igpp.ucla.edu/
 
 Do you know of other missions that use CCSDSPy? Let us know `through a github issue`_!
 
 .. _through a github issue: https://github.com/ccsdspy/ccsdspy/issues/new
 
 Install ccsdspy
 ---------------
```

### Comparing `ccsdspy-1.1.0/docs/make.bat` & `ccsdspy-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/user-guide/ccsds.rst` & `ccsdspy-1.1.1/docs/user-guide/ccsds.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/user-guide/converters.rst` & `ccsdspy-1.1.1/docs/user-guide/converters.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/user-guide/fixedlength.rst` & `ccsdspy-1.1.1/docs/user-guide/fixedlength.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/user-guide/packetfields.rst` & `ccsdspy-1.1.1/docs/user-guide/packetfields.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/user-guide/utils.rst` & `ccsdspy-1.1.1/docs/user-guide/utils.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/docs/user-guide/variablelength.rst` & `ccsdspy-1.1.1/docs/user-guide/variablelength.rst`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/pyproject.toml` & `ccsdspy-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ccsdspy-1.1.0/readthedocs.yml` & `ccsdspy-1.1.1/readthedocs.yml`

 * *Files identical despite different names*

