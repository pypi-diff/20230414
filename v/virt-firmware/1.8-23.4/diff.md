# Comparing `tmp/virt-firmware-1.8.tar.gz` & `tmp/virt-firmware-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virt-firmware-1.8.tar", last modified: Mon Jan 16 16:03:38 2023, max compression
+gzip compressed data, was "virt-firmware-23.4.tar", last modified: Fri Apr 14 07:50:34 2023, max compression
```

## Comparing `virt-firmware-1.8.tar` & `virt-firmware-23.4.tar`

### file list

```diff
@@ -1,63 +1,73 @@
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.897994 virt-firmware-1.8/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    18012 2022-04-20 16:46:39.000000 virt-firmware-1.8/LICENSE
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       87 2023-01-12 08:31:18.000000 virt-firmware-1.8/MANIFEST.in
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2531 2023-01-16 16:03:38.897994 virt-firmware-1.8/PKG-INFO
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2199 2022-07-18 11:50:43.000000 virt-firmware-1.8/README.md
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       81 2022-03-30 09:41:51.000000 virt-firmware-1.8/pyproject.toml
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1026 2023-01-16 16:03:38.897994 virt-firmware-1.8/setup.cfg
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       69 2022-03-30 09:41:51.000000 virt-firmware-1.8/setup.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.887994 virt-firmware-1.8/tests/
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.887994 virt-firmware-1.8/tests/data/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3737 2022-11-24 12:28:42.000000 virt-firmware-1.8/tests/data/DBXUpdate-20100307.x64.bin
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1772 2022-05-11 20:36:49.000000 virt-firmware-1.8/tests/data/secboot.aws
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      345 2022-12-02 08:59:55.000000 virt-firmware-1.8/tests/test-dump.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      183 2022-09-02 08:20:10.000000 virt-firmware-1.8/tests/test-pe.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      185 2022-09-02 08:19:03.000000 virt-firmware-1.8/tests/test-sigdb.sh
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      689 2022-09-02 08:10:06.000000 virt-firmware-1.8/tests/test-vars.sh
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     3687 2022-12-07 13:29:04.000000 virt-firmware-1.8/tests/tests.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.884994 virt-firmware-1.8/virt/
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.889994 virt-firmware-1.8/virt/firmware/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      130 2022-11-10 08:06:38.000000 virt-firmware-1.8/virt/firmware/__init__.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.890994 virt-firmware-1.8/virt/firmware/aws/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    11381 2022-05-11 20:36:49.000000 virt-firmware-1.8/virt/firmware/aws/dict.v0
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.892994 virt-firmware-1.8/virt/firmware/certs/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4323 2022-07-07 16:26:41.000000 virt-firmware-1.8/virt/firmware/certs/CentOSSecureBootCA2.pem
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4339 2022-07-07 16:26:41.000000 virt-firmware-1.8/virt/firmware/certs/CentOSSecureBootCAkey1.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6739 2022-03-30 10:39:05.000000 virt-firmware-1.8/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6869 2022-03-30 10:39:05.000000 virt-firmware-1.8/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6698 2022-03-30 10:39:05.000000 virt-firmware-1.8/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4615 2022-07-07 08:32:28.000000 virt-firmware-1.8/virt/firmware/certs/RedHatSecureBootCA3.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4431 2022-07-07 08:32:38.000000 virt-firmware-1.8/virt/firmware/certs/RedHatSecureBootCA5.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4324 2022-07-07 08:32:47.000000 virt-firmware-1.8/virt/firmware/certs/RedHatSecureBootCA6.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4500 2022-03-30 10:39:05.000000 virt-firmware-1.8/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5007 2022-07-16 16:13:52.000000 virt-firmware-1.8/virt/firmware/certs/fedoraca-20200709.pem
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    21024 2023-01-11 05:55:56.000000 virt-firmware-1.8/virt/firmware/dump.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.894994 virt-firmware-1.8/virt/firmware/efi/
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      110 2022-03-30 11:58:43.000000 virt-firmware-1.8/virt/firmware/efi/__init__.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2774 2022-12-07 13:30:17.000000 virt-firmware-1.8/virt/firmware/efi/certs.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4916 2022-07-15 15:06:27.000000 virt-firmware-1.8/virt/firmware/efi/devpath.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1663 2022-12-14 07:11:30.000000 virt-firmware-1.8/virt/firmware/efi/efijson.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    17855 2022-12-14 17:02:10.000000 virt-firmware-1.8/virt/firmware/efi/efivar.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5173 2022-12-02 08:15:31.000000 virt-firmware-1.8/virt/firmware/efi/guids.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6053 2022-11-30 08:12:07.000000 virt-firmware-1.8/virt/firmware/efi/siglist.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1379 2022-03-30 10:39:05.000000 virt-firmware-1.8/virt/firmware/efi/ucs16.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1434 2023-01-11 05:55:56.000000 virt-firmware-1.8/virt/firmware/host.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1689 2023-01-11 05:55:56.000000 virt-firmware-1.8/virt/firmware/migrate.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      494 2022-05-11 20:36:49.000000 virt-firmware-1.8/virt/firmware/misc.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1588 2023-01-11 05:55:56.000000 virt-firmware-1.8/virt/firmware/sigdb.py
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)    13036 2023-01-11 05:55:56.000000 virt-firmware-1.8/virt/firmware/vars.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.895994 virt-firmware-1.8/virt/firmware/varstore/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       66 2023-01-11 05:55:50.000000 virt-firmware-1.8/virt/firmware/varstore/__init__.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5423 2022-11-24 13:01:24.000000 virt-firmware-1.8/virt/firmware/varstore/aws.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4837 2022-11-24 13:00:27.000000 virt-firmware-1.8/virt/firmware/varstore/edk2.py
--rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1400 2022-03-30 10:39:05.000000 virt-firmware-1.8/virt/firmware/varstore/linux.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.896994 virt-firmware-1.8/virt/peutils/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       60 2022-12-14 09:40:14.000000 virt-firmware-1.8/virt/peutils/__init__.py
--rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)     6820 2023-01-11 05:55:56.000000 virt-firmware-1.8/virt/peutils/peutils.py
-drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-01-16 16:03:38.896994 virt-firmware-1.8/virt_firmware.egg-info/
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2531 2023-01-16 16:03:38.000000 virt-firmware-1.8/virt_firmware.egg-info/PKG-INFO
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1511 2023-01-16 16:03:38.000000 virt-firmware-1.8/virt_firmware.egg-info/SOURCES.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)        1 2023-01-16 16:03:38.000000 virt-firmware-1.8/virt_firmware.egg-info/dependency_links.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)      358 2023-01-16 16:03:38.000000 virt-firmware-1.8/virt_firmware.egg-info/entry_points.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       31 2023-01-16 16:03:38.000000 virt-firmware-1.8/virt_firmware.egg-info/requires.txt
--rw-r--r--   0 kraxel    (1000) kraxel    (1000)       68 2023-01-16 16:03:38.000000 virt-firmware-1.8/virt_firmware.egg-info/top_level.txt
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.054046 virt-firmware-23.4/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    18012 2022-04-20 16:46:39.000000 virt-firmware-23.4/LICENSE
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      116 2023-01-26 11:26:15.000000 virt-firmware-23.4/MANIFEST.in
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-04-14 07:50:34.054046 virt-firmware-23.4/PKG-INFO
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2199 2022-07-18 11:50:43.000000 virt-firmware-23.4/README.md
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.048045 virt-firmware-23.4/experimental/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1820 2023-01-11 05:55:56.000000 virt-firmware-23.4/experimental/dbxupdate.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     8627 2023-03-03 09:52:27.000000 virt-firmware-23.4/experimental/measure.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.048045 virt-firmware-23.4/man/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      939 2023-04-14 07:21:17.000000 virt-firmware-23.4/man/virt-fw-dump.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      223 2022-10-05 11:46:37.000000 virt-firmware-23.4/man/virt-fw-dump.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      734 2023-04-14 07:21:18.000000 virt-firmware-23.4/man/virt-fw-sigdb.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       45 2022-10-05 11:46:32.000000 virt-firmware-23.4/man/virt-fw-sigdb.inc
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4317 2023-04-14 07:21:18.000000 virt-firmware-23.4/man/virt-fw-vars.1
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      515 2022-10-05 11:55:41.000000 virt-firmware-23.4/man/virt-fw-vars.inc
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       81 2022-03-30 09:41:51.000000 virt-firmware-23.4/pyproject.toml
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1027 2023-04-14 07:50:34.055045 virt-firmware-23.4/setup.cfg
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)       69 2022-03-30 09:41:51.000000 virt-firmware-23.4/setup.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.049045 virt-firmware-23.4/tests/
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.049045 virt-firmware-23.4/tests/data/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     3737 2022-11-24 12:28:42.000000 virt-firmware-23.4/tests/data/DBXUpdate-20100307.x64.bin
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1772 2022-05-11 20:36:49.000000 virt-firmware-23.4/tests/data/secboot.aws
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      345 2022-12-02 08:59:55.000000 virt-firmware-23.4/tests/test-dump.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      271 2023-04-14 07:25:30.000000 virt-firmware-23.4/tests/test-pe.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      185 2022-09-02 08:19:03.000000 virt-firmware-23.4/tests/test-sigdb.sh
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)      689 2022-09-02 08:10:06.000000 virt-firmware-23.4/tests/test-vars.sh
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     3687 2022-12-07 13:29:04.000000 virt-firmware-23.4/tests/tests.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.046046 virt-firmware-23.4/virt/
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.050046 virt-firmware-23.4/virt/firmware/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      130 2022-11-10 08:06:38.000000 virt-firmware-23.4/virt/firmware/__init__.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.050046 virt-firmware-23.4/virt/firmware/aws/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    11381 2022-05-11 20:36:49.000000 virt-firmware-23.4/virt/firmware/aws/dict.v0
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.052045 virt-firmware-23.4/virt/firmware/certs/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4323 2022-07-07 16:26:41.000000 virt-firmware-23.4/virt/firmware/certs/CentOSSecureBootCA2.pem
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     4339 2022-07-07 16:26:41.000000 virt-firmware-23.4/virt/firmware/certs/CentOSSecureBootCAkey1.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6739 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6869 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6698 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4615 2022-07-07 08:32:28.000000 virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA3.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4431 2022-07-07 08:32:38.000000 virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA5.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4324 2022-07-07 08:32:47.000000 virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA6.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     4500 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5007 2022-07-16 16:13:52.000000 virt-firmware-23.4/virt/firmware/certs/fedoraca-20200709.pem
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)    21024 2023-01-11 05:55:56.000000 virt-firmware-23.4/virt/firmware/dump.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.053045 virt-firmware-23.4/virt/firmware/efi/
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      110 2022-03-30 11:58:43.000000 virt-firmware-23.4/virt/firmware/efi/__init__.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     2774 2022-12-07 13:30:17.000000 virt-firmware-23.4/virt/firmware/efi/certs.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5109 2023-03-24 08:04:11.000000 virt-firmware-23.4/virt/firmware/efi/devpath.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1663 2022-12-14 07:11:30.000000 virt-firmware-23.4/virt/firmware/efi/efijson.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)    17855 2023-03-27 15:52:53.000000 virt-firmware-23.4/virt/firmware/efi/efivar.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5173 2022-12-02 08:15:31.000000 virt-firmware-23.4/virt/firmware/efi/guids.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     6167 2023-04-13 11:19:16.000000 virt-firmware-23.4/virt/firmware/efi/siglist.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1379 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/efi/ucs16.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1434 2023-01-11 05:55:56.000000 virt-firmware-23.4/virt/firmware/host.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1689 2023-01-11 05:55:56.000000 virt-firmware-23.4/virt/firmware/migrate.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)      494 2022-05-11 20:36:49.000000 virt-firmware-23.4/virt/firmware/misc.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1588 2023-01-11 05:55:56.000000 virt-firmware-23.4/virt/firmware/sigdb.py
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)    13202 2023-04-13 10:13:39.000000 virt-firmware-23.4/virt/firmware/vars.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.053045 virt-firmware-23.4/virt/firmware/varstore/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       66 2023-03-03 10:32:41.000000 virt-firmware-23.4/virt/firmware/varstore/__init__.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     5423 2022-11-24 13:01:24.000000 virt-firmware-23.4/virt/firmware/varstore/aws.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     6271 2023-04-13 10:23:09.000000 virt-firmware-23.4/virt/firmware/varstore/edk2.py
+-rw-rw-r--   0 kraxel    (1000) kraxel    (1000)     1400 2022-03-30 10:39:05.000000 virt-firmware-23.4/virt/firmware/varstore/linux.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.053045 virt-firmware-23.4/virt/peutils/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       60 2022-12-14 09:40:14.000000 virt-firmware-23.4/virt/peutils/__init__.py
+-rwxr-xr-x   0 kraxel    (1000) kraxel    (1000)     8733 2023-04-13 11:51:41.000000 virt-firmware-23.4/virt/peutils/peutils.py
+drwxr-xr-x   0 kraxel    (1000) kraxel    (1000)        0 2023-04-14 07:50:34.054046 virt-firmware-23.4/virt_firmware.egg-info/
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     2532 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/PKG-INFO
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)     1683 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/SOURCES.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)        1 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/dependency_links.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)      358 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/entry_points.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       31 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/requires.txt
+-rw-r--r--   0 kraxel    (1000) kraxel    (1000)       68 2023-04-14 07:50:34.000000 virt-firmware-23.4/virt_firmware.egg-info/top_level.txt
```

### Comparing `virt-firmware-1.8/LICENSE` & `virt-firmware-23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/PKG-INFO` & `virt-firmware-23.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virt-firmware
-Version: 1.8
+Version: 23.4
 Summary: tools for virtual machine firmware volumes
 Author: Gerd Hoffmann
 Author-email: kraxel@redhat.com
 License: GPLv2
 Project-URL: GitLab, https://gitlab.com/kraxel/virt-firmware
 Keywords: ovmf,armvirt,edk2,aws
 Description-Content-Type: text/markdown
```

### Comparing `virt-firmware-1.8/README.md` & `virt-firmware-23.4/README.md`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/setup.cfg` & `virt-firmware-23.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = virt-firmware
-version = 1.8
+version = 23.4
 description = tools for virtual machine firmware volumes
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ovmf, armvirt, edk2, aws
 license = GPLv2
 license_files = LICENSE
 author = Gerd Hoffmann
```

### Comparing `virt-firmware-1.8/tests/data/DBXUpdate-20100307.x64.bin` & `virt-firmware-23.4/tests/data/DBXUpdate-20100307.x64.bin`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/tests/data/secboot.aws` & `virt-firmware-23.4/tests/data/secboot.aws`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/tests/test-vars.sh` & `virt-firmware-23.4/tests/test-vars.sh`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/tests/tests.py` & `virt-firmware-23.4/tests/tests.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/aws/dict.v0` & `virt-firmware-23.4/virt/firmware/aws/dict.v0`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/CentOSSecureBootCA2.pem` & `virt-firmware-23.4/virt/firmware/certs/CentOSSecureBootCA2.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/CentOSSecureBootCAkey1.pem` & `virt-firmware-23.4/virt/firmware/certs/CentOSSecureBootCAkey1.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem` & `virt-firmware-23.4/virt/firmware/certs/MicrosoftCorporationKEKCA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem` & `virt-firmware-23.4/virt/firmware/certs/MicrosoftCorporationUEFICA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem` & `virt-firmware-23.4/virt/firmware/certs/MicrosoftWindowsProductionPCA2011.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/RedHatSecureBootCA3.pem` & `virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA3.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/RedHatSecureBootCA5.pem` & `virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA5.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/RedHatSecureBootCA6.pem` & `virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootCA6.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem` & `virt-firmware-23.4/virt/firmware/certs/RedHatSecureBootPKKEKkey1.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/certs/fedoraca-20200709.pem` & `virt-firmware-23.4/virt/firmware/certs/fedoraca-20200709.pem`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/dump.py` & `virt-firmware-23.4/virt/firmware/dump.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/efi/certs.py` & `virt-firmware-23.4/virt/firmware/efi/certs.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/efi/devpath.py` & `virt-firmware-23.4/virt/firmware/efi/devpath.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,14 +73,18 @@
         if self.subtype == 0x0c:
             return 'IPv4()'
         if self.subtype == 0x0d:
             return 'IPv6()'
         if self.subtype == 0x12:
             (port, mul, lun) = struct.unpack_from('=HHH', self.data)
             return f'SATA(port={port})'
+        if self.subtype == 0x13:
+            (proto,login,lun,tag) = struct.unpack_from('=HHQH', self.data)
+            target = self.data[ 14: ].decode()
+            return f'ISCSI({target})'
         if self.subtype == 0x18:
             return f'URI({self.data.decode()})'
         if self.subtype == 0x1f:
             return 'DNS()'
         return f'Msg(subtype=0x{self.subtype:x})'
 
     def fmt_media(self):
```

### Comparing `virt-firmware-1.8/virt/firmware/efi/efijson.py` & `virt-firmware-23.4/virt/firmware/efi/efijson.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/efi/efivar.py` & `virt-firmware-23.4/virt/firmware/efi/efivar.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
             string += f' optdata={optdata.hex()}'
         return string
 
     def fmt_boot_list(self):
         bootlist = []
         for pos in range(len(self.data) >> 1):
             nr = struct.unpack_from('=H', self.data, pos * 2)
-            bootlist.append(f'{nr[0]:04d}')
+            bootlist.append(f'{nr[0]:04x}')
             desc= ", ".join(bootlist)
         return f'boot order: {desc}'
 
     def fmt_dev_path(self):
         obj = devpath.DevicePath(self.data)
         return f'devpath: {obj}'
```

### Comparing `virt-firmware-1.8/virt/firmware/efi/guids.py` & `virt-firmware-23.4/virt/firmware/efi/guids.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/efi/siglist.py` & `virt-firmware-23.4/virt/firmware/efi/siglist.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import struct
 import hashlib
 import logging
 import collections
 
 from cryptography import x509
+from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 
 from virt.firmware.efi import guids
 
 class EfiSigList(collections.UserList):
     """  efi signature list """
 
@@ -45,15 +46,15 @@
         if self.sigsize != 16 + len(data):
             raise ValueError('incorrect signature size')
         if str(self.guid) == guids.EfiCertX509:
             if len(self):
                 raise RuntimeError('x509 signature list not empty')
             if self.x509 is None:
                 try:
-                    self.x509 = x509.load_der_x509_certificate(data)
+                    self.x509 = x509.load_der_x509_certificate(data, default_backend())
                 except ValueError:
                     logging.error("x509: failed to load certificate")
                     self.x509 = None
         sig = { 'guid' : guid,
                 'data' : data }
         self.append(sig)
 
@@ -61,17 +62,17 @@
         if str(self.guid) != guids.EfiCertX509:
             raise RuntimeError('incorrect siglist type guid')
         if len(self):
             raise RuntimeError('x509 signature list not empty')
         with open(filename, "rb") as f:
             pem = f.read()
         if b'-----BEGIN' in pem:
-            self.x509 = x509.load_pem_x509_certificate(pem)
+            self.x509 = x509.load_pem_x509_certificate(pem, default_backend())
         else:
-            self.x509 = x509.load_der_x509_certificate(pem)
+            self.x509 = x509.load_der_x509_certificate(pem, default_backend())
         data = self.x509.public_bytes(serialization.Encoding.DER)
         self.add_sig(guid, data)
 
     def extract_cert(self, prefix = None):
         if self.x509 is None:
             return
         cn = self.x509.subject.get_attributes_for_oid(x509.oid.NameOID.COMMON_NAME)[0]
```

### Comparing `virt-firmware-1.8/virt/firmware/efi/ucs16.py` & `virt-firmware-23.4/virt/firmware/efi/ucs16.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/host.py` & `virt-firmware-23.4/virt/firmware/host.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/migrate.py` & `virt-firmware-23.4/virt/firmware/migrate.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/sigdb.py` & `virt-firmware-23.4/virt/firmware/sigdb.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/vars.py` & `virt-firmware-23.4/virt/firmware/vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,17 @@
     awsstore = None
     varlist = efivar.EfiVarList()
 
     if options.input:
         if edk2.Edk2VarStore.probe(options.input):
             edk2store = edk2.Edk2VarStore(options.input)
             varlist = edk2store.get_varlist()
+        elif edk2.Edk2VarStoreQcow2.probe(options.input):
+            edk2store = edk2.Edk2VarStoreQcow2(options.input)
+            varlist = edk2store.get_varlist()
         elif aws.AwsVarStore.probe(options.input):
             awsstore = aws.AwsVarStore(options.input)
             varlist = awsstore.get_varlist()
         else:
             logging.error("unknown input file format")
             sys.exit(1)
```

### Comparing `virt-firmware-1.8/virt/firmware/varstore/aws.py` & `virt-firmware-23.4/virt/firmware/varstore/aws.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/firmware/varstore/edk2.py` & `virt-firmware-23.4/virt/firmware/varstore/edk2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/python
 """ edk2 varstore parser """
 import sys
 import struct
 import logging
+import tempfile
+import subprocess
 
 from virt.firmware.efi import guids
 from virt.firmware.efi import ucs16
 from virt.firmware.efi import efivar
 
 class Edk2VarStore:
-    """  class for edk2 efi varstore """
+    """  class for edk2 efi varstore, raw image """
 
     def __init__(self, filename):
         self.filename = filename
         self.filedata = b''
         self.start    = None
         self.end      = None
 
@@ -26,15 +28,15 @@
             header = f.read(64)
         guid = guids.parse_bin(header, 16)
         if str(guid) != guids.NvData:
             return False
         return True
 
     def readfile(self):
-        logging.info('reading edk2 varstore from %s', self.filename)
+        logging.info('reading raw edk2 varstore from %s', self.filename)
         with open(self.filename, "rb") as f:
             self.filedata = f.read()
 
     def parse_volume(self):
         guid = guids.parse_bin(self.filedata, 16)
         (vlen, sig, attr, hlen, csum, xoff, rev, blocks, blksize) = \
             struct.unpack_from("=QLLHHHxBLL", self.filedata, 32)
@@ -124,11 +126,46 @@
         blob += self.bytes_varlist(varlist)
         for i in range(self.end - len(blob)):
             blob += b'\xff'
         blob += self.filedata[ self.end : ]
         return blob
 
     def write_varstore(self, filename, varlist):
-        logging.info('writing edk2 varstore to %s', filename)
+        logging.info('writing raw edk2 varstore to %s', filename)
         blob = self.bytes_varstore(varlist)
         with open(filename, "wb") as f:
             f.write(blob)
+
+class Edk2VarStoreQcow2(Edk2VarStore):
+    """  class for edk2 efi varstore, qcow2 image """
+
+    @staticmethod
+    def probe(filename):
+        with open(filename, "rb") as f:
+            header = f.read(64)
+        (magic, version, boff, bsize, mtime, size) = struct.unpack_from('>LLQLLQ', header)
+        if magic != 0x514649fb:
+            return False
+        if size > 1024 * 1024 * 256:
+            return False
+        return True
+
+    def readfile(self):
+        logging.info('reading qcow2 edk2 varstore from %s', self.filename)
+        with tempfile.NamedTemporaryFile() as rawfile:
+            cmdline = [ 'qemu-img', 'convert',
+                        '-f', 'qcow2', '-O', 'raw',
+                        self.filename, rawfile.name ]
+            subprocess.run(cmdline, check = True)
+            self.filedata = rawfile.read()
+
+    def write_varstore(self, filename, varlist):
+        logging.info('writing qcow2 edk2 varstore to %s', filename)
+        blob = self.bytes_varstore(varlist)
+        with tempfile.NamedTemporaryFile() as rawfile:
+            rawfile.write(blob)
+            rawfile.flush()
+            cmdline = [ 'qemu-img', 'convert',
+                        '-f', 'raw', '-O', 'qcow2',
+                        '-o', 'cluster_size=4096', '-S', '4096',
+                        rawfile.name, filename ]
+            subprocess.run(cmdline, check = True)
```

### Comparing `virt-firmware-1.8/virt/firmware/varstore/linux.py` & `virt-firmware-23.4/virt/firmware/varstore/linux.py`

 * *Files identical despite different names*

### Comparing `virt-firmware-1.8/virt/peutils/peutils.py` & `virt-firmware-23.4/virt/peutils/peutils.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,70 +3,125 @@
 import sys
 import struct
 import argparse
 
 import pefile
 
 from cryptography import x509
+from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.serialization import pkcs7
 
+from virt.firmware.efi import guids
+from virt.firmware.efi import siglist
+
 def common_name(item):
     try:
         scn = item.get_attributes_for_oid(x509.oid.NameOID.COMMON_NAME)[0]
         return scn.value
     except IndexError:
         return 'no CN'
 
 def is_ca_cert(cert):
-    bc = cert.extensions.get_extension_for_oid(x509.oid.ExtensionOID.BASIC_CONSTRAINTS)
+    try:
+        bc = cert.extensions.get_extension_for_oid(x509.oid.ExtensionOID.BASIC_CONSTRAINTS)
+    except x509.extensions.ExtensionNotFound:
+        bc = False
     if bc:
         return bc.value.ca
     return False
 
-def print_cert_short(cert):
-    scn = common_name(cert.subject)
-    icn = common_name(cert.issuer)
-    print(f'#             subject CN: {scn}')
-    print(f'#             issuer  CN: {icn}')
-
-def print_cert_long(cert):
-    print(f'#             subject: {cert.subject.rfc4514_string()}')
-    print(f'#             issuer : {cert.issuer.rfc4514_string()}')
-    print(f'#             valid  : {cert.not_valid_before} -> {cert.not_valid_after}')
-    print(f'#             CA     : {is_ca_cert(cert)}')
+def print_cert(cert, verbose = False):
+    print('#          certificate')
+    if verbose:
+        print(f'#             subject: {cert.subject.rfc4514_string()}')
+        print(f'#             issuer : {cert.issuer.rfc4514_string()}')
+        print(f'#             valid  : {cert.not_valid_before} -> {cert.not_valid_after}')
+        print(f'#             CA     : {is_ca_cert(cert)}')
+    else:
+        scn = common_name(cert.subject)
+        icn = common_name(cert.issuer)
+        print(f'#             subject CN: {scn}')
+        print(f'#             issuer  CN: {icn}')
+
+def print_vendor_cert(db, verbose = False):
+    # VENDOR_CERT_FILE
+    try:
+        crt = x509.load_der_x509_certificate(db, default_backend())
+        print_cert(crt, verbose)
+        return
+    except ValueError:
+        pass
+
+    # VENDOR_DB_FILE
+    sigdb = siglist.EfiSigDB(db)
+    for sl in sigdb:
+        if str(sl.guid) == guids.EfiCertX509:
+            print_cert(sl.x509, verbose)
+        elif str(sl.guid) == guids.EfiCertSha256:
+            print('#          sha256')
+            print(f'#             {len(sl)} entries')
+        else:
+            print(f'#          {sl.guid}')
 
 def sig_type2(data, extract = False, verbose = False):
     certs = pkcs7.load_der_pkcs7_certificates(data)
     for cert in certs:
-        print('#          certificate')
-        if verbose:
-            print_cert_long(cert)
-        else:
-            print_cert_short(cert)
+        print_cert(cert, verbose)
 
         if extract:
             scn = common_name(cert.subject)
             fn = "".join(x for x in scn if x.isalnum()) + '.pem'
             print(f'#             >>> {fn}')
             with open(fn, 'wb') as f:
                 f.write(cert.public_bytes(serialization.Encoding.PEM))
 
+def getcstr(data):
+    """ get C string (terminated by null byte) """
+    idx = 0
+    for b in data:
+        if b == 0:
+            break
+        idx += 1
+    return data[:idx]
+
+def pe_string(pe, index):
+    """ lookup string in string table (right after symbol table) """
+    strtab  = pe.FILE_HEADER.PointerToSymbolTable
+    strtab += pe.FILE_HEADER.NumberOfSymbols * 18
+    strtab += index
+    return getcstr(pe.__data__[strtab:])
+
 def efi_binary(filename, extract = False, verbose = False):
     print(f'# file: {filename}')
     pe = pefile.PE(filename)
     for sec in pe.sections:
+        if sec.Name.startswith(b'/'):
+            idx = getcstr(sec.Name[1:])
+            sec.Name = pe_string(pe, int(idx))
         print(f'#    section: 0x{sec.PointerToRawData:06x} +0x{sec.SizeOfRawData:06x}'
               f' ({sec.Name.decode()})')
         if sec.Name == b'.sbat\0\0\0':
             sbat = pe.__data__[ sec.PointerToRawData :
                                 sec.PointerToRawData + sec.SizeOfRawData ]
             entries = sbat.decode().rstrip('\n\0').split('\n')
             for entry in entries:
                 print(f'#       {entry}')
+        if sec.Name == b'.vendor_cert':
+            vcert = pe.__data__[ sec.PointerToRawData :
+                                 sec.PointerToRawData + sec.SizeOfRawData ]
+            (dbs, dbxs, dbo, dbxo) = struct.unpack_from('<IIII', vcert)
+            if dbs:
+                print(f'#       db: {dbo} +{dbs}')
+                db = vcert [ dbo : dbo + dbs ]
+                print_vendor_cert(db, verbose)
+            if dbxs:
+                print(f'#       dbx: {dbxo} +{dbxs}')
+                dbx = vcert [ dbxo : dbxo + dbxs ]
+                print_vendor_cert(dbx, verbose)
     sighdr = pe.OPTIONAL_HEADER.DATA_DIRECTORY[4]
     if sighdr.VirtualAddress and sighdr.Size:
         print(f'#    sigdata: 0x{sighdr.VirtualAddress:06x} +0x{sighdr.Size:06x}')
         sigs = pe.__data__[ sighdr.VirtualAddress :
                             sighdr.VirtualAddress + sighdr.Size ]
         pos = 0
         index = 0
```

### Comparing `virt-firmware-1.8/virt_firmware.egg-info/PKG-INFO` & `virt-firmware-23.4/virt_firmware.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virt-firmware
-Version: 1.8
+Version: 23.4
 Summary: tools for virtual machine firmware volumes
 Author: Gerd Hoffmann
 Author-email: kraxel@redhat.com
 License: GPLv2
 Project-URL: GitLab, https://gitlab.com/kraxel/virt-firmware
 Keywords: ovmf,armvirt,edk2,aws
 Description-Content-Type: text/markdown
```

### Comparing `virt-firmware-1.8/virt_firmware.egg-info/SOURCES.txt` & `virt-firmware-23.4/virt_firmware.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+experimental/dbxupdate.py
+experimental/measure.py
+man/virt-fw-dump.1
+man/virt-fw-dump.inc
+man/virt-fw-sigdb.1
+man/virt-fw-sigdb.inc
+man/virt-fw-vars.1
+man/virt-fw-vars.inc
 tests/test-dump.sh
 tests/test-pe.sh
 tests/test-sigdb.sh
 tests/test-vars.sh
 tests/tests.py
 tests/data/DBXUpdate-20100307.x64.bin
 tests/data/secboot.aws
```

