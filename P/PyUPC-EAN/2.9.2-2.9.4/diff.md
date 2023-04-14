# Comparing `tmp/PyUPC-EAN-2.9.2.tar.gz` & `tmp/PyUPC-EAN-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyUPC-EAN-2.9.2.tar", last modified: Fri Apr 14 20:33:08 2023, max compression
+gzip compressed data, was "PyUPC-EAN-2.9.4.tar", last modified: Fri Apr 14 21:56:14 2023, max compression
```

## Comparing `PyUPC-EAN-2.9.2.tar` & `PyUPC-EAN-2.9.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.864804 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5026 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/pypkg-gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/pyverinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 20:33:08.880804 PyUPC-EAN-2.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    14318 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.864804 PyUPC-EAN-2.9.2/upcean/
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.868804 PyUPC-EAN-2.9.2/upcean/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/convert/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.868804 PyUPC-EAN-2.9.2/upcean/decode/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/barcode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/ean13.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/ean8.py
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/itf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/itf14.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/stf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/upca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/upce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.872804 PyUPC-EAN-2.9.2/upcean/encode/
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19668 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/barcode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19170 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/codabar.py
--rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/code11.py
--rw-r--r--   0 runner    (1001) docker     (123)    47054 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/code128.py
--rw-r--r--   0 runner    (1001) docker     (123)    20661 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/code39.py
--rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/code93.py
--rw-r--r--   0 runner    (1001) docker     (123)    30054 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/ean13.py
--rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/ean2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27897 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/ean5.py
--rw-r--r--   0 runner    (1001) docker     (123)    28053 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/ean8.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/getsfname.py
--rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/goodwill.py
--rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/itf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22327 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/itf14.py
--rw-r--r--   0 runner    (1001) docker     (123)    17934 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/msi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17525 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/plessey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/precairo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/predraw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/prepil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/stf.py
--rw-r--r--   0 runner    (1001) docker     (123)    27194 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/upca.py
--rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/upce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.872804 PyUPC-EAN-2.9.2/upcean/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/OCRA.otf
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/OCRA.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/OCRB.otf
--rw-r--r--   0 runner    (1001) docker     (123)    18764 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/OCRB.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/upcean/getprefix/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/getprefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/getprefix/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    39042 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/getprefix/getprefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/getprefix/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/upcean/oopfuncs/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/oopfuncs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13055 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/oopfuncs/oopfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/oopfuncs/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/upcean/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/validate/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    61700 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/validate/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/upcean/versioninfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/upcean/xml/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.dtd
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.rnc
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.rng
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    50254 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    25521 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.715052 PyUPC-EAN-2.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-14 21:56:14.715052 PyUPC-EAN-2.9.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.703052 PyUPC-EAN-2.9.4/PyUPC_EAN.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-14 21:56:14.000000 PyUPC-EAN-2.9.4/PyUPC_EAN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-14 21:56:14.000000 PyUPC-EAN-2.9.4/PyUPC_EAN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:56:14.000000 PyUPC-EAN-2.9.4/PyUPC_EAN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:56:14.000000 PyUPC-EAN-2.9.4/PyUPC_EAN.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 21:56:14.000000 PyUPC-EAN-2.9.4/PyUPC_EAN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 21:56:14.000000 PyUPC-EAN-2.9.4/PyUPC_EAN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5026 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/pypkg-gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/pyverinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 21:56:14.715052 PyUPC-EAN-2.9.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14318 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.707052 PyUPC-EAN-2.9.4/upcean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.707052 PyUPC-EAN-2.9.4/upcean/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/convert/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.707052 PyUPC-EAN-2.9.4/upcean/decode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/barcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/ean13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/ean8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/itf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/itf14.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/stf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/upca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/decode/upce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.711052 PyUPC-EAN-2.9.4/upcean/encode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19668 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/barcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19170 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/codabar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/code11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47128 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/code128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20661 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/code39.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/code93.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30054 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/ean13.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/ean2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27897 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/ean5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28053 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/ean8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/getsfname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/goodwill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/itf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22327 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/itf14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17934 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/msi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17525 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/plessey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/precairo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/predraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/prepil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/stf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27194 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/upca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/encode/upce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.711052 PyUPC-EAN-2.9.4/upcean/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/fonts/OCRA.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/fonts/OCRA.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/fonts/OCRB.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    18764 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/fonts/OCRB.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.715052 PyUPC-EAN-2.9.4/upcean/getprefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/getprefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/getprefix/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39042 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/getprefix/getprefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/getprefix/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.715052 PyUPC-EAN-2.9.4/upcean/oopfuncs/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/oopfuncs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13055 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/oopfuncs/oopfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/oopfuncs/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.715052 PyUPC-EAN-2.9.4/upcean/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/validate/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61907 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/validate/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-14 21:56:14.000000 PyUPC-EAN-2.9.4/upcean/versioninfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:14.715052 PyUPC-EAN-2.9.4/upcean/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/xml/barcodes.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/xml/barcodes.rnc
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/xml/barcodes.rng
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/xml/barcodes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/xml/barcodes.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    50254 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/xml/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25521 2023-04-14 21:56:04.000000 PyUPC-EAN-2.9.4/upcean/xml/files.py
```

### Comparing `PyUPC-EAN-2.9.2/LICENSE` & `PyUPC-EAN-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/PKG-INFO` & `PyUPC-EAN-2.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyUPC-EAN
-Version: 2.9.2
+Version: 2.9.4
 Summary: A barcode library/module for python.
 Home-page: https://github.com/GameMaker2k/PyUPC-EAN
 Download-URL: https://github.com/GameMaker2k/PyUPC-EAN/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/PKG-INFO` & `PyUPC-EAN-2.9.4/PyUPC_EAN.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyUPC-EAN
-Version: 2.9.2
+Version: 2.9.4
 Summary: A barcode library/module for python.
 Home-page: https://github.com/GameMaker2k/PyUPC-EAN
 Download-URL: https://github.com/GameMaker2k/PyUPC-EAN/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/SOURCES.txt` & `PyUPC-EAN-2.9.4/PyUPC_EAN.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/README.rst` & `PyUPC-EAN-2.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/pypkg-gen.py` & `PyUPC-EAN-2.9.4/pypkg-gen.py`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/pyverinfo.py` & `PyUPC-EAN-2.9.4/pyverinfo.py`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/setup.py` & `PyUPC-EAN-2.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 import re, os, sys, time, datetime, platform, pkg_resources;
 from setuptools import setup, find_packages;
 
 install_requires = [];
 extras_requires = [];
```

### Comparing `PyUPC-EAN-2.9.2/upcean/__init__.py` & `PyUPC-EAN-2.9.4/upcean/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 from upcean.versioninfo import getcuryear, __author__, __copyright__, __credits__, __copyright_year__, __license__, __license_string__, __maintainer__, __email__, __status__, __project__, __project_url__, __version_info__, __build_time__, __build_time_utc__, __build_python_info__, get_build_python_info, __revision__, __revision_id__, __version__, __version_alt__, version_info, __version_date_info__, __version_date__, __version_date_alt__, version_date;
 
 '''
 // UPC Resources and Info
```

### Comparing `PyUPC-EAN-2.9.2/upcean/__main__.py` & `PyUPC-EAN-2.9.4/upcean/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __main__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __main__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, os, argparse;
 pyupceandir = os.path.dirname(__file__);
 sys.path.append(pyupceandir);
 import upcean;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/convert/__init__.py` & `PyUPC-EAN-2.9.4/upcean/convert/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 
 from upcean.convert.convert import *;
 from upcean.convert.shortcuts import *;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/convert/convert.py` & `PyUPC-EAN-2.9.4/upcean/convert/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: convert.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: convert.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.validate;
 
 def make_upca_barcode(numbersystem, manufacturer, product):
  numbersystem = str(numbersystem);
```

### Comparing `PyUPC-EAN-2.9.2/upcean/convert/shortcuts.py` & `PyUPC-EAN-2.9.4/upcean/convert/shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.convert.convert, upcean.support;
 
 
 '''
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/__init__.py` & `PyUPC-EAN-2.9.4/upcean/decode/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 
 '''
 // UPC Resources and Info
 // Source: http://en.wikipedia.org/wiki/Universal_Product_Code
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/barcode.py` & `PyUPC-EAN-2.9.4/upcean/decode/barcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2020 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2020 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: barcode.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: barcode.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.support, upcean.getprefix.getprefix;
 
 ''' // Code for decoding UPC-A by Kazuki Przyborowski '''
 from upcean.decode.upca import *;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/ean13.py` & `PyUPC-EAN-2.9.4/upcean/decode/ean13.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean13.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: ean13.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/ean8.py` & `PyUPC-EAN-2.9.4/upcean/decode/ean8.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean8.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: ean8.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/itf.py` & `PyUPC-EAN-2.9.4/upcean/decode/itf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: itf.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: itf.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/itf14.py` & `PyUPC-EAN-2.9.4/upcean/decode/itf14.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: itf14.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: itf14.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/shortcuts.py` & `PyUPC-EAN-2.9.4/upcean/decode/shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.decode.barcode, upcean.support;
 
 ''' // Shortcut Codes by Kazuki Przyborowski '''
 def decode_barcode(bctype,infile,resize=1,barheight=(48, 54),barwidth=(1, 1),shiftcheck=False,shiftxy=(0, 0),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),locatebarcode=False,imageoutlib="pillow"):
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/stf.py` & `PyUPC-EAN-2.9.4/upcean/decode/stf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: stf.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: stf.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/upca.py` & `PyUPC-EAN-2.9.4/upcean/decode/upca.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: upca.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: upca.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/decode/upce.py` & `PyUPC-EAN-2.9.4/upcean/decode/upce.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: upce.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: upce.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/__init__.py` & `PyUPC-EAN-2.9.4/upcean/encode/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 
 '''
 // UPC Resources and Info
 // Source: http://en.wikipedia.org/wiki/Universal_Product_Code
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/barcode.py` & `PyUPC-EAN-2.9.4/upcean/encode/barcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2020 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2020 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: barcode.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: barcode.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.support, upcean.getprefix.getprefix;
 
 ''' // Code for making EAN-2 supplement by Kazuki Przyborowski '''
 from upcean.encode.ean2 import *;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/codabar.py` & `PyUPC-EAN-2.9.4/upcean/encode/codabar.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: codabar.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: codabar.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/code11.py` & `PyUPC-EAN-2.9.4/upcean/encode/code11.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: code11.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: code11.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/code128.py` & `PyUPC-EAN-2.9.4/upcean/encode/code128.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: code128.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: code128.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 from upcean.validate import convert_ascii_code128_to_hex_code128, convert_text_to_hex_code128_with_checksum, convert_text_to_hex_code128_manual_with_checksum;
 try:
  from io import StringIO, BytesIO;
@@ -424,14 +424,17 @@
    cur_set = 2;
   if(upc_matches[NumZero]=="6a"):
    left_barcolor =  [1, 1, 0, 0, 0, 1, 1, 1, 0, 1, 0];
   if(upc_matches[NumZero]=="6b"):
    left_barcolor =  [1, 1, 0, 1, 0, 1, 1, 1, 0, 0, 0];
   if(upc_matches[NumZero]=="6c"):
    left_barcolor =  [1, 1, 0, 0, 0, 1, 1, 1, 0, 1, 0, 1, 1];
+  if(upc_matches[NumZero]=="6d"):
+   left_barcolor =  [];
+   cur_set = 3;
   if(start_shift==1):
    cur_set = old_cur_set;
    start_shift = 0;
   InnerUPCNum = 0;
   while (InnerUPCNum < len(left_barcolor)):
    if(left_barcolor[InnerUPCNum]==1):
     drawColorLine(upc_img, LineStart, 4, LineStart, LineSize, barwidth[0], barcolor[0], imageoutlib);
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/code39.py` & `PyUPC-EAN-2.9.4/upcean/encode/code39.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: code39.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: code39.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/code93.py` & `PyUPC-EAN-2.9.4/upcean/encode/code93.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: code93.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: code93.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/ean13.py` & `PyUPC-EAN-2.9.4/upcean/encode/ean13.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean13.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: ean13.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/ean2.py` & `PyUPC-EAN-2.9.4/upcean/encode/ean2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean2.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: ean2.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/ean5.py` & `PyUPC-EAN-2.9.4/upcean/encode/ean5.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    FileInfo: ean5.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k
+    FileInfo: ean5.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/ean8.py` & `PyUPC-EAN-2.9.4/upcean/encode/ean8.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean8.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: ean8.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/getsfname.py` & `PyUPC-EAN-2.9.4/upcean/encode/getsfname.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: getsfname.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: getsfname.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, os, re, upcean.support;
 pilsupport = upcean.support.check_for_pil();
 cairosupport = upcean.support.check_for_cairo();
 from upcean.encode.predraw import *;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/goodwill.py` & `PyUPC-EAN-2.9.4/upcean/encode/goodwill.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: goodwill.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: goodwill.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support, upcean.getprefix.getprefix;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/itf.py` & `PyUPC-EAN-2.9.4/upcean/encode/itf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: itf.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: itf.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/itf14.py` & `PyUPC-EAN-2.9.4/upcean/encode/itf14.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: itf14.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: itf14.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/msi.py` & `PyUPC-EAN-2.9.4/upcean/encode/msi.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: msi.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: msi.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/plessey.py` & `PyUPC-EAN-2.9.4/upcean/encode/plessey.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: plessey.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: plessey.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/precairo.py` & `PyUPC-EAN-2.9.4/upcean/encode/precairo.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2011-2023 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: precairo.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1  - Author: cooldude2k $
+    $FileInfo: precairo.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1  - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import cairo, upcean.fonts;
 
 try:
  import pkg_resources;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/predraw.py` & `PyUPC-EAN-2.9.4/upcean/encode/predraw.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: predraw.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: predraw.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.fonts, upcean.support;
 pilsupport = upcean.support.check_for_pil();
 if(pilsupport):
  from PIL import Image, ImageDraw, ImageFont;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/prepil.py` & `PyUPC-EAN-2.9.4/upcean/encode/prepil.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: prepil.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: prepil.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 from PIL import Image, ImageDraw, ImageFont;
 import upcean.fonts;
 
 try:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/shortcuts.py` & `PyUPC-EAN-2.9.4/upcean/encode/shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.encode.barcode, upcean.xml.files, upcean.support;
 
 ''' // Shortcut Codes by Kazuki Przyborowski '''
 def create_barcode(bctype,upc,outfile="./barcode.png",resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/stf.py` & `PyUPC-EAN-2.9.4/upcean/encode/stf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: stf.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: stf.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/upca.py` & `PyUPC-EAN-2.9.4/upcean/encode/upca.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: upca.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: upca.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/encode/upce.py` & `PyUPC-EAN-2.9.4/upcean/encode/upce.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: upce.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: upce.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.2/upcean/fonts/OCRA.otf` & `PyUPC-EAN-2.9.4/upcean/fonts/OCRA.otf`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/upcean/fonts/OCRA.ttf` & `PyUPC-EAN-2.9.4/upcean/fonts/OCRA.ttf`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/upcean/fonts/OCRB.otf` & `PyUPC-EAN-2.9.4/upcean/fonts/OCRB.otf`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/upcean/fonts/OCRB.ttf` & `PyUPC-EAN-2.9.4/upcean/fonts/OCRB.ttf`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/upcean/fonts/__init__.py` & `PyUPC-EAN-2.9.4/upcean/fonts/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import os;
 
 try:
  import pkg_resources;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/getprefix/__init__.py` & `PyUPC-EAN-2.9.4/upcean/getprefix/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.getprefix.getprefix;
 
 from upcean.getprefix.countries import *;
 from upcean.getprefix.getprefix import *;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/getprefix/countries.py` & `PyUPC-EAN-2.9.4/upcean/getprefix/countries.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: countries.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: countries.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.validate;
 
 '''
 // Get GS1 Prefix for EAN-13 EAN-9 barcodes
```

### Comparing `PyUPC-EAN-2.9.2/upcean/getprefix/getprefix.py` & `PyUPC-EAN-2.9.4/upcean/getprefix/getprefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: getprefix.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: getprefix.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.validate, upcean.convert;
 
 def get_upca_barcode_info(upc, infotype=None):
  upc = str(upc);
```

### Comparing `PyUPC-EAN-2.9.2/upcean/getprefix/shortcuts.py` & `PyUPC-EAN-2.9.4/upcean/getprefix/shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.getprefix.getprefix;
 
 '''
 // Shortcut Codes by Kazuki Przyborowski
```

### Comparing `PyUPC-EAN-2.9.2/upcean/oopfuncs/__init__.py` & `PyUPC-EAN-2.9.4/upcean/oopfuncs/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 
 from upcean.oopfuncs.oopfuncs import *;
 from upcean.oopfuncs.shortcuts import *;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/oopfuncs/oopfuncs.py` & `PyUPC-EAN-2.9.4/upcean/oopfuncs/oopfuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: oopfuncs.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: oopfuncs.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.validate, upcean.convert, upcean.getprefix, upcean.encode.getsfname, upcean.support;
 pilsupport = upcean.support.check_for_pil();
 cairosupport = upcean.support.check_for_cairo();
 if(pilsupport or cairosupport):
```

### Comparing `PyUPC-EAN-2.9.2/upcean/oopfuncs/shortcuts.py` & `PyUPC-EAN-2.9.4/upcean/oopfuncs/shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.oopfuncs.oopfuncs, upcean.support;
 
 '''
 // Shortcut Codes by Kazuki Przyborowski
```

### Comparing `PyUPC-EAN-2.9.2/upcean/support.py` & `PyUPC-EAN-2.9.4/upcean/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: support.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: support.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import imp, platform;
 from upcean.versioninfo import getcuryear, __author__, __copyright__, __credits__, __copyright_year__, __license__, __license_string__, __maintainer__, __email__, __status__, __project__, __project_url__, __version_info__, __build_time__, __build_time_utc__, __build_python_info__, __build_python_is_set__, get_build_python_info, __revision__, __version__, __version_alt__, version_info, __version_date_info__, __version_date__, __version_date_alt__, version_date;
 
 ''' // Barcode Support List '''
```

### Comparing `PyUPC-EAN-2.9.2/upcean/validate/__init__.py` & `PyUPC-EAN-2.9.4/upcean/validate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 
 from upcean.validate.validate import *;
 from upcean.validate.shortcuts import *;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/validate/shortcuts.py` & `PyUPC-EAN-2.9.4/upcean/validate/shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.validate.validate, upcean.support;
 
 '''
 // Shortcut Codes by Kazuki Przyborowski
```

### Comparing `PyUPC-EAN-2.9.2/upcean/validate/validate.py` & `PyUPC-EAN-2.9.4/upcean/validate/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: validate.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: validate.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re;
 
 '''
 // Digital Root
@@ -874,15 +874,15 @@
  asciitohex = { ' ': "00", '!': "01", '"': "02", '#': "03", '$': "04", '%': "05", '&': "06", '\'': "07", '(': "08", ')': "09", '*': "0a", '+': "0b", ',': "0c", '-': "0d", '.': "0e", '/': "0f", '0': "10", '1': "11", '2': "12", '3': "13", '4': "14", '5': "15", '6': "16", '7': "17", '8': "18", '9': "19", ':': "1a", ';': "1b", '<': "1c", '=': "1d", '>': "1e", '?': "1f", '@': "20", 'A': "21", 'B': "22", 'C': "23", 'D': "24", 'E': "25", 'F': "26", 'G': "27", 'H': "28", 'I': "29", 'J': "2a", 'K': "2b", 'L': "2c", 'M': "2d", 'N': "2e", 'O': "2f", 'P': "30", 'Q': "31", 'R': "32", 'S': "33", 'T': "34", 'U': "35", 'V': "36", 'W': "37", 'X': "38", 'Y': "39", 'Z': "3a", '[': "3b", '\\': "3c", ']': "3d", '^': "3e", '_': "3f", '`': "40", 'a': "41", 'b': "42", 'c': "43", 'd': "44", 'e': "45", 'f': "46", 'g': "47", 'h': "48", 'i': "49", 'j': "4a", 'k': "4b", 'l': "4c", 'm': "4d", 'n': "4e", 'o': "4f", 'p': "50", 'q': "51", 'r': "52", 's': "53", 't': "54", 'u': "55", 'v': "56", 'w': "57", 'x': "58", 'y': "59", 'z': "5a", '{': "5b", '|': "5c", '}': "5d", '~': "5e", 'Ã': "5f", 'Ä': "60", 'Å': "61", 'Æ': "62", 'Ç': "63", 'È': "64", 'É': "65", 'Ê': "66", 'Ë': "67", 'Ì': "68", 'Í': "69", 'Î': "6a", 'Ï': "6b", 'Î': "6c" };
  barcodeout = "";
  for upcpart in upc:
   barcodeout = barcodeout + hextoascii.get(upcpart, '');
  return barcodeout;
 
 def convert_text_to_hex_code128(upc):
- hextocharsetone = { ' ': "00", '!': "01", '\\': "02", '#': "03", '$': "04", '%': "05", '&': "06", '\'': "07", '(': "08", ')': "09", '*': "0a", '+': "0b", ',': "0c", '-': "0d", '.': "0e", '/': "0f", '10': "0", '1': "11", '2': "12", '3': "13", '4': "14", '5': "15", '6': "16", '7': "17", '8': "18", '9': "19", ':': "1a", ';': "1b", '<': "1c", '=': "1d", '>': "1e", '?': "1f", '@': "20", 'A': "21", 'B': "22", 'C': "23", 'D': "24", 'E': "25", 'F': "26", 'G': "27", 'H': "28", 'I': "29", 'J': "2a", 'K': "2b", 'L': "2c", 'M': "2d", 'N': "2e", 'O': "2f", 'P': "30", 'Q': "31", 'R': "32", 'S': "33", 'T': "34", 'U': "35", 'V': "36", 'W': "37", 'X': "38", 'Y': "39", 'Z': "3a", '[': "3b", '\\': "3c", ']': "3d", '^': "3e", '_': "3f", '\x00': "40", '\x01': "41", '\x02': "42", '\x03': "43", '\x04': "44", '\x05': "45", '\x06': "46", '\x07': "47", '\x08': "48", '\x09': "49", '\x0a': "4a", '\x0b': "4b", '\x0c': "4c", '\x0d': "4d", '\x0e': "4e", '\x0f': "4f", '\x10': "50", '\x11': "51", '\x12': "52", '\x13': "53", '\x14': "54", '\x15': "55", '\x16': "56", '\x17': "57", '\x18': "58", '\x19': "59", '\x1a': "5a", '\x1b': "5b", '\x1c': "5c", '\x1d': "5d", '\x1e': "5e", '\x1f': "5f" };
+ hextocharsetone = { ' ': "00", '!': "01", '\\': "02", '#': "03", '$': "04", '%': "05", '&': "06", '\'': "07", '(': "08", ')': "09", '*': "0a", '+': "0b", ',': "0c", '-': "0d", '.': "0e", '/': "0f", '0': "10", '1': "11", '2': "12", '3': "13", '4': "14", '5': "15", '6': "16", '7': "17", '8': "18", '9': "19", ':': "1a", ';': "1b", '<': "1c", '=': "1d", '>': "1e", '?': "1f", '@': "20", 'A': "21", 'B': "22", 'C': "23", 'D': "24", 'E': "25", 'F': "26", 'G': "27", 'H': "28", 'I': "29", 'J': "2a", 'K': "2b", 'L': "2c", 'M': "2d", 'N': "2e", 'O': "2f", 'P': "30", 'Q': "31", 'R': "32", 'S': "33", 'T': "34", 'U': "35", 'V': "36", 'W': "37", 'X': "38", 'Y': "39", 'Z': "3a", '[': "3b", '\\': "3c", ']': "3d", '^': "3e", '_': "3f", '\x00': "40", '\x01': "41", '\x02': "42", '\x03': "43", '\x04': "44", '\x05': "45", '\x06': "46", '\x07': "47", '\x08': "48", '\x09': "49", '\x0a': "4a", '\x0b': "4b", '\x0c': "4c", '\x0d': "4d", '\x0e': "4e", '\x0f': "4f", '\x10': "50", '\x11': "51", '\x12': "52", '\x13': "53", '\x14': "54", '\x15': "55", '\x16': "56", '\x17': "57", '\x18': "58", '\x19': "59", '\x1a': "5a", '\x1b': "5b", '\x1c': "5c", '\x1d': "5d", '\x1e': "5e", '\x1f': "5f" };
  hextocharsettwo = { ' ': "00", '!': "01", '\\': "02", '#': "03", '$': "04", '%': "05", '&': "06", '\'': "07", '(': "08", ')': "09", '*': "0a", '+': "0b", ',': "0c", '-': "0d", '.': "0e", '/': "0f", '0': "10", '1': "11", '2': "12", '3': "13", '4': "14", '5': "15", '6': "16", '7': "17", '8': "18", '9': "19", ':': "1a", ';': "1b", '<': "1c", '=': "1d", '>': "1e", '?': "1f", '@': "20", 'A': "21", 'B': "22", 'C': "23", 'D': "24", 'E': "25", 'F': "26", 'G': "27", 'H': "28", 'I': "29", 'J': "2a", 'K': "2b", 'L': "2c", 'M': "2d", 'N': "2e", 'O': "2f", 'P': "30", 'Q': "31", 'R': "32", 'S': "33", 'T': "34", 'U': "35", 'V': "36", 'W': "37", 'X': "38", 'Y': "39", 'Z': "3a", '[': "3b", '\\': "3c", ']': "3d", '^': "3e", '_': "3f", '`': "40", 'a': "41", 'b': "42", 'c': "43", 'd': "44", 'e': "45", 'f': "46", 'g': "47", 'h': "48", 'i': "49", 'j': "4a", 'k': "4b", 'l': "4c", 'm': "4d", 'n': "4e", 'o': "4f", 'p': "50", 'q': "51", 'r': "52", 's': "53", 't': "54", 'u': "55", 'v': "56", 'w': "57", 'x': "58", 'y': "59", 'z': "5a", '{': "5b", '|': "5c", '}': "5d", '~': "5e", '\x7f': "5f" };
  hextocharsetthree = { '00': "00", '01': "01", '02': "02", '03': "03", '04': "04", '05': "05", '06': "06", '07': "07", '08': "08", '09': "09", '10': "0a", '11': "0b", '12': "0c", '13': "0d", '14': "0e", '15': "0f", '16': "10", '17': "11", '18': "12", '19': "13", '20': "14", '21': "15", '22': "16", '23': "17", '24': "18", '25': "19", '26': "1a", '27': "1b", '28': "1c", '29': "1d", '30': "1e", '31': "1f", '32': "20", '33': "21", '34': "22", '35': "23", '36': "24", '37': "25", '38': "26", '39': "27", '40': "28", '41': "29", '42': "2a", '43': "2b", '44': "2c", '45': "2d", '46': "2e", '47': "2f", '48': "30", '49': "31", '50': "32", '51': "33", '52': "34", '53': "35", '54': "36", '55': "37", '56': "38", '57': "39", '58': "3a", '59': "3b", '60': "3c", '61': "3d", '62': "3e", '63': "3f", '64': "40", '65': "41", '66': "42", '67': "43", '68': "44", '69': "45", '70': "46", '71': "47", '72': "48", '73': "49", '74': "4a", '75': "4b", '76': "4c", '77': "4d", '78': "4e", '79': "4f", '80': "50", '81': "51", '82': "52", '83': "53", '84': "54", '85': "55", '86': "56", '87': "57", '88': "58", '89': "59", '90': "5a", '91': "5b", '92': "5c", '93': "5d", '94': "5e", '95': "5f", '96': "60", '97': "61", '98': "62", '99': "63", ' ': "64", ' ': "65", ' ': "66", ' ': "67", ' ': "68", ' ': "69", ' ': "6a", ' ': "6b", ' ': "6c" };
  hextocharsetfour = { '32': "00", '194': "00", '207': "00", '212': "00", '252': "00", '33': "01", '34': "02", '35': "03", '36': "04", '37': "05", '38': "06", '39': "07", '40': "08", '41': "09", '42': "0a", '43': "0b", '44': "0c", '45': "0d", '46': "0e", '47': "0f", '48': "10", '49': "11", '50': "12", '51': "13", '52': "14", '53': "15", '54': "16", '55': "17", '56': "18", '57': "19", '58': "1a", '59': "1b", '60': "1c", '61': "1d", '62': "1e", '63': "1f", '64': "20", '65': "21", '66': "22", '67': "23", '68': "24", '69': "25", '70': "26", '71': "27", '72': "28", '73': "29", '74': "2a", '75': "2b", '76': "2c", '77': "2d", '78': "2e", '79': "2f", '80': "30", '81': "31", '82': "32", '83': "33", '84': "34", '85': "35", '86': "36", '87': "37", '88': "38", '89': "39", '90': "3a", '91': "3b", '92': "3c", '93': "3d", '94': "3e", '95': "3f", '96': "40", '97': "41", '98': "42", '99': "43", '100': "44", '101': "45", '102': "46", '103': "47", '104': "48", '105': "49", '106': "4a", '107': "4b", '108': "4c", '109': "4d", '110': "4e", '111': "4f", '112': "50", '113': "51", '114': "52", '115': "53", '116': "54", '117': "55", '118': "56", '119': "57", '120': "58", '121': "59", '122': "5a", '123': "5b", '124': "5c", '125': "5d", '126': "5e", '195': "5f", '200': "5f", '240': "5f", '196': "60", '201': "60", '241': "60", '197': "61", '202': "61", '242': "61", '198': "62", '203': "62", '243': "62", '199': "63", '204': "63", '244': "63", '200': "64", '205': "64", '245': "64", '201': "65", '206': "65", '246': "65", '202': "66", '207': "66", '247': "66", '203': "67", '208': "67", '248': "67", '204': "68", '209': "68", '249': "68", '205': "69", '210': "69", '250': "69", '127': "6a", '128': "6b", '129': "6c" };
  hextoascii = { '60': "Ä", '61': "Å", '62': "Æ", '63': "Ç", '64': "È", '65': "É", '66': "Ê", '67': "Ë", '68': "Ì", '69': "Í", '6a': "Î", '6b': "Ï", '6c': "Î" };
  asciitohex = { 'Ä': "60", 'Å': "61", 'Æ': "62", 'Ç': "63", 'È': "64", 'É': "65", 'Ê': "66", 'Ë': "67", 'Ì': "68", 'Í': "69", 'Î': "6a", 'Ï': "6b", 'Î': "6c" };
  textlen = len(upc);
  textc = 0;
@@ -945,36 +945,38 @@
     textlist.append(hextocharsetone.get(upc[textc], False));
    skipcheck = True;
    if(shiftcharset is None):
     incharset = 1;
    else:
     shiftcharset = None;
   textc += 1;
+ if(not any(textlist)):
+  return False;
  return str(''.join(textlist));
 
 def convert_text_to_hex_code128_manual(upc):
- hextocharsetone = { ' ': "00", '!': "01", '\\': "02", '#': "03", '$': "04", '%': "05", '&': "06", '\'': "07", '(': "08", ')': "09", '*': "0a", '+': "0b", ',': "0c", '-': "0d", '.': "0e", '/': "0f", '10': "0", '1': "11", '2': "12", '3': "13", '4': "14", '5': "15", '6': "16", '7': "17", '8': "18", '9': "19", ':': "1a", ';': "1b", '<': "1c", '=': "1d", '>': "1e", '?': "1f", '@': "20", 'A': "21", 'B': "22", 'C': "23", 'D': "24", 'E': "25", 'F': "26", 'G': "27", 'H': "28", 'I': "29", 'J': "2a", 'K': "2b", 'L': "2c", 'M': "2d", 'N': "2e", 'O': "2f", 'P': "30", 'Q': "31", 'R': "32", 'S': "33", 'T': "34", 'U': "35", 'V': "36", 'W': "37", 'X': "38", 'Y': "39", 'Z': "3a", '[': "3b", '\\': "3c", ']': "3d", '^': "3e", '_': "3f", '\x00': "40", '\x01': "41", '\x02': "42", '\x03': "43", '\x04': "44", '\x05': "45", '\x06': "46", '\x07': "47", '\x08': "48", '\x09': "49", '\x0a': "4a", '\x0b': "4b", '\x0c': "4c", '\x0d': "4d", '\x0e': "4e", '\x0f': "4f", '\x10': "50", '\x11': "51", '\x12': "52", '\x13': "53", '\x14': "54", '\x15': "55", '\x16': "56", '\x17': "57", '\x18': "58", '\x19': "59", '\x1a': "5a", '\x1b': "5b", '\x1c': "5c", '\x1d': "5d", '\x1e': "5e", '\x1f': "5f" };
+ hextocharsetone = { ' ': "00", '!': "01", '\\': "02", '#': "03", '$': "04", '%': "05", '&': "06", '\'': "07", '(': "08", ')': "09", '*': "0a", '+': "0b", ',': "0c", '-': "0d", '.': "0e", '/': "0f", '0': "10", '1': "11", '2': "12", '3': "13", '4': "14", '5': "15", '6': "16", '7': "17", '8': "18", '9': "19", ':': "1a", ';': "1b", '<': "1c", '=': "1d", '>': "1e", '?': "1f", '@': "20", 'A': "21", 'B': "22", 'C': "23", 'D': "24", 'E': "25", 'F': "26", 'G': "27", 'H': "28", 'I': "29", 'J': "2a", 'K': "2b", 'L': "2c", 'M': "2d", 'N': "2e", 'O': "2f", 'P': "30", 'Q': "31", 'R': "32", 'S': "33", 'T': "34", 'U': "35", 'V': "36", 'W': "37", 'X': "38", 'Y': "39", 'Z': "3a", '[': "3b", '\\': "3c", ']': "3d", '^': "3e", '_': "3f", '\x00': "40", '\x01': "41", '\x02': "42", '\x03': "43", '\x04': "44", '\x05': "45", '\x06': "46", '\x07': "47", '\x08': "48", '\x09': "49", '\x0a': "4a", '\x0b': "4b", '\x0c': "4c", '\x0d': "4d", '\x0e': "4e", '\x0f': "4f", '\x10': "50", '\x11': "51", '\x12': "52", '\x13': "53", '\x14': "54", '\x15': "55", '\x16': "56", '\x17': "57", '\x18': "58", '\x19': "59", '\x1a': "5a", '\x1b': "5b", '\x1c': "5c", '\x1d': "5d", '\x1e': "5e", '\x1f': "5f" };
  hextocharsettwo = { ' ': "00", '!': "01", '\\': "02", '#': "03", '$': "04", '%': "05", '&': "06", '\'': "07", '(': "08", ')': "09", '*': "0a", '+': "0b", ',': "0c", '-': "0d", '.': "0e", '/': "0f", '0': "10", '1': "11", '2': "12", '3': "13", '4': "14", '5': "15", '6': "16", '7': "17", '8': "18", '9': "19", ':': "1a", ';': "1b", '<': "1c", '=': "1d", '>': "1e", '?': "1f", '@': "20", 'A': "21", 'B': "22", 'C': "23", 'D': "24", 'E': "25", 'F': "26", 'G': "27", 'H': "28", 'I': "29", 'J': "2a", 'K': "2b", 'L': "2c", 'M': "2d", 'N': "2e", 'O': "2f", 'P': "30", 'Q': "31", 'R': "32", 'S': "33", 'T': "34", 'U': "35", 'V': "36", 'W': "37", 'X': "38", 'Y': "39", 'Z': "3a", '[': "3b", '\\': "3c", ']': "3d", '^': "3e", '_': "3f", '`': "40", 'a': "41", 'b': "42", 'c': "43", 'd': "44", 'e': "45", 'f': "46", 'g': "47", 'h': "48", 'i': "49", 'j': "4a", 'k': "4b", 'l': "4c", 'm': "4d", 'n': "4e", 'o': "4f", 'p': "50", 'q': "51", 'r': "52", 's': "53", 't': "54", 'u': "55", 'v': "56", 'w': "57", 'x': "58", 'y': "59", 'z': "5a", '{': "5b", '|': "5c", '}': "5d", '~': "5e", '\x7f': "5f" };
  hextocharsetthree = { '00': "00", '01': "01", '02': "02", '03': "03", '04': "04", '05': "05", '06': "06", '07': "07", '08': "08", '09': "09", '10': "0a", '11': "0b", '12': "0c", '13': "0d", '14': "0e", '15': "0f", '16': "10", '17': "11", '18': "12", '19': "13", '20': "14", '21': "15", '22': "16", '23': "17", '24': "18", '25': "19", '26': "1a", '27': "1b", '28': "1c", '29': "1d", '30': "1e", '31': "1f", '32': "20", '33': "21", '34': "22", '35': "23", '36': "24", '37': "25", '38': "26", '39': "27", '40': "28", '41': "29", '42': "2a", '43': "2b", '44': "2c", '45': "2d", '46': "2e", '47': "2f", '48': "30", '49': "31", '50': "32", '51': "33", '52': "34", '53': "35", '54': "36", '55': "37", '56': "38", '57': "39", '58': "3a", '59': "3b", '60': "3c", '61': "3d", '62': "3e", '63': "3f", '64': "40", '65': "41", '66': "42", '67': "43", '68': "44", '69': "45", '70': "46", '71': "47", '72': "48", '73': "49", '74': "4a", '75': "4b", '76': "4c", '77': "4d", '78': "4e", '79': "4f", '80': "50", '81': "51", '82': "52", '83': "53", '84': "54", '85': "55", '86': "56", '87': "57", '88': "58", '89': "59", '90': "5a", '91': "5b", '92': "5c", '93': "5d", '94': "5e", '95': "5f", '96': "60", '97': "61", '98': "62", '99': "63" };
  hextocharsetfour = { '32': "00", '194': "00", '207': "00", '212': "00", '252': "00", '33': "01", '34': "02", '35': "03", '36': "04", '37': "05", '38': "06", '39': "07", '40': "08", '41': "09", '42': "0a", '43': "0b", '44': "0c", '45': "0d", '46': "0e", '47': "0f", '48': "10", '49': "11", '50': "12", '51': "13", '52': "14", '53': "15", '54': "16", '55': "17", '56': "18", '57': "19", '58': "1a", '59': "1b", '60': "1c", '61': "1d", '62': "1e", '63': "1f", '64': "20", '65': "21", '66': "22", '67': "23", '68': "24", '69': "25", '70': "26", '71': "27", '72': "28", '73': "29", '74': "2a", '75': "2b", '76': "2c", '77': "2d", '78': "2e", '79': "2f", '80': "30", '81': "31", '82': "32", '83': "33", '84': "34", '85': "35", '86': "36", '87': "37", '88': "38", '89': "39", '90': "3a", '91': "3b", '92': "3c", '93': "3d", '94': "3e", '95': "3f", '96': "40", '97': "41", '98': "42", '99': "43", '100': "44", '101': "45", '102': "46", '103': "47", '104': "48", '105': "49", '106': "4a", '107': "4b", '108': "4c", '109': "4d", '110': "4e", '111': "4f", '112': "50", '113': "51", '114': "52", '115': "53", '116': "54", '117': "55", '118': "56", '119': "57", '120': "58", '121': "59", '122': "5a", '123': "5b", '124': "5c", '125': "5d", '126': "5e", '195': "5f", '200': "5f", '240': "5f", '196': "60", '201': "60", '241': "60", '197': "61", '202': "61", '242': "61", '198': "62", '203': "62", '243': "62", '199': "63", '204': "63", '244': "63", '200': "64", '205': "64", '245': "64", '201': "65", '206': "65", '246': "65", '202': "66", '207': "66", '247': "66", '203': "67", '208': "67", '248': "67", '204': "68", '209': "68", '249': "68", '205': "69", '210': "69", '250': "69", '127': "6a", '128': "6b", '129': "6c" };
  hextoascii = { '60': "Ä", '61': "Å", '62': "Æ", '63': "Ç", '64': "È", '65': "É", '66': "Ê", '67': "Ë", '68': "Ì", '69': "Í", '6a': "Î", '6b': "Ï", '6c': "Î" };
  asciitohex = { 'Ä': "60", 'Å': "61", 'Æ': "62", 'Ç': "63", 'È': "64", 'É': "65", 'Ê': "66", 'Ë': "67", 'Ì': "68", 'Í': "69", 'Î': "6a", 'Ï': "6b", 'Î': "6c" };
  textlen = len(upc);
  textc = 0;
  incharset = None;
  shiftcharset = None;
  textlist = [];
  while(textc < textlen):
   skipcheck = False;
   if(asciitohex.get(upc[textc], False)):
-   if(upc[textc]=="Ë"):
+   if(upc[textc]=="Ë" and textc==0):
     incharset = 1;
-   elif(upc[textc]=="Ì"):
+   elif(upc[textc]=="Ì" and textc==0):
     incharset = 2;
-   elif(upc[textc]=="Í"):
+   elif(upc[textc]=="Í" and textc==0):
     incharset = 3;
    elif(upc[textc]=="Æ"):
     if(incharset==1):
      shiftcharset = 2;
     elif(incharset==2):
      shiftcharset = 1;
    elif(upc[textc]=="Ç" and (incharset==1 or incharset==2)):
@@ -995,23 +997,29 @@
    skipcheck = True;
   elif((incharset==1 and shiftcharset is None) or (shiftcharset==1 and incharset==2)):
    textlist.append(hextocharsetone.get(upc[textc], False));
    if(shiftcharset==1 and incharset==2):
     shiftcharset = None;
    skipcheck = True;
   textc += 1;
+ if(not any(textlist)):
+  return False;
  return str(''.join(textlist));
 
 def convert_text_to_hex_code128_with_checksum(upc):
  code128out = convert_text_to_hex_code128(upc);
- return code128out + get_code128_checksum(code128out)+"6c";
+ if(not code128out):
+  return False;
+ return code128out + "6d" + get_code128_checksum(code128out)+"6c";
 
 def convert_text_to_hex_code128_manual_with_checksum(upc):
  code128out = convert_text_to_hex_code128_manual(upc);
- return code128out + get_code128_checksum(code128out)+"6c";
+ if(not code128out):
+  return False;
+ return code128out + "6d" + get_code128_checksum(code128out)+"6c";
 
 def get_code128alt_checksum(upc):
  upc = str(upc);
  if(len(upc) < 4):
   return False;
  upc = convert_ascii_code128_to_hex_code128(upc);
  return get_code128_checksum(upc);
```

### Comparing `PyUPC-EAN-2.9.2/upcean/versioninfo.py` & `PyUPC-EAN-2.9.4/upcean/versioninfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: versioninfo.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: versioninfo.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import datetime;
 
 getcuryear = datetime.date.today().year;
 if(getcuryear <= 2015):
@@ -63,28 +63,28 @@
 or implied, of Game Maker 2k.
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-""";
 __maintainer__ = "Kazuki Przyborowski";
 __email__ = "kazuki.przyborowski@gmail.com";
 __status__ = "Production";
 __project__ = "PyUPC-EAN";
 __project_url__ = "https://pypi.python.org/pypi/PyUPC-EAN";
-__version_info__ = (2, 9, 2, "RC 1", 1);
-__build_time__ = {"timestamp": 1681504388, "year": 2023, "month": 4, "day": 14, "hour": 20, "minute": 33, "second": 8};
-__build_time_utc__ = {"timestamp": 1681504388, "year": 2023, "month": 4, "day": 14, "hour": 20, "minute": 33, "second": 8};
-__build_python_info__ = {'python_branch': '', 'python_build': ('main', 'Apr  6 2023 07:55:46'), 'python_compiler': 'GCC 11.3.0', 'python_implementation': 'CPython', 'python_revision': '', 'python_version': '3.11.3', 'python_version_tuple': ('3', '11', '3'), 'release': '5.15.0-1035-azure', 'system': 'Linux', 'uname': ('Linux', 'fv-az175-279', '5.15.0-1035-azure', '#42-Ubuntu SMP Tue Feb 28 19:41:23 UTC 2023', 'x86_64', 'x86_64'), 'machine': 'x86_64', 'node': 'fv-az175-279', 'platform': 'Linux-5.15.0-1035-azure-x86_64-with-glibc2.35', 'processor': 'x86_64', 'architecture': ('64bit', 'ELF'), 'version': '#42-Ubuntu SMP Tue Feb 28 19:41:23 UTC 2023', 'java_ver': ('', '', ('', '', ''), ('', '', '')), 'win32_ver': ('', '', '', ''), 'mac_ver': ('', ('', '', ''), ''), 'linux_distribution': None, 'libc_ver': ('glibc', '2.35')};
+__version_info__ = (2, 9, 4, "RC 1", 1);
+__build_time__ = {"timestamp": 1681509374, "year": 2023, "month": 4, "day": 14, "hour": 21, "minute": 56, "second": 14};
+__build_time_utc__ = {"timestamp": 1681509374, "year": 2023, "month": 4, "day": 14, "hour": 21, "minute": 56, "second": 14};
+__build_python_info__ = {'python_branch': '', 'python_build': ('main', 'Apr  6 2023 07:55:46'), 'python_compiler': 'GCC 11.3.0', 'python_implementation': 'CPython', 'python_revision': '', 'python_version': '3.11.3', 'python_version_tuple': ('3', '11', '3'), 'release': '5.15.0-1035-azure', 'system': 'Linux', 'uname': ('Linux', 'fv-az613-440', '5.15.0-1035-azure', '#42-Ubuntu SMP Tue Feb 28 19:41:23 UTC 2023', 'x86_64', 'x86_64'), 'machine': 'x86_64', 'node': 'fv-az613-440', 'platform': 'Linux-5.15.0-1035-azure-x86_64-with-glibc2.35', 'processor': 'x86_64', 'architecture': ('64bit', 'ELF'), 'version': '#42-Ubuntu SMP Tue Feb 28 19:41:23 UTC 2023', 'java_ver': ('', '', ('', '', ''), ('', '', '')), 'win32_ver': ('', '', '', ''), 'mac_ver': ('', ('', '', ''), ''), 'linux_distribution': None, 'libc_ver': ('glibc', '2.35')};
 __build_python_is_set__ = True;
 def get_build_python_info(infotype=None):
  global __build_python_info__;
  python_info = __build_python_info__;
  if(infotype is None):
   return python_info;
  if(infotype is not None):
   return python_info.get(infotype, python_info);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: 44dcb600c3cbb8ade6818cb4bd0deb725a31a50b $";
+__revision_id__ = "$Id: 293a3b8baf9969adaca23ce9fe38dc30aeab8809 $";
 if(__version_info__[3] is not None):
  __version__ = "{major}.{minor}.{build} {release}".format(major=__version_info__[0], minor=__version_info__[1], build=__version_info__[2], release=__version_info__[3]);
 if(__version_info__[3] is None):
  __version__ = "{major}.{minor}.{build}".format(major=__version_info__[0], minor=__version_info__[1], build=__version_info__[2]);
 __version_alt__ = "{major}.{minor}.{build}".format(major=__version_info__[0], minor=__version_info__[1], build=__version_info__[2]);
 def version_info():
  if(__version_info__[3] is not None):
```

### Comparing `PyUPC-EAN-2.9.2/upcean/xml/__init__.py` & `PyUPC-EAN-2.9.4/upcean/xml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import os;
 
 try:
  import pkg_resources;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/xml/barcodes.dtd` & `PyUPC-EAN-2.9.4/upcean/xml/barcodes.dtd`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/upcean/xml/barcodes.rnc` & `PyUPC-EAN-2.9.4/upcean/xml/barcodes.rnc`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/upcean/xml/barcodes.rng` & `PyUPC-EAN-2.9.4/upcean/xml/barcodes.rng`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/upcean/xml/barcodes.xsd` & `PyUPC-EAN-2.9.4/upcean/xml/barcodes.xsd`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/upcean/xml/barcodes.xsl` & `PyUPC-EAN-2.9.4/upcean/xml/barcodes.xsl`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.2/upcean/xml/downloader.py` & `PyUPC-EAN-2.9.4/upcean/xml/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: downloader.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: downloader.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import division, absolute_import, print_function;
 import re, os, sys, hashlib, shutil, platform, tempfile, urllib, gzip, time, cgi, imp;
 import logging as log;
 from upcean.versioninfo import getcuryear, __author__, __copyright__, __credits__, __copyright_year__, __license__, __license_string__, __maintainer__, __email__, __status__, __project__, __project_url__, __version_info__, __build_time__, __build_time_utc__, __build_python_info__, __build_python_is_set__, get_build_python_info, __revision__, __version__, __version_alt__, version_info, __version_date_info__, __version_date__, __version_date_alt__, version_date;
```

### Comparing `PyUPC-EAN-2.9.2/upcean/xml/files.py` & `PyUPC-EAN-2.9.4/upcean/xml/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: files.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: files.py - Last Update: 4/14/2023 Ver. 2.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, re, platform, upcean.validate, upcean.support;
 try:
  import simplejson as json;
 except ImportError:
```

