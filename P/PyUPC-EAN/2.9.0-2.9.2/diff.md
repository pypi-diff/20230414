# Comparing `tmp/PyUPC-EAN-2.9.0.tar.gz` & `tmp/PyUPC-EAN-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyUPC-EAN-2.9.0.tar", last modified: Sat Apr  8 01:28:01 2023, max compression
+gzip compressed data, was "PyUPC-EAN-2.9.2.tar", last modified: Fri Apr 14 20:33:08 2023, max compression
```

## Comparing `PyUPC-EAN-2.9.0.tar` & `PyUPC-EAN-2.9.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.787860 PyUPC-EAN-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-08 01:28:01.787860 PyUPC-EAN-2.9.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.767860 PyUPC-EAN-2.9.0/PyUPC_EAN.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-08 01:28:01.000000 PyUPC-EAN-2.9.0/PyUPC_EAN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-08 01:28:01.000000 PyUPC-EAN-2.9.0/PyUPC_EAN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 01:28:01.000000 PyUPC-EAN-2.9.0/PyUPC_EAN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 01:28:01.000000 PyUPC-EAN-2.9.0/PyUPC_EAN.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-08 01:28:01.000000 PyUPC-EAN-2.9.0/PyUPC_EAN.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 01:28:01.000000 PyUPC-EAN-2.9.0/PyUPC_EAN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5026 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/pypkg-gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/pyverinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-08 01:28:01.787860 PyUPC-EAN-2.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    14317 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.767860 PyUPC-EAN-2.9.0/upcean/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.767860 PyUPC-EAN-2.9.0/upcean/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29664 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/convert/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.771860 PyUPC-EAN-2.9.0/upcean/decode/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/barcode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/ean13.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/ean8.py
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/itf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/itf14.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/stf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/upca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/decode/upce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.779860 PyUPC-EAN-2.9.0/upcean/encode/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/barcode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19169 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/codabar.py
--rw-r--r--   0 runner    (1001) docker     (123)    17846 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/code11.py
--rw-r--r--   0 runner    (1001) docker     (123)    47130 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/code128.py
--rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/code39.py
--rw-r--r--   0 runner    (1001) docker     (123)    21197 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/code93.py
--rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/ean13.py
--rw-r--r--   0 runner    (1001) docker     (123)    24055 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/ean2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/ean5.py
--rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/ean8.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/getsfname.py
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/goodwill.py
--rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/itf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22326 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/itf14.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/msi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/plessey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/precairo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/predraw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/prepil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/stf.py
--rw-r--r--   0 runner    (1001) docker     (123)    27193 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/upca.py
--rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/encode/upce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.783860 PyUPC-EAN-2.9.0/upcean/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/fonts/OCRA.otf
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/fonts/OCRA.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/fonts/OCRB.otf
--rw-r--r--   0 runner    (1001) docker     (123)    18764 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/fonts/OCRB.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.783860 PyUPC-EAN-2.9.0/upcean/getprefix/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/getprefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23839 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/getprefix/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    39041 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/getprefix/getprefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/getprefix/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.783860 PyUPC-EAN-2.9.0/upcean/oopfuncs/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/oopfuncs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/oopfuncs/oopfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/oopfuncs/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.783860 PyUPC-EAN-2.9.0/upcean/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/validate/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/validate/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-08 01:28:01.000000 PyUPC-EAN-2.9.0/upcean/versioninfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:28:01.787860 PyUPC-EAN-2.9.0/upcean/xml/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/xml/barcodes.dtd
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/xml/barcodes.rnc
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/xml/barcodes.rng
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/xml/barcodes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/xml/barcodes.xsl
--rw-r--r--   0 runner    (1001) docker     (123)    50253 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/xml/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    25520 2023-04-08 01:27:53.000000 PyUPC-EAN-2.9.0/upcean/xml/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.864804 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5026 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/pypkg-gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/pyverinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 20:33:08.880804 PyUPC-EAN-2.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14318 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.864804 PyUPC-EAN-2.9.2/upcean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.868804 PyUPC-EAN-2.9.2/upcean/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/convert/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.868804 PyUPC-EAN-2.9.2/upcean/decode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/barcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/ean13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/ean8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/itf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/itf14.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/stf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/upca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/decode/upce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.872804 PyUPC-EAN-2.9.2/upcean/encode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19668 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/barcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19170 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/codabar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/code11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47054 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/code128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20661 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/code39.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/code93.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30054 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/ean13.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/ean2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27897 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/ean5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28053 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/ean8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/getsfname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/goodwill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/itf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22327 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/itf14.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17934 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/msi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17525 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/plessey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/precairo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/predraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/prepil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/stf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27194 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/upca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/encode/upce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.872804 PyUPC-EAN-2.9.2/upcean/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/OCRA.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/OCRA.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/OCRB.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    18764 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/OCRB.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/upcean/getprefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/getprefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/getprefix/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39042 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/getprefix/getprefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/getprefix/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/upcean/oopfuncs/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/oopfuncs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13055 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/oopfuncs/oopfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/oopfuncs/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/upcean/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/validate/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61700 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/validate/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-14 20:33:08.000000 PyUPC-EAN-2.9.2/upcean/versioninfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:08.876804 PyUPC-EAN-2.9.2/upcean/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.rnc
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.rng
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/barcodes.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    50254 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25521 2023-04-14 20:32:54.000000 PyUPC-EAN-2.9.2/upcean/xml/files.py
```

### Comparing `PyUPC-EAN-2.9.0/LICENSE` & `PyUPC-EAN-2.9.2/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
 		    Revised BSD License
 
-Copyright (C) 2011-2016 Game Maker 2k. 
+Copyright (C) 2011-2023 Game Maker 2k. 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
   1. Redistributions of source code must retain the above copyright notice,
      this list of conditions and the following disclaimer.
@@ -29,8 +29,8 @@
 CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) 
 ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF 
 THE POSSIBILITY OF SUCH DAMAGE.
 
 The views and conclusions contained in the software and documentation are those of the
 authors and should not be interpreted as representing official policies, either expressed
 or implied, of Game Maker 2k.
--=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
+-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-
```

### Comparing `PyUPC-EAN-2.9.0/PKG-INFO` & `PyUPC-EAN-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyUPC-EAN
-Version: 2.9.0
+Version: 2.9.2
 Summary: A barcode library/module for python.
 Home-page: https://github.com/GameMaker2k/PyUPC-EAN
 Download-URL: https://github.com/GameMaker2k/PyUPC-EAN/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyUPC-EAN-2.9.0/PyUPC_EAN.egg-info/PKG-INFO` & `PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyUPC-EAN
-Version: 2.9.0
+Version: 2.9.2
 Summary: A barcode library/module for python.
 Home-page: https://github.com/GameMaker2k/PyUPC-EAN
 Download-URL: https://github.com/GameMaker2k/PyUPC-EAN/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyUPC-EAN-2.9.0/PyUPC_EAN.egg-info/SOURCES.txt` & `PyUPC-EAN-2.9.2/PyUPC_EAN.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/README.rst` & `PyUPC-EAN-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/pypkg-gen.py` & `PyUPC-EAN-2.9.2/pypkg-gen.py`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/pyverinfo.py` & `PyUPC-EAN-2.9.2/pyverinfo.py`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/setup.py` & `PyUPC-EAN-2.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 import re, os, sys, time, datetime, platform, pkg_resources;
 from setuptools import setup, find_packages;
 
 install_requires = [];
 extras_requires = [];
```

### Comparing `PyUPC-EAN-2.9.0/upcean/__init__.py` & `PyUPC-EAN-2.9.2/upcean/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 from upcean.versioninfo import getcuryear, __author__, __copyright__, __credits__, __copyright_year__, __license__, __license_string__, __maintainer__, __email__, __status__, __project__, __project_url__, __version_info__, __build_time__, __build_time_utc__, __build_python_info__, get_build_python_info, __revision__, __revision_id__, __version__, __version_alt__, version_info, __version_date_info__, __version_date__, __version_date_alt__, version_date;
 
 '''
 // UPC Resources and Info
```

### Comparing `PyUPC-EAN-2.9.0/upcean/__main__.py` & `PyUPC-EAN-2.9.2/upcean/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __main__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __main__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, os, argparse;
 pyupceandir = os.path.dirname(__file__);
 sys.path.append(pyupceandir);
 import upcean;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/convert/__init__.py` & `PyUPC-EAN-2.9.2/upcean/convert/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 
 from upcean.convert.convert import *;
 from upcean.convert.shortcuts import *;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/convert/convert.py` & `PyUPC-EAN-2.9.2/upcean/convert/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: convert.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: convert.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.validate;
 
 def make_upca_barcode(numbersystem, manufacturer, product):
  numbersystem = str(numbersystem);
```

### Comparing `PyUPC-EAN-2.9.0/upcean/convert/shortcuts.py` & `PyUPC-EAN-2.9.2/upcean/convert/shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.convert.convert, upcean.support;
 
 
 '''
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/__init__.py` & `PyUPC-EAN-2.9.2/upcean/decode/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 
 '''
 // UPC Resources and Info
 // Source: http://en.wikipedia.org/wiki/Universal_Product_Code
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/barcode.py` & `PyUPC-EAN-2.9.2/upcean/decode/barcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,42 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2020 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2020 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: barcode.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: barcode.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.support, upcean.getprefix.getprefix;
 
 ''' // Code for decoding UPC-A by Kazuki Przyborowski '''
 from upcean.decode.upca import *;
+import upcean.decode.upca as gtin12;
+import upcean.decode.upca as ucc12;
 ''' // Code for decoding UPC-E by Kazuki Przyborowski '''
 from upcean.decode.upce import *;
 ''' // Code for decoding EAN-13 by Kazuki Przyborowski '''
 from upcean.decode.ean13 import *;
+import upcean.decode.ean13 as gtin13;
+import upcean.decode.ean13 as ucc13;
 ''' // Code for decoding EAN-8 by Kazuki Przyborowski '''
 from upcean.decode.ean8 import *;
+import upcean.decode.ean8 as gtin8;
+import upcean.decode.ean8 as ucc8;
 ''' // Code for making Interleaved 2 of 5 by Kazuki Przyborowski '''
 from upcean.decode.itf import *;
 ''' // Code for making ITF-14 by Kazuki Przyborowski '''
 from upcean.decode.itf14 import *;
+import upcean.decode.itf14 as itf6;
 ''' // Code for making Standard 2 of 5 by Kazuki Przyborowski '''
 from upcean.decode.stf import *;
+import upcean.decode.stf as code25;
 
 def validate_decode_upca_barcode(infile="./upca.png",resize=1,barheight=(48, 54),barwidth=(1, 1),shiftcheck=False,shiftxy=(0, 0),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),locatebarcode=False,imageoutlib="pillow"):
  upc = decode_upca_barcode(infile,resize,barheight,barwidth,shiftcheck,shiftxy,barcolor,locatebarcode,imageoutlib);
  if(len(upc)>12 or len(upc)<12):
   return False;
  if(not upcean.validate.validate_upca_checksum(upc)):
   return False;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/ean13.py` & `PyUPC-EAN-2.9.2/upcean/decode/ean13.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean13.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: ean13.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/ean8.py` & `PyUPC-EAN-2.9.2/upcean/decode/ean8.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean8.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: ean8.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/itf.py` & `PyUPC-EAN-2.9.2/upcean/decode/itf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: itf.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: itf.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/itf14.py` & `PyUPC-EAN-2.9.2/upcean/decode/itf14.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: itf14.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: itf14.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/shortcuts.py` & `PyUPC-EAN-2.9.2/upcean/decode/shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.decode.barcode, upcean.support;
 
 ''' // Shortcut Codes by Kazuki Przyborowski '''
 def decode_barcode(bctype,infile,resize=1,barheight=(48, 54),barwidth=(1, 1),shiftcheck=False,shiftxy=(0, 0),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),locatebarcode=False,imageoutlib="pillow"):
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/stf.py` & `PyUPC-EAN-2.9.2/upcean/decode/stf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: stf.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: stf.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/upca.py` & `PyUPC-EAN-2.9.2/upcean/decode/upca.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: upca.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: upca.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/decode/upce.py` & `PyUPC-EAN-2.9.2/upcean/decode/upce.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: upce.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: upce.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.encode.getsfname, upcean.support;
 try:
  from PIL import Image, UnidentifiedImageError;
  hasuie = True;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/__init__.py` & `PyUPC-EAN-2.9.2/upcean/encode/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 
 '''
 // UPC Resources and Info
 // Source: http://en.wikipedia.org/wiki/Universal_Product_Code
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/barcode.py` & `PyUPC-EAN-2.9.2/upcean/encode/barcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,40 +7,48 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2020 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2020 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: barcode.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: barcode.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.support, upcean.getprefix.getprefix;
 
 ''' // Code for making EAN-2 supplement by Kazuki Przyborowski '''
 from upcean.encode.ean2 import *;
 ''' // Code for making EAN-5 supplement by Kazuki Przyborowski '''
 from upcean.encode.ean5 import *;
 ''' // Code for making UPC-A by Kazuki Przyborowski '''
 from upcean.encode.upca import *;
+import upcean.encode.upca as gtin12;
+import upcean.encode.upca as ucc12;
 ''' // Code for making Goodwill Barcodes by Kazuki Przyborowski '''
 from upcean.encode.goodwill import *;
 ''' // Code for making UPC-E by Kazuki Przyborowski '''
 from upcean.encode.upce import *;
 ''' // Code for making EAN-13 by Kazuki Przyborowski '''
 from upcean.encode.ean13 import *;
+import upcean.encode.ean13 as gtin13;
+import upcean.encode.ean13 as ucc13;
 ''' // Code for making EAN-8 by Kazuki Przyborowski '''
 from upcean.encode.ean8 import *;
+import upcean.encode.ean8 as gtin8;
+import upcean.encode.ean8 as ucc8;
 ''' // Code for making Standard 2 of 5 by Kazuki Przyborowski '''
 from upcean.encode.stf import *;
+import upcean.encode.stf as code25;
 ''' // Code for making Interleaved 2 of 5 by Kazuki Przyborowski '''
 from upcean.encode.itf import *;
 ''' // Code for making ITF-14 by Kazuki Przyborowski '''
 from upcean.encode.itf14 import *;
+import upcean.encode.itf14 as itf6;
 ''' // Code for making Code 11 by Kazuki Przyborowski '''
 from upcean.encode.code11 import *;
 ''' // Code for making Code 39 by Kazuki Przyborowski '''
 from upcean.encode.code39 import *;
 ''' // Code for making Code 93 by Kazuki Przyborowski '''
 from upcean.encode.code93 import *;
 ''' // Code for making Code 128 by Kazuki Przyborowski '''
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/codabar.py` & `PyUPC-EAN-2.9.2/upcean/encode/codabar.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: codabar.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: codabar.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/code11.py` & `PyUPC-EAN-2.9.2/upcean/encode/code11.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: code11.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: code11.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/code128.py` & `PyUPC-EAN-2.9.2/upcean/encode/code128.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,20 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: code128.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: code128.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
+from upcean.validate import convert_ascii_code128_to_hex_code128, convert_text_to_hex_code128_with_checksum, convert_text_to_hex_code128_manual_with_checksum;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
  try:
   from cStringIO import StringIO;
   from cStringIO import StringIO as BytesIO;
  except ImportError:
@@ -29,15 +30,15 @@
 cairosupport = upcean.support.check_for_cairo();
 from upcean.encode.predraw import *;
 if(pilsupport):
  import upcean.encode.prepil;
 if(cairosupport):
  import upcean.encode.precairo;
 
-def create_code128_barcode(upc,outfile="./code128.png",resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+def create_code128hex_barcode(upc,outfile="./code128.png",resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  upc = str(upc).lower();
  hidesn = hideinfo[0];
  hidecd = hideinfo[1];
  hidetext = hideinfo[2];
  imageoutlib = imageoutlib.lower();
  if(not pilsupport and imageoutlib=="pillow"):
   imageoutlib = "cairo";
@@ -488,16 +489,22 @@
   new_upc_img.set_source(upc_imgpat);
   new_upc_img.paint();
   upc_img = new_upc_img;
  if(not hidetext):
   NumTxtZero = 0;
   LineTxtStart = 16;
   while (NumTxtZero < len(upc_print)):
-   drawColorText(upc_img, 10 * int(resize * barwidth[1]), (LineTxtStart + (16 * (int(resize) - 1))) * barwidth[0], cairo_addon_fix + (barheight[0] + (barheight[0] * (int(resize) - 1)) + pil_addon_fix) + (textxy[1] * int(resize)), upc_print[NumTxtZero], barcolor[1], "ocrb", imageoutlib);
-   LineTxtStart += 11 * int(resize);
+   if(len(upc_print[NumTxtZero])==1):
+    drawColorText(upc_img, 10 * int(resize * barwidth[1]), (LineTxtStart + (16 * (int(resize) - 1))) * barwidth[0], cairo_addon_fix + (barheight[0] + (barheight[0] * (int(resize) - 1)) + pil_addon_fix) + (textxy[1] * int(resize)), upc_print[NumTxtZero], barcolor[1], "ocrb", imageoutlib);
+    LineTxtStart += 11 * int(resize);
+   if(len(upc_print[NumTxtZero])==2):
+    drawColorText(upc_img, 10 * int(resize * barwidth[1]), (LineTxtStart + (16 * (int(resize) - 1))) * barwidth[0], cairo_addon_fix + (barheight[0] + (barheight[0] * (int(resize) - 1)) + pil_addon_fix) + (textxy[1] * int(resize)), upc_print[NumTxtZero][0], barcolor[1], "ocrb", imageoutlib);
+    LineTxtStart += 6 * int(resize);
+    drawColorText(upc_img, 10 * int(resize * barwidth[1]), (LineTxtStart + (16 * (int(resize) - 1))) * barwidth[0], cairo_addon_fix + (barheight[0] + (barheight[0] * (int(resize) - 1)) + pil_addon_fix) + (textxy[1] * int(resize)), upc_print[NumTxtZero][1], barcolor[1], "ocrb", imageoutlib);
+    LineTxtStart += 5 * int(resize);
    NumTxtZero += 1;
  del(upc_img);
  exargdict = {};
  if(oldoutfile is None or isinstance(oldoutfile, bool)):
   if(pilsupport and imageoutlib=="pillow"):
    return new_upc_img;
   if(cairosupport and (imageoutlib=="cairo" or imageoutlib=="cairosvg")):
@@ -637,42 +644,20 @@
     else:
      new_upc_preimg.write_to_png(outfile);
      return True;
   except:
    return False;
  return True;
 
-def draw_code128_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+def draw_code128hex_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  return create_code128_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
 
-def encode_code128_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+def encode_code128hex_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  return create_code128_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
 
-def convert_ascii_code128_to_hex_code128(upc):
- upc = str(upc);
- if(len(upc) < 4):
-  return False;
- hextoascii = { '00': " ", '01': "!", '02': "\"", '03': "#", '04': "$", '05': "%", '06': "&", '07': "'", '08': "(", '09': ")", '0a': "*", '0b': "+", '0c': ",", '0d': "-", '0e': ".", '0f': "/", '10': "0", '11': "1", '12': "2", '13': "3", '14': "4", '15': "5", '16': "6", '17': "7", '18': "8", '19': "9", '1a': ":", '1b': ";", '1c': "<", '1d': "=", '1e': ">", '1f': "?", '20': "@", '21': "A", '22': "B", '23': "C", '24': "D", '25': "E", '26': "F", '27': "G", '28': "H", '29': "I", '2a': "J", '2b': "K", '2c': "L", '2d': "M", '2e': "N", '2f': "O", '30': "P", '31': "Q", '32': "R", '33': "S", '34': "T", '35': "U", '36': "V", '37': "W", '38': "X", '39': "Y", '3a': "Z", '3b': "[", '3c': "\\", '3d': "]", '3e': "^", '3f': "_", '40': "`", '41': "a", '42': "b", '43': "c", '44': "d", '45': "e", '46': "f", '47': "g", '48': "h", '49': "i", '4a': "j", '4b': "k", '4c': "l", '4d': "m", '4e': "n", '4f': "o", '50': "p", '51': "q", '52': "r", '53': "s", '54': "t", '55': "u", '56': "v", '57': "w", '58': "x", '59': "y", '5a': "z", '5b': "{", '5c': "|", '5d': "}", '5e': "~", '5f': "Ã", '60': "Ä", '61': "Å", '62': "Æ", '63': "Ç", '64': "È", '65': "É", '66': "Ê", '67': "Ë", '68': "Ì", '69': "Í", '6a': "Î", '6b': "Ï", '6c': "Î" };
- asciitohex = { ' ': "00", '!': "01", '"': "02", '#': "03", '$': "04", '%': "05", '&': "06", '\'': "07", '(': "08", ')': "09", '*': "0a", '+': "0b", ',': "0c", '-': "0d", '.': "0e", '/': "0f", '0': "10", '1': "11", '2': "12", '3': "13", '4': "14", '5': "15", '6': "16", '7': "17", '8': "18", '9': "19", ':': "1a", ';': "1b", '<': "1c", '=': "1d", '>': "1e", '?': "1f", '@': "20", 'A': "21", 'B': "22", 'C': "23", 'D': "24", 'E': "25", 'F': "26", 'G': "27", 'H': "28", 'I': "29", 'J': "2a", 'K': "2b", 'L': "2c", 'M': "2d", 'N': "2e", 'O': "2f", 'P': "30", 'Q': "31", 'R': "32", 'S': "33", 'T': "34", 'U': "35", 'V': "36", 'W': "37", 'X': "38", 'Y': "39", 'Z': "3a", '[': "3b", '\\': "3c", ']': "3d", '^': "3e", '_': "3f", '`': "40", 'a': "41", 'b': "42", 'c': "43", 'd': "44", 'e': "45", 'f': "46", 'g': "47", 'h': "48", 'i': "49", 'j': "4a", 'k': "4b", 'l': "4c", 'm': "4d", 'n': "4e", 'o': "4f", 'p': "50", 'q': "51", 'r': "52", 's': "53", 't': "54", 'u': "55", 'v': "56", 'w': "57", 'x': "58", 'y': "59", 'z': "5a", '{': "5b", '|': "5c", '}': "5d", '~': "5e", 'Ã': "5f", 'Ä': "60", 'Å': "61", 'Æ': "62", 'Ç': "63", 'È': "64", 'É': "65", 'Ê': "66", 'Ë': "67", 'Ì': "68", 'Í': "69", 'Î': "6a", 'Ï': "6b", 'Î': "6c" };
- barcodeout = "";
- for upcpart in upc:
-  barcodeout = barcodeout + asciitohex.get(upcpart, '');
- return barcodeout;
-
-def convert_hex_code128_to_ascii_code128(upc):
- upc = str(upc);
- if(len(upc) < 8):
-  return False;
- hextoascii = { '00': " ", '01': "!", '02': "\"", '03': "#", '04': "$", '05': "%", '06': "&", '07': "'", '08': "(", '09': ")", '0a': "*", '0b': "+", '0c': ",", '0d': "-", '0e': ".", '0f': "/", '10': "0", '11': "1", '12': "2", '13': "3", '14': "4", '15': "5", '16': "6", '17': "7", '18': "8", '19': "9", '1a': ":", '1b': ";", '1c': "<", '1d': "=", '1e': ">", '1f': "?", '20': "@", '21': "A", '22': "B", '23': "C", '24': "D", '25': "E", '26': "F", '27': "G", '28': "H", '29': "I", '2a': "J", '2b': "K", '2c': "L", '2d': "M", '2e': "N", '2f': "O", '30': "P", '31': "Q", '32': "R", '33': "S", '34': "T", '35': "U", '36': "V", '37': "W", '38': "X", '39': "Y", '3a': "Z", '3b': "[", '3c': "\\", '3d': "]", '3e': "^", '3f': "_", '40': "`", '41': "a", '42': "b", '43': "c", '44': "d", '45': "e", '46': "f", '47': "g", '48': "h", '49': "i", '4a': "j", '4b': "k", '4c': "l", '4d': "m", '4e': "n", '4f': "o", '50': "p", '51': "q", '52': "r", '53': "s", '54': "t", '55': "u", '56': "v", '57': "w", '58': "x", '59': "y", '5a': "z", '5b': "{", '5c': "|", '5d': "}", '5e': "~", '5f': "Ã", '60': "Ä", '61': "Å", '62': "Æ", '63': "Ç", '64': "È", '65': "É", '66': "Ê", '67': "Ë", '68': "Ì", '69': "Í", '6a': "Î", '6b': "Ï", '6c': "Î" };
- asciitohex = { ' ': "00", '!': "01", '"': "02", '#': "03", '$': "04", '%': "05", '&': "06", '\'': "07", '(': "08", ')': "09", '*': "0a", '+': "0b", ',': "0c", '-': "0d", '.': "0e", '/': "0f", '0': "10", '1': "11", '2': "12", '3': "13", '4': "14", '5': "15", '6': "16", '7': "17", '8': "18", '9': "19", ':': "1a", ';': "1b", '<': "1c", '=': "1d", '>': "1e", '?': "1f", '@': "20", 'A': "21", 'B': "22", 'C': "23", 'D': "24", 'E': "25", 'F': "26", 'G': "27", 'H': "28", 'I': "29", 'J': "2a", 'K': "2b", 'L': "2c", 'M': "2d", 'N': "2e", 'O': "2f", 'P': "30", 'Q': "31", 'R': "32", 'S': "33", 'T': "34", 'U': "35", 'V': "36", 'W': "37", 'X': "38", 'Y': "39", 'Z': "3a", '[': "3b", '\\': "3c", ']': "3d", '^': "3e", '_': "3f", '`': "40", 'a': "41", 'b': "42", 'c': "43", 'd': "44", 'e': "45", 'f': "46", 'g': "47", 'h': "48", 'i': "49", 'j': "4a", 'k': "4b", 'l': "4c", 'm': "4d", 'n': "4e", 'o': "4f", 'p': "50", 'q': "51", 'r': "52", 's': "53", 't': "54", 'u': "55", 'v': "56", 'w': "57", 'x': "58", 'y': "59", 'z': "5a", '{': "5b", '|': "5c", '}': "5d", '~': "5e", 'Ã': "5f", 'Ä': "60", 'Å': "61", 'Æ': "62", 'Ç': "63", 'È': "64", 'É': "65", 'Ê': "66", 'Ë': "67", 'Ì': "68", 'Í': "69", 'Î': "6a", 'Ï': "6b", 'Î': "6c" };
- barcodeout = "";
- for upcpart in upc:
-  barcodeout = barcodeout + hextoascii.get(upcpart, '');
- return barcodeout;
-
 def create_code128alt_barcode(upc,outfile="./code128.png",resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  upc = str(upc);
  hidesn = hideinfo[0];
  hidecd = hideinfo[1];
  hidetext = hideinfo[2];
  imageoutlib = imageoutlib.lower();
  if(not pilsupport and imageoutlib=="pillow"):
@@ -703,15 +688,15 @@
    if(cairosupport and imageoutlib=="cairo" and outfileext=="SVG"):
     imageoutlib = "cairosvg";
    if(cairosupport and imageoutlib=="cairosvg" and outfileext!="SVG"):
     imageoutlib = "cairo";
  if(len(upc) < 4):
   return False;
  upc = convert_ascii_code128_to_hex_code128(upc);
- return create_code128_barcode(upc,outfile,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+ return create_code128hex_barcode(upc,outfile,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
 
 def draw_code128alt_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  return create_code128alt_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
 
 def encode_code128alt_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  return create_code128alt_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
 
@@ -762,15 +747,106 @@
   dectohex = format(int(upc_matches[i]), 'x');
   dectohexzero = str(dectohex).zfill(2);
   if(len(dectohexzero)>2):
    return False;
   upcout = upcout+str(dectohexzero);
   i = i + 1;
  upc = upcout;
- return create_code128_barcode(upc,outfile,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+ return create_code128hex_barcode(upc,outfile,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
 
 def draw_code128dec_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  return create_code128dec_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
 
 def encode_code128dec_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  return create_code128dec_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
 
+def create_code128_barcode(upc,outfile="./code128.png",resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+ upc = str(upc);
+ hidesn = hideinfo[0];
+ hidecd = hideinfo[1];
+ hidetext = hideinfo[2];
+ imageoutlib = imageoutlib.lower();
+ if(not pilsupport and imageoutlib=="pillow"):
+  imageoutlib = "cairo";
+ if(not cairosupport and (imageoutlib=="cairo" or imageoutlib=="cairosvg")):
+  imageoutlib = "pillow";
+ if(not cairosupport and imageoutlib=="cairosvg"):
+  imageoutlib = "pillow";
+ if(imageoutlib!="pillow" and imageoutlib!="cairo" and imageoutlib!="cairosvg"):
+  imageoutlib = "pillow";
+ if(not pilsupport and not cairosupport):
+  return False;
+ if(outfile is None):
+  if(imageoutlib=="cairosvg"):
+   oldoutfile = None;
+   outfile = None;
+   outfileext = "SVG";
+  else:
+   oldoutfile = None;
+   outfile = None;
+   outfileext = None;
+ else:
+  oldoutfile = upcean.encode.getsfname.get_save_filename(outfile, imageoutlib);
+  if(isinstance(oldoutfile, tuple) or isinstance(oldoutfile, list)):
+   del(outfile);
+   outfile = oldoutfile[0];
+   outfileext = oldoutfile[1];
+   if(cairosupport and imageoutlib=="cairo" and outfileext=="SVG"):
+    imageoutlib = "cairosvg";
+   if(cairosupport and imageoutlib=="cairosvg" and outfileext!="SVG"):
+    imageoutlib = "cairo";
+ if(len(upc) < 4):
+  return False;
+ upc = convert_text_to_hex_code128_with_checksum(upc);
+ return create_code128hex_barcode(upc,outfile,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+
+def draw_code128_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+ return create_code128_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+
+def encode_code128_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+ return create_code128_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+
+def create_code128man_barcode(upc,outfile="./code128.png",resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+ upc = str(upc);
+ hidesn = hideinfo[0];
+ hidecd = hideinfo[1];
+ hidetext = hideinfo[2];
+ imageoutlib = imageoutlib.lower();
+ if(not pilsupport and imageoutlib=="pillow"):
+  imageoutlib = "cairo";
+ if(not cairosupport and (imageoutlib=="cairo" or imageoutlib=="cairosvg")):
+  imageoutlib = "pillow";
+ if(not cairosupport and imageoutlib=="cairosvg"):
+  imageoutlib = "pillow";
+ if(imageoutlib!="pillow" and imageoutlib!="cairo" and imageoutlib!="cairosvg"):
+  imageoutlib = "pillow";
+ if(not pilsupport and not cairosupport):
+  return False;
+ if(outfile is None):
+  if(imageoutlib=="cairosvg"):
+   oldoutfile = None;
+   outfile = None;
+   outfileext = "SVG";
+  else:
+   oldoutfile = None;
+   outfile = None;
+   outfileext = None;
+ else:
+  oldoutfile = upcean.encode.getsfname.get_save_filename(outfile, imageoutlib);
+  if(isinstance(oldoutfile, tuple) or isinstance(oldoutfile, list)):
+   del(outfile);
+   outfile = oldoutfile[0];
+   outfileext = oldoutfile[1];
+   if(cairosupport and imageoutlib=="cairo" and outfileext=="SVG"):
+    imageoutlib = "cairosvg";
+   if(cairosupport and imageoutlib=="cairosvg" and outfileext!="SVG"):
+    imageoutlib = "cairo";
+ if(len(upc) < 4):
+  return False;
+ upc = convert_text_to_hex_code128_manual_with_checksum(upc);
+ return create_code128hex_barcode(upc,outfile,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+
+def draw_code128man_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+ return create_code128man_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+
+def encode_code128man_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+ return create_code128man_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/code39.py` & `PyUPC-EAN-2.9.2/upcean/encode/code39.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: code39.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: code39.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/code93.py` & `PyUPC-EAN-2.9.2/upcean/encode/code93.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: code93.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: code93.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/ean13.py` & `PyUPC-EAN-2.9.2/upcean/encode/ean13.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean13.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: ean13.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/ean2.py` & `PyUPC-EAN-2.9.2/upcean/encode/ean2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean2.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: ean2.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/ean5.py` & `PyUPC-EAN-2.9.2/upcean/encode/ean5.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    FileInfo: ean5.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k
+    FileInfo: ean5.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/ean8.py` & `PyUPC-EAN-2.9.2/upcean/encode/ean8.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: ean8.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: ean8.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/getsfname.py` & `PyUPC-EAN-2.9.2/upcean/encode/getsfname.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: getsfname.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: getsfname.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, os, re, upcean.support;
 pilsupport = upcean.support.check_for_pil();
 cairosupport = upcean.support.check_for_cairo();
 from upcean.encode.predraw import *;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/goodwill.py` & `PyUPC-EAN-2.9.2/upcean/encode/goodwill.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: goodwill.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: goodwill.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support, upcean.getprefix.getprefix;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/itf.py` & `PyUPC-EAN-2.9.2/upcean/encode/itf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: itf.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: itf.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/itf14.py` & `PyUPC-EAN-2.9.2/upcean/encode/itf14.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: itf14.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: itf14.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/msi.py` & `PyUPC-EAN-2.9.2/upcean/encode/msi.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: msi.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: msi.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
@@ -412,7 +412,16 @@
  return True;
 
 def draw_msi_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  return create_msi_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
 
 def encode_msi_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
  return create_msi_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+
+def create_modified_plessey_barcode(upc,outfile="./plessey.png",resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+ return create_msi_barcode(upc,outfile,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+
+def draw_modified_plessey_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+ return create_modified_plessey_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
+
+def encode_modified_plessey_barcode(upc,resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
+ return create_modified_plessey_barcode(upc,None,resize,hideinfo,barheight,barwidth,textxy,barcolor,imageoutlib);
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/plessey.py` & `PyUPC-EAN-2.9.2/upcean/encode/plessey.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: plessey.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: plessey.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/precairo.py` & `PyUPC-EAN-2.9.2/upcean/encode/precairo.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2011-2023 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: precairo.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1  - Author: cooldude2k $
+    $FileInfo: precairo.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1  - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import cairo, upcean.fonts;
 
 try:
  import pkg_resources;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/predraw.py` & `PyUPC-EAN-2.9.2/upcean/encode/predraw.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: predraw.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: predraw.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.fonts, upcean.support;
 pilsupport = upcean.support.check_for_pil();
 if(pilsupport):
  from PIL import Image, ImageDraw, ImageFont;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/prepil.py` & `PyUPC-EAN-2.9.2/upcean/encode/prepil.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: prepil.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: prepil.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 from PIL import Image, ImageDraw, ImageFont;
 import upcean.fonts;
 
 try:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/shortcuts.py` & `PyUPC-EAN-2.9.2/upcean/encode/shortcuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.encode.barcode, upcean.xml.files, upcean.support;
 
 ''' // Shortcut Codes by Kazuki Przyborowski '''
 def create_barcode(bctype,upc,outfile="./barcode.png",resize=1,hideinfo=(False, False, False),barheight=(48, 54),barwidth=(1, 1),textxy=(1, 1, 1),barcolor=((0, 0, 0), (0, 0, 0), (255, 255, 255)),imageoutlib="pillow"):
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/stf.py` & `PyUPC-EAN-2.9.2/upcean/encode/stf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: stf.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: stf.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/upca.py` & `PyUPC-EAN-2.9.2/upcean/encode/upca.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: upca.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: upca.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/encode/upce.py` & `PyUPC-EAN-2.9.2/upcean/encode/upce.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: upce.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: upce.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, sys, upcean.encode.getsfname, upcean.support;
 try:
  from io import StringIO, BytesIO;
 except ImportError:
```

### Comparing `PyUPC-EAN-2.9.0/upcean/fonts/OCRA.otf` & `PyUPC-EAN-2.9.2/upcean/fonts/OCRA.otf`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/upcean/fonts/OCRA.ttf` & `PyUPC-EAN-2.9.2/upcean/fonts/OCRA.ttf`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/upcean/fonts/OCRB.otf` & `PyUPC-EAN-2.9.2/upcean/fonts/OCRB.otf`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/upcean/fonts/OCRB.ttf` & `PyUPC-EAN-2.9.2/upcean/fonts/OCRB.ttf`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/upcean/fonts/__init__.py` & `PyUPC-EAN-2.9.2/upcean/fonts/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import os;
 
 try:
  import pkg_resources;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/getprefix/__init__.py` & `PyUPC-EAN-2.9.2/upcean/oopfuncs/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,14 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
-import upcean.getprefix.getprefix;
 
-from upcean.getprefix.countries import *;
-from upcean.getprefix.getprefix import *;
-from upcean.getprefix.shortcuts import *;
+from upcean.oopfuncs.oopfuncs import *;
+from upcean.oopfuncs.shortcuts import *;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/getprefix/countries.py` & `PyUPC-EAN-2.9.2/upcean/getprefix/countries.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: countries.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: countries.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.validate;
 
 '''
 // Get GS1 Prefix for EAN-13 EAN-9 barcodes
```

### Comparing `PyUPC-EAN-2.9.0/upcean/getprefix/getprefix.py` & `PyUPC-EAN-2.9.2/upcean/getprefix/getprefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: getprefix.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: getprefix.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import re, upcean.validate, upcean.convert;
 
 def get_upca_barcode_info(upc, infotype=None):
  upc = str(upc);
```

### Comparing `PyUPC-EAN-2.9.0/upcean/getprefix/shortcuts.py` & `PyUPC-EAN-2.9.2/upcean/getprefix/shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.getprefix.getprefix;
 
 '''
 // Shortcut Codes by Kazuki Przyborowski
```

### Comparing `PyUPC-EAN-2.9.0/upcean/oopfuncs/__init__.py` & `PyUPC-EAN-2.9.2/upcean/validate/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 
-from upcean.oopfuncs.oopfuncs import *;
-from upcean.oopfuncs.shortcuts import *;
+from upcean.validate.validate import *;
+from upcean.validate.shortcuts import *;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/oopfuncs/oopfuncs.py` & `PyUPC-EAN-2.9.2/upcean/oopfuncs/oopfuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: oopfuncs.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: oopfuncs.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.validate, upcean.convert, upcean.getprefix, upcean.encode.getsfname, upcean.support;
 pilsupport = upcean.support.check_for_pil();
 cairosupport = upcean.support.check_for_cairo();
 if(pilsupport or cairosupport):
```

### Comparing `PyUPC-EAN-2.9.0/upcean/oopfuncs/shortcuts.py` & `PyUPC-EAN-2.9.2/upcean/oopfuncs/shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.oopfuncs.oopfuncs, upcean.support;
 
 '''
 // Shortcut Codes by Kazuki Przyborowski
```

### Comparing `PyUPC-EAN-2.9.0/upcean/support.py` & `PyUPC-EAN-2.9.2/upcean/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: support.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: support.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import imp, platform;
 from upcean.versioninfo import getcuryear, __author__, __copyright__, __credits__, __copyright_year__, __license__, __license_string__, __maintainer__, __email__, __status__, __project__, __project_url__, __version_info__, __build_time__, __build_time_utc__, __build_python_info__, __build_python_is_set__, get_build_python_info, __revision__, __version__, __version_alt__, version_info, __version_date_info__, __version_date__, __version_date_alt__, version_date;
 
 ''' // Barcode Support List '''
```

### Comparing `PyUPC-EAN-2.9.0/upcean/validate/__init__.py` & `PyUPC-EAN-2.9.2/upcean/getprefix/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
+import upcean.getprefix.getprefix;
 
-from upcean.validate.validate import *;
-from upcean.validate.shortcuts import *;
+from upcean.getprefix.countries import *;
+from upcean.getprefix.getprefix import *;
+from upcean.getprefix.shortcuts import *;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/validate/shortcuts.py` & `PyUPC-EAN-2.9.2/upcean/validate/shortcuts.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: shortcuts.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: shortcuts.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import upcean.validate.validate, upcean.support;
 
 '''
 // Shortcut Codes by Kazuki Przyborowski
```

### Comparing `PyUPC-EAN-2.9.0/upcean/versioninfo.py` & `PyUPC-EAN-2.9.2/upcean/versioninfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: versioninfo.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: versioninfo.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import datetime;
 
 getcuryear = datetime.date.today().year;
 if(getcuryear <= 2015):
@@ -63,39 +63,39 @@
 or implied, of Game Maker 2k.
 -=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-""";
 __maintainer__ = "Kazuki Przyborowski";
 __email__ = "kazuki.przyborowski@gmail.com";
 __status__ = "Production";
 __project__ = "PyUPC-EAN";
 __project_url__ = "https://pypi.python.org/pypi/PyUPC-EAN";
-__version_info__ = (2, 9, 0, "RC 1", 1);
-__build_time__ = {"timestamp": 1680917281, "year": 2023, "month": 4, "day": 8, "hour": 1, "minute": 28, "second": 1};
-__build_time_utc__ = {"timestamp": 1680917281, "year": 2023, "month": 4, "day": 8, "hour": 1, "minute": 28, "second": 1};
-__build_python_info__ = {'python_branch': '', 'python_build': ('main', 'Feb  8 2023 08:38:01'), 'python_compiler': 'GCC 11.3.0', 'python_implementation': 'CPython', 'python_revision': '', 'python_version': '3.11.2', 'python_version_tuple': ('3', '11', '2'), 'release': '5.15.0-1035-azure', 'system': 'Linux', 'uname': ('Linux', 'fv-az627-994', '5.15.0-1035-azure', '#42-Ubuntu SMP Tue Feb 28 19:41:23 UTC 2023', 'x86_64', 'x86_64'), 'machine': 'x86_64', 'node': 'fv-az627-994', 'platform': 'Linux-5.15.0-1035-azure-x86_64-with-glibc2.35', 'processor': 'x86_64', 'architecture': ('64bit', 'ELF'), 'version': '#42-Ubuntu SMP Tue Feb 28 19:41:23 UTC 2023', 'java_ver': ('', '', ('', '', ''), ('', '', '')), 'win32_ver': ('', '', '', ''), 'mac_ver': ('', ('', '', ''), ''), 'linux_distribution': None, 'libc_ver': ('glibc', '2.35')};
+__version_info__ = (2, 9, 2, "RC 1", 1);
+__build_time__ = {"timestamp": 1681504388, "year": 2023, "month": 4, "day": 14, "hour": 20, "minute": 33, "second": 8};
+__build_time_utc__ = {"timestamp": 1681504388, "year": 2023, "month": 4, "day": 14, "hour": 20, "minute": 33, "second": 8};
+__build_python_info__ = {'python_branch': '', 'python_build': ('main', 'Apr  6 2023 07:55:46'), 'python_compiler': 'GCC 11.3.0', 'python_implementation': 'CPython', 'python_revision': '', 'python_version': '3.11.3', 'python_version_tuple': ('3', '11', '3'), 'release': '5.15.0-1035-azure', 'system': 'Linux', 'uname': ('Linux', 'fv-az175-279', '5.15.0-1035-azure', '#42-Ubuntu SMP Tue Feb 28 19:41:23 UTC 2023', 'x86_64', 'x86_64'), 'machine': 'x86_64', 'node': 'fv-az175-279', 'platform': 'Linux-5.15.0-1035-azure-x86_64-with-glibc2.35', 'processor': 'x86_64', 'architecture': ('64bit', 'ELF'), 'version': '#42-Ubuntu SMP Tue Feb 28 19:41:23 UTC 2023', 'java_ver': ('', '', ('', '', ''), ('', '', '')), 'win32_ver': ('', '', '', ''), 'mac_ver': ('', ('', '', ''), ''), 'linux_distribution': None, 'libc_ver': ('glibc', '2.35')};
 __build_python_is_set__ = True;
 def get_build_python_info(infotype=None):
  global __build_python_info__;
  python_info = __build_python_info__;
  if(infotype is None):
   return python_info;
  if(infotype is not None):
   return python_info.get(infotype, python_info);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: 58a7e2a27aaab65000af83df819a6e3987c895d4 $";
+__revision_id__ = "$Id: 44dcb600c3cbb8ade6818cb4bd0deb725a31a50b $";
 if(__version_info__[3] is not None):
  __version__ = "{major}.{minor}.{build} {release}".format(major=__version_info__[0], minor=__version_info__[1], build=__version_info__[2], release=__version_info__[3]);
 if(__version_info__[3] is None):
  __version__ = "{major}.{minor}.{build}".format(major=__version_info__[0], minor=__version_info__[1], build=__version_info__[2]);
 __version_alt__ = "{major}.{minor}.{build}".format(major=__version_info__[0], minor=__version_info__[1], build=__version_info__[2]);
 def version_info():
  if(__version_info__[3] is not None):
   return {"major": __version_info__[0], "minor": __version_info__[1], "build": __version_info__[2], "release": __version_info__[3]};
  if(__version_info__[3] is None):
   return {"major": __version_info__[0], "minor": __version_info__[1], "build": __version_info__[2], "release": None};
-__version_date_info__ = (2023, 4, 7, "RC 1", 1);
+__version_date_info__ = (2023, 4, 14, "RC 1", 1);
 def version_date():
  if(__version_date_info__[3] is not None):
   return {"year":__version_date_info__[0], "month": __version_date_info__[1], "day": __version_date_info__[2], "release": __version_date_info__[3]};
  if(__version_date_info__[3] is None):
   return {"year":__version_date_info__[0], "month": __version_date_info__[1], "day": __version_date_info__[2], "release": None};
 __version_date__ = "{year}.{month}.{day}".format(year=__version_date_info__[0], month=__version_date_info__[1], day=__version_date_info__[2]);
 __version_date_alt__ = "{year}.{month}.{day} {release}".format(year=__version_date_info__[0], month=__version_date_info__[1], day=__version_date_info__[2], release=__version_date_info__[2]);
```

### Comparing `PyUPC-EAN-2.9.0/upcean/xml/__init__.py` & `PyUPC-EAN-2.9.2/upcean/xml/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: __init__.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: __init__.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import os;
 
 try:
  import pkg_resources;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/xml/barcodes.dtd` & `PyUPC-EAN-2.9.2/upcean/xml/barcodes.dtd`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/upcean/xml/barcodes.rnc` & `PyUPC-EAN-2.9.2/upcean/xml/barcodes.rnc`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/upcean/xml/barcodes.rng` & `PyUPC-EAN-2.9.2/upcean/xml/barcodes.rng`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/upcean/xml/barcodes.xsd` & `PyUPC-EAN-2.9.2/upcean/xml/barcodes.xsd`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/upcean/xml/barcodes.xsl` & `PyUPC-EAN-2.9.2/upcean/xml/barcodes.xsl`

 * *Files identical despite different names*

### Comparing `PyUPC-EAN-2.9.0/upcean/xml/downloader.py` & `PyUPC-EAN-2.9.2/upcean/xml/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: downloader.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: downloader.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import division, absolute_import, print_function;
 import re, os, sys, hashlib, shutil, platform, tempfile, urllib, gzip, time, cgi, imp;
 import logging as log;
 from upcean.versioninfo import getcuryear, __author__, __copyright__, __credits__, __copyright_year__, __license__, __license_string__, __maintainer__, __email__, __status__, __project__, __project_url__, __version_info__, __build_time__, __build_time_utc__, __build_python_info__, __build_python_is_set__, get_build_python_info, __revision__, __version__, __version_alt__, version_info, __version_date_info__, __version_date__, __version_date_alt__, version_date;
```

### Comparing `PyUPC-EAN-2.9.0/upcean/xml/files.py` & `PyUPC-EAN-2.9.2/upcean/xml/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2011-2023 Game Maker 2k - https://github.com/GameMaker2k
     Copyright 2011-2023 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: files.py - Last Update: 4/7/2023 Ver. 2.9.0 RC 1 - Author: cooldude2k $
+    $FileInfo: files.py - Last Update: 4/14/2023 Ver. 2.9.2 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, re, platform, upcean.validate, upcean.support;
 try:
  import simplejson as json;
 except ImportError:
```

