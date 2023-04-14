# Comparing `tmp/speconed-1.0.0.tar.gz` & `tmp/speconed-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speconed-1.0.0.tar", last modified: Fri Apr 14 07:56:47 2023, max compression
+gzip compressed data, was "speconed-1.0.1.tar", last modified: Fri Apr 14 08:29:30 2023, max compression
```

## Comparing `speconed-1.0.0.tar` & `speconed-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,88 @@
-drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.878183 speconed-1.0.0/
--rw-r--r--   0 jtschindler   (501) staff       (20)     1499 2023-04-14 05:00:23.000000 speconed-1.0.0/LICENSE
--rw-r--r--   0 jtschindler   (501) staff       (20)     2807 2023-04-14 07:56:47.878256 speconed-1.0.0/PKG-INFO
--rw-r--r--   0 jtschindler   (501) staff       (20)      472 2023-04-14 07:46:28.000000 speconed-1.0.0/README.md
--rw-r--r--   0 jtschindler   (501) staff       (20)       86 2023-04-14 06:00:57.000000 speconed-1.0.0/pyproject.toml
--rw-r--r--   0 jtschindler   (501) staff       (20)     1110 2023-04-14 07:56:47.878570 speconed-1.0.0/setup.cfg
--rw-r--r--   0 jtschindler   (501) staff       (20)      125 2023-03-06 14:40:10.000000 speconed-1.0.0/setup.py
-drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.877220 speconed-1.0.0/speconed/
--rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 05:06:10.000000 speconed-1.0.0/speconed/__init__.py
-drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.877995 speconed-1.0.0/speconed/data/
--rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 06:33:26.000000 speconed-1.0.0/speconed/data/__init__.py
-drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.878098 speconed-1.0.0/speconed/data/passbands/
--rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 06:33:40.000000 speconed-1.0.0/speconed/data/passbands/__init__.py
--rw-r--r--   0 jtschindler   (501) staff       (20)   129538 2023-04-14 06:25:17.000000 speconed-1.0.0/speconed/speconed.py
-drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.877883 speconed-1.0.0/speconed.egg-info/
--rw-r--r--   0 jtschindler   (501) staff       (20)     2807 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/PKG-INFO
--rw-r--r--   0 jtschindler   (501) staff       (20)      314 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/SOURCES.txt
--rw-r--r--   0 jtschindler   (501) staff       (20)        1 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/dependency_links.txt
--rw-r--r--   0 jtschindler   (501) staff       (20)      119 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/requires.txt
--rw-r--r--   0 jtschindler   (501) staff       (20)        9 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/top_level.txt
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 08:29:30.250412 speconed-1.0.1/
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1499 2023-04-14 05:00:23.000000 speconed-1.0.1/LICENSE
+-rw-r--r--   0 jtschindler   (501) staff       (20)       74 2023-04-14 08:15:30.000000 speconed-1.0.1/MANIFEST.in
+-rw-r--r--   0 jtschindler   (501) staff       (20)     2807 2023-04-14 08:29:30.250506 speconed-1.0.1/PKG-INFO
+-rw-r--r--   0 jtschindler   (501) staff       (20)      472 2023-04-14 08:19:49.000000 speconed-1.0.1/README.md
+-rw-r--r--   0 jtschindler   (501) staff       (20)       86 2023-04-14 06:00:57.000000 speconed-1.0.1/pyproject.toml
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1064 2023-04-14 08:29:30.250878 speconed-1.0.1/setup.cfg
+-rw-r--r--   0 jtschindler   (501) staff       (20)      150 2023-04-14 08:09:56.000000 speconed-1.0.1/setup.py
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 08:29:30.228384 speconed-1.0.1/speconed/
+-rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 05:06:10.000000 speconed-1.0.1/speconed/__init__.py
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 08:29:30.229143 speconed-1.0.1/speconed/data/
+-rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 06:33:26.000000 speconed-1.0.1/speconed/data/__init__.py
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 08:29:30.242443 speconed-1.0.1/speconed/data/example_spectra/
+-rw-r--r--   0 jtschindler   (501) staff       (20)   581760 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/example_spectra/J030341.04-002321.8_0.fits
+-rw-r--r--   0 jtschindler   (501) staff       (20)  1278720 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/example_spectra/J2125-1719_NIR.fits
+-rwxr-xr-x   0 jtschindler   (501) staff       (20)    60480 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/example_spectra/J2125-1719_OPT_A.fits
+-rwxr-xr-x   0 jtschindler   (501) staff       (20)    60480 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/example_spectra/J2125-1719_OPT_B.fits
+-rw-r--r--   0 jtschindler   (501) staff       (20) 19464190 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/example_spectra/J2125-1719_composite.hdf
+-rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 08:16:00.000000 speconed-1.0.1/speconed/data/example_spectra/__init__.py
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 08:29:30.250316 speconed-1.0.1/speconed/data/passbands/
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1063 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/2MASS-H.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1934 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/2MASS-J.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1387 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/2MASS-Ks.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     2289 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/CAHA_Omega2000-J.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    21744 2023-03-10 08:35:31.000000 speconed-1.0.1/speconed/data/passbands/DECAM-g.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    21744 2023-03-10 08:35:35.000000 speconed-1.0.1/speconed/data/passbands/DECAM-r.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    21744 2023-03-10 08:35:43.000000 speconed-1.0.1/speconed/data/passbands/DECAM-z.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     4674 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/FOURSTAR-J.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     7524 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/FOURSTAR-Ks.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     3516 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/HSC-g.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     3660 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/HSC-i.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     3519 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/HSC-r.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     2915 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/HSC-y.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     2125 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/HSC-z.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    18304 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LCO_RetroCam-J.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)   106721 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LSST-g.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)   104044 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LSST-i.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)   105353 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LSST-r.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    98934 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LSST-u.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)   108845 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LSST-y.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)   101731 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LSST-z.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    12096 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LaSilla_GROND-H.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     9996 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LaSilla_GROND-J.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    12789 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LaSilla_GROND-K.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    31526 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LaSilla_SOFI-H.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    50336 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LaSilla_SOFI-J.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    16412 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LaSilla_SOFI-Js.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    19206 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/LaSilla_SOFI-Ks.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     3717 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/PS1-g.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     3759 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/PS1-i.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     3885 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/PS1-r.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     4385 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/PS1-y.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     3486 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/PS1-z.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    10120 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/Paranal_VISTA-H.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     6446 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/Paranal_VISTA-J.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    11616 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/Paranal_VISTA-Ks.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     4782 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/Paranal_VISTA-Y.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     3402 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/Paranal_VISTA-Z.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     3148 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/README.txt
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1385 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/SDSS-g.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1381 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/SDSS-i.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1190 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/SDSS-r.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)      798 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/SDSS-u.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     2156 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/SDSS-z.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    32677 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/SWIRC-H.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    12258 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/SWIRC-J.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    25849 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/SWIRC-Y.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    16346 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/UKIRT_UKIDSS-H.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     8998 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/UKIRT_UKIDSS-J.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    20900 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/UKIRT_UKIDSS-K.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     6065 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/UKIRT_UKIDSS-Y.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     5166 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/UKIRT_UKIDSS-Z.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)     8468 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/WISE-W1.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    10472 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/WISE-W1_energy.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    11618 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/WISE-W2.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    14372 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/WISE-W2_energy.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    53849 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/WISE-W3.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    66658 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/WISE-W3_energy.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    53849 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/WISE-W4.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)    66658 2022-05-30 16:37:13.000000 speconed-1.0.1/speconed/data/passbands/WISE-W4_energy.dat
+-rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 08:15:49.000000 speconed-1.0.1/speconed/data/passbands/__init__.py
+-rw-r--r--   0 jtschindler   (501) staff       (20)   129538 2023-04-14 06:25:17.000000 speconed-1.0.1/speconed/speconed.py
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 08:29:30.229030 speconed-1.0.1/speconed.egg-info/
+-rw-r--r--   0 jtschindler   (501) staff       (20)     2807 2023-04-14 08:29:30.000000 speconed-1.0.1/speconed.egg-info/PKG-INFO
+-rw-r--r--   0 jtschindler   (501) staff       (20)     2944 2023-04-14 08:29:30.000000 speconed-1.0.1/speconed.egg-info/SOURCES.txt
+-rw-r--r--   0 jtschindler   (501) staff       (20)        1 2023-04-14 08:29:30.000000 speconed-1.0.1/speconed.egg-info/dependency_links.txt
+-rw-r--r--   0 jtschindler   (501) staff       (20)      119 2023-04-14 08:29:30.000000 speconed-1.0.1/speconed.egg-info/requires.txt
+-rw-r--r--   0 jtschindler   (501) staff       (20)        9 2023-04-14 08:29:30.000000 speconed-1.0.1/speconed.egg-info/top_level.txt
```

### Comparing `speconed-1.0.0/LICENSE` & `speconed-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `speconed-1.0.0/PKG-INFO` & `speconed-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speconed
-Version: 1.0.0
+Version: 1.0.1
 Summary: A lightweight package for the manipulation of 1-D astronomical specta
 Home-page: https://github.com/jtschindler/speconed
 Author: Jan-Torge Schindler
 Author-email: schindler@strw.leidenuniv.nl
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jtschindler/speconed/issues
 Keywords: spectroscopy,astronomy,science,python
@@ -16,15 +16,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SpecOneD
-##### (Version 1.0.0)
+##### (Version 1.0.1)
 
 [![Documentation Status](https://readthedocs.org/projects/speconed/badge/?version=latest)](https://speconed.readthedocs.io/en/latest/?badge=latest)
 
 SpecOneD is a lightweight python package that introduces the SpecOneD class for the manipulation of one-dimensional astronomical spectra.
 
 For installation instructions and documentation visit [SpecOneD's ReadTheDocs]
```

### Comparing `speconed-1.0.0/setup.cfg` & `speconed-1.0.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = speconed
-version = 1.0.0
+version = 1.0.1
 author = Jan-Torge Schindler
 author_email = schindler@strw.leidenuniv.nl
 description = A lightweight package for the manipulation of 1-D astronomical specta
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/jtschindler/speconed
 project_urls = 
@@ -40,15 +40,11 @@
 	notebook
 	nbsphinx
 	nbsphinx-link
 	sphinx-rtd-theme
 requirement_files = 
 	requirements.txt
 
-[options.packages.find]
-exclude = 
-	examples
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `speconed-1.0.0/speconed/speconed.py` & `speconed-1.0.1/speconed/speconed.py`

 * *Files identical despite different names*

### Comparing `speconed-1.0.0/speconed.egg-info/PKG-INFO` & `speconed-1.0.1/speconed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speconed
-Version: 1.0.0
+Version: 1.0.1
 Summary: A lightweight package for the manipulation of 1-D astronomical specta
 Home-page: https://github.com/jtschindler/speconed
 Author: Jan-Torge Schindler
 Author-email: schindler@strw.leidenuniv.nl
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jtschindler/speconed/issues
 Keywords: spectroscopy,astronomy,science,python
@@ -16,15 +16,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SpecOneD
-##### (Version 1.0.0)
+##### (Version 1.0.1)
 
 [![Documentation Status](https://readthedocs.org/projects/speconed/badge/?version=latest)](https://speconed.readthedocs.io/en/latest/?badge=latest)
 
 SpecOneD is a lightweight python package that introduces the SpecOneD class for the manipulation of one-dimensional astronomical spectra.
 
 For installation instructions and documentation visit [SpecOneD's ReadTheDocs]
```

