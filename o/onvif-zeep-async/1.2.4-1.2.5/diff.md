# Comparing `tmp/onvif-zeep-async-1.2.4.tar.gz` & `tmp/onvif-zeep-async-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-1.2.4.tar", last modified: Thu Apr 13 23:24:59 2023, max compression
+gzip compressed data, was "onvif-zeep-async-1.2.5.tar", last modified: Fri Apr 14 01:53:19 2023, max compression
```

## Comparing `onvif-zeep-async-1.2.4.tar` & `onvif-zeep-async-1.2.5.tar`

### file list

```diff
@@ -1,58 +1,70 @@
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/CHANGES.txt
--rw-r--r--   0 jason     (1000) jason     (1000)     1087 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)      100 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/MANIFEST.in
--rw-rw-r--   0 jason     (1000) jason     (1000)     6667 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)     4926 2021-08-27 21:44:54.000000 onvif-zeep-async-1.2.4/README.rst
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-13 23:24:59.953377 onvif-zeep-async-1.2.4/onvif/
--rw-rw-r--   0 jason     (1000) jason     (1000)      599 2020-10-18 04:42:45.000000 onvif-zeep-async-1.2.4/onvif/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)    18227 2023-04-13 23:24:18.000000 onvif-zeep-async-1.2.4/onvif/client.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2190 2020-05-18 19:22:35.000000 onvif-zeep-async-1.2.4/onvif/definition.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      886 2020-10-18 04:42:45.000000 onvif-zeep-async-1.2.4/onvif/exceptions.py
--rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-04-13 23:24:33.000000 onvif-zeep-async-1.2.4/onvif/version.txt
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/onvif/wsdl/
--rw-r--r--   0 jason     (1000) jason     (1000)       26 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)    38072 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    57255 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     7263 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/addressing
--rw-r--r--   0 jason     (1000) jason     (1000)    79284 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    24131 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    31976 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    23300 2020-05-07 15:00:34.000000 onvif-zeep-async-1.2.4/onvif/wsdl/b-2.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     5100 2020-05-07 04:46:04.000000 onvif-zeep-async-1.2.4/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)    20498 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    60231 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)   163209 2020-05-07 14:59:35.000000 onvif-zeep-async-1.2.4/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    24593 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/display.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    53648 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     6249 2020-05-07 14:59:35.000000 onvif-zeep-async-1.2.4/onvif/wsdl/envelope
--rw-r--r--   0 jason     (1000) jason     (1000)    37870 2020-05-18 19:48:12.000000 onvif-zeep-async-1.2.4/onvif/wsdl/events.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    17998 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)      511 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/include
--rw-r--r--   0 jason     (1000) jason     (1000)   174812 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/media.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)   363349 2020-05-07 14:59:35.000000 onvif-zeep-async-1.2.4/onvif/wsdl/onvif.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)    54058 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     3660 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/r-2.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)    17214 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    40704 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/recording.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     5596 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    10581 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/replay.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     3727 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    43139 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/search.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     8960 2020-05-07 04:45:04.000000 onvif-zeep-async-1.2.4/onvif/wsdl/t-1.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     3738 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/types.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     5849 2020-05-07 04:44:07.000000 onvif-zeep-async-1.2.4/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)    10455 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     8836 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/xml.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     1639 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/xmlmime
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/
--rw-rw-r--   0 jason     (1000) jason     (1000)     6667 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)     1255 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/SOURCES.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/dependency_links.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)       46 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/entry_points.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/not-zip-safe
--rw-rw-r--   0 jason     (1000) jason     (1000)       47 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/requires.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/top_level.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)       77 2020-10-18 04:42:45.000000 onvif-zeep-async-1.2.4/pyproject.toml
--rw-rw-r--   0 jason     (1000) jason     (1000)      409 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/setup.cfg
--rw-rw-r--   0 jason     (1000) jason     (1000)     1801 2021-08-27 21:44:54.000000 onvif-zeep-async-1.2.4/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 01:53:19.638491 onvif-zeep-async-1.2.5/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.5/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.5/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-14 01:53:19.638590 onvif-zeep-async-1.2.5/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 01:53:19.628505 onvif-zeep-async-1.2.5/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 01:53:19.629094 onvif-zeep-async-1.2.5/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    19078 2023-04-14 01:52:17.000000 onvif-zeep-async-1.2.5/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-14 01:52:45.000000 onvif-zeep-async-1.2.5/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 01:53:19.637443 onvif-zeep-async-1.2.5/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 01:53:19.638260 onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-14 01:53:19.000000 onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1417 2023-04-14 01:53:19.000000 onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-14 01:53:19.000000 onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-04-14 01:53:19.000000 onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-04-14 01:53:19.000000 onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-14 01:53:19.000000 onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-04-14 01:53:19.638869 onvif-zeep-async-1.2.5/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 01:53:19.638375 onvif-zeep-async-1.2.5/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.5/tests/test.py
```

### Comparing `onvif-zeep-async-1.2.4/LICENSE` & `onvif-zeep-async-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/PKG-INFO` & `onvif-zeep-async-1.2.5/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,185 +1,171 @@
-Metadata-Version: 1.2
-Name: onvif-zeep-async
-Version: 1.2.4
-Summary: Async Python Client for ONVIF Camera
-Home-page: http://github.com/hunterjm/python-onvif-zeep-async
-Author: Cherish Chen
-Author-email: sinchb128@gmail.com
-Maintainer: sinchb
-Maintainer-email: sinchb128@gmail.com
-License: MIT
-Description: python-onvif-zeep-async
-        =======================
-        
-        ONVIF Client Implementation in Python 3
-        
-        Dependencies
-        ------------
-        `zeep[async] <http://docs.python-zeep.org>`_ >= 4.1.0, < 5.0.0
-        `httpx <https://www.python-httpx.org/>`_ >= 0.19.0, < 1.0.0
-        
-        Install python-onvif-zeep-async
-        -------------------------------
-        **From Source**
-        
-        You should clone this repository and run setup.py::
-        
-            cd python-onvif-zeep-async && python setup.py install
-        
-        Alternatively, you can run::
-        
-            pip install --upgrade onvif-zeep-async
-        
-        
-        Getting Started
-        ---------------
-        
-        Initialize an ONVIFCamera instance
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            from onvif import ONVIFCamera
-            mycam = ONVIFCamera('192.168.0.2', 80, 'user', 'passwd', '/etc/onvif/wsdl/')
-            await mycam.update_xaddrs()
-        
-        Now, an ONVIFCamera instance is available. By default, a devicemgmt service is also available if everything is OK.
-        
-        So, all operations defined in the WSDL document::
-        
-        /etc/onvif/wsdl/devicemgmt.wsdl
-        
-        are available.
-        
-        Get information from your camera
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        ::
-        
-            # Get Hostname
-            resp = await mycam.devicemgmt.GetHostname()
-            print 'My camera`s hostname: ' + str(resp.Name)
-        
-            # Get system date and time
-            dt = await mycam.devicemgmt.GetSystemDateAndTime()
-            tz = dt.TimeZone
-            year = dt.UTCDateTime.Date.Year
-            hour = dt.UTCDateTime.Time.Hour
-        
-        Configure (Control) your camera
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To configure your camera, there are two ways to pass parameters to service methods.
-        
-        **Dict**
-        
-        This is the simpler way::
-        
-            params = {'Name': 'NewHostName'}
-            await device_service.SetHostname(params)
-        
-        **Type Instance**
-        
-        This is the recommended way. Type instance will raise an
-        exception if you set an invalid (or non-existent) parameter.
-        
-        ::
-        
-            params = mycam.devicemgmt.create_type('SetHostname')
-            params.Hostname = 'NewHostName'
-            await mycam.devicemgmt.SetHostname(params)
-        
-            time_params = mycam.devicemgmt.create_type('SetSystemDateAndTime')
-            time_params.DateTimeType = 'Manual'
-            time_params.DaylightSavings = True
-            time_params.TimeZone.TZ = 'CST-8:00:00'
-            time_params.UTCDateTime.Date.Year = 2014
-            time_params.UTCDateTime.Date.Month = 12
-            time_params.UTCDateTime.Date.Day = 3
-            time_params.UTCDateTime.Time.Hour = 9
-            time_params.UTCDateTime.Time.Minute = 36
-            time_params.UTCDateTime.Time.Second = 11
-            await mycam.devicemgmt.SetSystemDateAndTime(time_params)
-        
-        Use other services
-        ~~~~~~~~~~~~~~~~~~
-        ONVIF protocol has defined many services.
-        You can find all the services and operations `here <http://www.onvif.org/onvif/ver20/util/operationIndex.html>`_.
-        ONVIFCamera has support methods to create new services::
-        
-            # Create ptz service
-            ptz_service = mycam.create_ptz_service()
-            # Get ptz configuration
-            await mycam.ptz.GetConfiguration()
-            # Another way
-            # await ptz_service.GetConfiguration()
-        
-        Or create an unofficial service::
-        
-            xaddr = 'http://192.168.0.3:8888/onvif/yourservice'
-            yourservice = mycam.create_onvif_service('service.wsdl', xaddr, 'yourservice')
-            await yourservice.SomeOperation()
-            # Another way
-            # await mycam.yourservice.SomeOperation()
-        
-        ONVIF CLI
-        ---------
-        python-onvif also provides a command line interactive interface: onvif-cli.
-        onvif-cli is installed automatically.
-        
-        Single command example
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            $ onvif-cli devicemgmt GetHostname --user 'admin' --password '12345' --host '192.168.0.112' --port 80
-            True: {'FromDHCP': True, 'Name': hision}
-            $ onvif-cli devicemgmt SetHostname "{'Name': 'NewerHostname'}" --user 'admin' --password '12345' --host '192.168.0.112' --port 80
-            True: {}
-        
-        Interactive mode
-        ~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            $ onvif-cli -u 'admin' -a '12345' --host '192.168.0.112' --port 80 --wsdl /etc/onvif/wsdl/
-            ONVIF >>> cmd
-            analytics   devicemgmt  events      imaging     media       ptz
-            ONVIF >>> cmd devicemgmt GetWsdlUrl
-            True: http://www.onvif.org/
-            ONVIF >>> cmd devicemgmt SetHostname {'Name': 'NewHostname'}
-            ONVIF >>> cmd devicemgmt GetHostname
-            True: {'Name': 'NewHostName'}
-            ONVIF >>> cmd devicemgmt SomeOperation
-            False: No Operation: SomeOperation
-        
-        NOTE: Tab completion is supported for interactive mode.
-        
-        Batch mode
-        ~~~~~~~~~~
-        
-        ::
-        
-            $ vim batchcmds
-            $ cat batchcmds
-            cmd devicemgmt GetWsdlUrl
-            cmd devicemgmt SetHostname {'Name': 'NewHostname', 'FromDHCP': True}
-            cmd devicemgmt GetHostname
-            $ onvif-cli --host 192.168.0.112 -u admin -a 12345 -w /etc/onvif/wsdl/ < batchcmds
-            ONVIF >>> True: http://www.onvif.org/
-            ONVIF >>> True: {}
-            ONVIF >>> True: {'FromDHCP': False, 'Name': NewHostname}
-        
-        References
-        ----------
-        
-        * `ONVIF Offical Website <http://www.onvif.com>`_
-        
-        * `Operations Index <http://www.onvif.org/onvif/ver20/util/operationIndex.html>`_
-        
-        * `ONVIF Develop Documents <http://www.onvif.org/specs/DocMap-2.4.2.html>`_
-        
-        * `Foscam Python Lib <http://github.com/quatanium/foscam-python-lib>`_
-        
-Keywords: ONVIF,Camera,IPC
-Platform: UNKNOWN
-Requires-Python: >=3
+python-onvif-zeep-async
+=======================
+
+ONVIF Client Implementation in Python 3
+
+Dependencies
+------------
+`zeep[async] <http://docs.python-zeep.org>`_ >= 4.1.0, < 5.0.0
+`httpx <https://www.python-httpx.org/>`_ >= 0.19.0, < 1.0.0
+
+Install python-onvif-zeep-async
+-------------------------------
+**From Source**
+
+You should clone this repository and run setup.py::
+
+    cd python-onvif-zeep-async && python setup.py install
+
+Alternatively, you can run::
+
+    pip install --upgrade onvif-zeep-async
+
+
+Getting Started
+---------------
+
+Initialize an ONVIFCamera instance
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    from onvif import ONVIFCamera
+    mycam = ONVIFCamera('192.168.0.2', 80, 'user', 'passwd', '/etc/onvif/wsdl/')
+    await mycam.update_xaddrs()
+
+Now, an ONVIFCamera instance is available. By default, a devicemgmt service is also available if everything is OK.
+
+So, all operations defined in the WSDL document::
+
+/etc/onvif/wsdl/devicemgmt.wsdl
+
+are available.
+
+Get information from your camera
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+::
+
+    # Get Hostname
+    resp = await mycam.devicemgmt.GetHostname()
+    print 'My camera`s hostname: ' + str(resp.Name)
+
+    # Get system date and time
+    dt = await mycam.devicemgmt.GetSystemDateAndTime()
+    tz = dt.TimeZone
+    year = dt.UTCDateTime.Date.Year
+    hour = dt.UTCDateTime.Time.Hour
+
+Configure (Control) your camera
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To configure your camera, there are two ways to pass parameters to service methods.
+
+**Dict**
+
+This is the simpler way::
+
+    params = {'Name': 'NewHostName'}
+    await device_service.SetHostname(params)
+
+**Type Instance**
+
+This is the recommended way. Type instance will raise an
+exception if you set an invalid (or non-existent) parameter.
+
+::
+
+    params = mycam.devicemgmt.create_type('SetHostname')
+    params.Hostname = 'NewHostName'
+    await mycam.devicemgmt.SetHostname(params)
+
+    time_params = mycam.devicemgmt.create_type('SetSystemDateAndTime')
+    time_params.DateTimeType = 'Manual'
+    time_params.DaylightSavings = True
+    time_params.TimeZone.TZ = 'CST-8:00:00'
+    time_params.UTCDateTime.Date.Year = 2014
+    time_params.UTCDateTime.Date.Month = 12
+    time_params.UTCDateTime.Date.Day = 3
+    time_params.UTCDateTime.Time.Hour = 9
+    time_params.UTCDateTime.Time.Minute = 36
+    time_params.UTCDateTime.Time.Second = 11
+    await mycam.devicemgmt.SetSystemDateAndTime(time_params)
+
+Use other services
+~~~~~~~~~~~~~~~~~~
+ONVIF protocol has defined many services.
+You can find all the services and operations `here <http://www.onvif.org/onvif/ver20/util/operationIndex.html>`_.
+ONVIFCamera has support methods to create new services::
+
+    # Create ptz service
+    ptz_service = mycam.create_ptz_service()
+    # Get ptz configuration
+    await mycam.ptz.GetConfiguration()
+    # Another way
+    # await ptz_service.GetConfiguration()
+
+Or create an unofficial service::
+
+    xaddr = 'http://192.168.0.3:8888/onvif/yourservice'
+    yourservice = mycam.create_onvif_service('service.wsdl', xaddr, 'yourservice')
+    await yourservice.SomeOperation()
+    # Another way
+    # await mycam.yourservice.SomeOperation()
+
+ONVIF CLI
+---------
+python-onvif also provides a command line interactive interface: onvif-cli.
+onvif-cli is installed automatically.
+
+Single command example
+~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    $ onvif-cli devicemgmt GetHostname --user 'admin' --password '12345' --host '192.168.0.112' --port 80
+    True: {'FromDHCP': True, 'Name': hision}
+    $ onvif-cli devicemgmt SetHostname "{'Name': 'NewerHostname'}" --user 'admin' --password '12345' --host '192.168.0.112' --port 80
+    True: {}
+
+Interactive mode
+~~~~~~~~~~~~~~~~
+
+::
+
+    $ onvif-cli -u 'admin' -a '12345' --host '192.168.0.112' --port 80 --wsdl /etc/onvif/wsdl/
+    ONVIF >>> cmd
+    analytics   devicemgmt  events      imaging     media       ptz
+    ONVIF >>> cmd devicemgmt GetWsdlUrl
+    True: http://www.onvif.org/
+    ONVIF >>> cmd devicemgmt SetHostname {'Name': 'NewHostname'}
+    ONVIF >>> cmd devicemgmt GetHostname
+    True: {'Name': 'NewHostName'}
+    ONVIF >>> cmd devicemgmt SomeOperation
+    False: No Operation: SomeOperation
+
+NOTE: Tab completion is supported for interactive mode.
+
+Batch mode
+~~~~~~~~~~
+
+::
+
+    $ vim batchcmds
+    $ cat batchcmds
+    cmd devicemgmt GetWsdlUrl
+    cmd devicemgmt SetHostname {'Name': 'NewHostname', 'FromDHCP': True}
+    cmd devicemgmt GetHostname
+    $ onvif-cli --host 192.168.0.112 -u admin -a 12345 -w /etc/onvif/wsdl/ < batchcmds
+    ONVIF >>> True: http://www.onvif.org/
+    ONVIF >>> True: {}
+    ONVIF >>> True: {'FromDHCP': False, 'Name': NewHostname}
+
+References
+----------
+
+* `ONVIF Offical Website <http://www.onvif.com>`_
+
+* `Operations Index <http://www.onvif.org/onvif/ver20/util/operationIndex.html>`_
+
+* `ONVIF Develop Documents <http://www.onvif.org/specs/DocMap-2.4.2.html>`_
+
+* `Foscam Python Lib <http://github.com/quatanium/foscam-python-lib>`_
```

### Comparing `onvif-zeep-async-1.2.4/README.rst` & `onvif-zeep-async-1.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: onvif-zeep-async
+Version: 1.2.5
+Summary: Async Python Client for ONVIF Camera
+Home-page: http://github.com/hunterjm/python-onvif-zeep-async
+Author: Cherish Chen
+Author-email: sinchb128@gmail.com
+Maintainer: sinchb
+Maintainer-email: sinchb128@gmail.com
+License: MIT
+Keywords: ONVIF,Camera,IPC
+Requires-Python: >=3
+License-File: LICENSE
+
 python-onvif-zeep-async
 =======================
 
 ONVIF Client Implementation in Python 3
 
 Dependencies
 ------------
```

### Comparing `onvif-zeep-async-1.2.4/onvif/__init__.py` & `onvif-zeep-async-1.2.5/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/client.py` & `onvif-zeep-async-1.2.5/onvif/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,15 +142,14 @@
     @safe_func
     def __init__(
         self,
         xaddr: str,
         user,
         passwd,
         url,
-        client: AsyncClient,
         encrypt=True,
         no_cache=False,
         dt_diff=None,
         binding_name="",
         binding_key="",
     ):
         if not _path_isfile(url):
@@ -159,19 +158,24 @@
         self.url = url
         self.xaddr = xaddr
         self.binding_key = binding_key
         wsse = UsernameDigestTokenDtDiff(
             user, passwd, dt_diff=dt_diff, use_digest=encrypt
         )
         # Create soap client
+        client = AsyncClient(verify=_NO_VERIFY_SSL_CONTEXT, timeout=90)
+        # The wsdl client should never actually be used, but it is required
+        # to avoid creating another ssl context since the underlying code
+        # will try to create a new one if it doesn't exist.
+        wsdl_client = httpx.Client(verify=_NO_VERIFY_SSL_CONTEXT, timeout=90)
         self.transport = (
-            AsyncTransport(client=client, verify_ssl=_NO_VERIFY_SSL_CONTEXT)
+            AsyncTransport(client=client, wsdl_client=wsdl_client)
             if no_cache
             else AsyncTransport(
-                client=client, verify_ssl=_NO_VERIFY_SSL_CONTEXT, cache=SqliteCache()
+                client=client, wsdl_client=wsdl_client, cache=SqliteCache()
             )
         )
         settings = Settings()
         settings.strict = False
         settings.xml_huge_tree = True
         self.zeep_client_authless = ZeepAsyncClient(
             wsdl=url,
@@ -205,15 +209,15 @@
             list(available_ns.keys())[list(available_ns.values()).index(namespace)]
             or "ns0"
         )
         self.create_type = lambda x: self.zeep_client.get_element(active_ns + ":" + x)()
 
     async def close(self):
         """Close the transport."""
-        # The client is not closed, as it is shared with the camera
+        await self.transport.aclose()
 
     @staticmethod
     @safe_func
     def to_dict(zeepobject):
         """Convert a WSDL Type instance into a dictionary."""
         return {} if zeepobject is None else zeep.helpers.serialize_object(zeepobject)
 
@@ -302,15 +306,15 @@
         # Active service client container
         self.services: Dict[Tuple[str, Optional[str]], ONVIFService] = {}
 
         self.to_dict = ONVIFService.to_dict
 
         self._snapshot_uris = {}
         self._snapshot_client = AsyncClient(verify=_NO_VERIFY_SSL_CONTEXT)
-        self._service_client = AsyncClient(verify=_NO_VERIFY_SSL_CONTEXT, timeout=90)
+        self._background_tasks = set()
 
     async def update_xaddrs(self):
         """Update xaddrs for services."""
         self.dt_diff = None
         devicemgmt = self.create_devicemgmt_service()
         if self.adjust_time:
             try:
@@ -356,15 +360,16 @@
         except Fault:
             return False
         return True
 
     async def close(self):
         """Close all transports."""
         await self._snapshot_client.aclose()
-        await self._service_client.aclose()
+        for service in self.services.values():
+            await service.close()
 
     async def get_snapshot_uri(self, profile_token):
         """Get the snapshot uri for a given profile."""
         uri = self._snapshot_uris.get(profile_token)
         if uri is None:
             media_service = self.create_media_service()
             req = media_service.create_type("GetSnapshotUri")
@@ -445,24 +450,34 @@
 
         xaddr, wsdl_file, binding_name = self.get_definition(name, port_type)
 
         existing_service = self.services.get(binding_key)
         if existing_service:
             if existing_service.xaddr == xaddr:
                 return existing_service
+            else:
+                # Close the existing service since it's no longer valid.
+                # This can happen when a new PullPointSubscription is created.
+                logger.debug(
+                    "Closing service %s with %s", binding_key, existing_service.xaddr
+                )
+                # Hold a reference to the task so it doesn't get
+                # garbage collected before it completes.
+                task = asyncio.create_task(existing_service.close())
+                task.add_done_callback(self._background_tasks.remove)
+                self._background_tasks.add(task)
             self.services.pop(binding_key)
 
         logger.debug("Creating service %s with %s", binding_key, xaddr)
 
         service = ONVIFService(
             xaddr,
             self.user,
             self.passwd,
             wsdl_file,
-            self._service_client,
             self.encrypt,
             no_cache=self.no_cache,
             dt_diff=self.dt_diff,
             binding_name=binding_name,
             binding_key=binding_key,
         )
```

### Comparing `onvif-zeep-async-1.2.4/onvif/definition.py` & `onvif-zeep-async-1.2.5/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/exceptions.py` & `onvif-zeep-async-1.2.5/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/addressing` & `onvif-zeep-async-1.2.5/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-1.2.5/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-1.2.5/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/display.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/envelope` & `onvif-zeep-async-1.2.5/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/events.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/media.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-1.2.5/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-1.2.5/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/search.wsdl` & `onvif-zeep-async-1.2.5/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-1.2.5/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/types.xsd` & `onvif-zeep-async-1.2.5/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-1.2.5/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-1.2.5/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/xml.xsd` & `onvif-zeep-async-1.2.5/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif/wsdl/xmlmime` & `onvif-zeep-async-1.2.5/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 1.2.4
+Version: 1.2.5
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
-Description: python-onvif-zeep-async
-        =======================
-        
-        ONVIF Client Implementation in Python 3
-        
-        Dependencies
-        ------------
-        `zeep[async] <http://docs.python-zeep.org>`_ >= 4.1.0, < 5.0.0
-        `httpx <https://www.python-httpx.org/>`_ >= 0.19.0, < 1.0.0
-        
-        Install python-onvif-zeep-async
-        -------------------------------
-        **From Source**
-        
-        You should clone this repository and run setup.py::
-        
-            cd python-onvif-zeep-async && python setup.py install
-        
-        Alternatively, you can run::
-        
-            pip install --upgrade onvif-zeep-async
-        
-        
-        Getting Started
-        ---------------
-        
-        Initialize an ONVIFCamera instance
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            from onvif import ONVIFCamera
-            mycam = ONVIFCamera('192.168.0.2', 80, 'user', 'passwd', '/etc/onvif/wsdl/')
-            await mycam.update_xaddrs()
-        
-        Now, an ONVIFCamera instance is available. By default, a devicemgmt service is also available if everything is OK.
-        
-        So, all operations defined in the WSDL document::
-        
-        /etc/onvif/wsdl/devicemgmt.wsdl
-        
-        are available.
-        
-        Get information from your camera
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        ::
-        
-            # Get Hostname
-            resp = await mycam.devicemgmt.GetHostname()
-            print 'My camera`s hostname: ' + str(resp.Name)
-        
-            # Get system date and time
-            dt = await mycam.devicemgmt.GetSystemDateAndTime()
-            tz = dt.TimeZone
-            year = dt.UTCDateTime.Date.Year
-            hour = dt.UTCDateTime.Time.Hour
-        
-        Configure (Control) your camera
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To configure your camera, there are two ways to pass parameters to service methods.
-        
-        **Dict**
-        
-        This is the simpler way::
-        
-            params = {'Name': 'NewHostName'}
-            await device_service.SetHostname(params)
-        
-        **Type Instance**
-        
-        This is the recommended way. Type instance will raise an
-        exception if you set an invalid (or non-existent) parameter.
-        
-        ::
-        
-            params = mycam.devicemgmt.create_type('SetHostname')
-            params.Hostname = 'NewHostName'
-            await mycam.devicemgmt.SetHostname(params)
-        
-            time_params = mycam.devicemgmt.create_type('SetSystemDateAndTime')
-            time_params.DateTimeType = 'Manual'
-            time_params.DaylightSavings = True
-            time_params.TimeZone.TZ = 'CST-8:00:00'
-            time_params.UTCDateTime.Date.Year = 2014
-            time_params.UTCDateTime.Date.Month = 12
-            time_params.UTCDateTime.Date.Day = 3
-            time_params.UTCDateTime.Time.Hour = 9
-            time_params.UTCDateTime.Time.Minute = 36
-            time_params.UTCDateTime.Time.Second = 11
-            await mycam.devicemgmt.SetSystemDateAndTime(time_params)
-        
-        Use other services
-        ~~~~~~~~~~~~~~~~~~
-        ONVIF protocol has defined many services.
-        You can find all the services and operations `here <http://www.onvif.org/onvif/ver20/util/operationIndex.html>`_.
-        ONVIFCamera has support methods to create new services::
-        
-            # Create ptz service
-            ptz_service = mycam.create_ptz_service()
-            # Get ptz configuration
-            await mycam.ptz.GetConfiguration()
-            # Another way
-            # await ptz_service.GetConfiguration()
-        
-        Or create an unofficial service::
-        
-            xaddr = 'http://192.168.0.3:8888/onvif/yourservice'
-            yourservice = mycam.create_onvif_service('service.wsdl', xaddr, 'yourservice')
-            await yourservice.SomeOperation()
-            # Another way
-            # await mycam.yourservice.SomeOperation()
-        
-        ONVIF CLI
-        ---------
-        python-onvif also provides a command line interactive interface: onvif-cli.
-        onvif-cli is installed automatically.
-        
-        Single command example
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            $ onvif-cli devicemgmt GetHostname --user 'admin' --password '12345' --host '192.168.0.112' --port 80
-            True: {'FromDHCP': True, 'Name': hision}
-            $ onvif-cli devicemgmt SetHostname "{'Name': 'NewerHostname'}" --user 'admin' --password '12345' --host '192.168.0.112' --port 80
-            True: {}
-        
-        Interactive mode
-        ~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            $ onvif-cli -u 'admin' -a '12345' --host '192.168.0.112' --port 80 --wsdl /etc/onvif/wsdl/
-            ONVIF >>> cmd
-            analytics   devicemgmt  events      imaging     media       ptz
-            ONVIF >>> cmd devicemgmt GetWsdlUrl
-            True: http://www.onvif.org/
-            ONVIF >>> cmd devicemgmt SetHostname {'Name': 'NewHostname'}
-            ONVIF >>> cmd devicemgmt GetHostname
-            True: {'Name': 'NewHostName'}
-            ONVIF >>> cmd devicemgmt SomeOperation
-            False: No Operation: SomeOperation
-        
-        NOTE: Tab completion is supported for interactive mode.
-        
-        Batch mode
-        ~~~~~~~~~~
-        
-        ::
-        
-            $ vim batchcmds
-            $ cat batchcmds
-            cmd devicemgmt GetWsdlUrl
-            cmd devicemgmt SetHostname {'Name': 'NewHostname', 'FromDHCP': True}
-            cmd devicemgmt GetHostname
-            $ onvif-cli --host 192.168.0.112 -u admin -a 12345 -w /etc/onvif/wsdl/ < batchcmds
-            ONVIF >>> True: http://www.onvif.org/
-            ONVIF >>> True: {}
-            ONVIF >>> True: {'FromDHCP': False, 'Name': NewHostname}
-        
-        References
-        ----------
-        
-        * `ONVIF Offical Website <http://www.onvif.com>`_
-        
-        * `Operations Index <http://www.onvif.org/onvif/ver20/util/operationIndex.html>`_
-        
-        * `ONVIF Develop Documents <http://www.onvif.org/specs/DocMap-2.4.2.html>`_
-        
-        * `Foscam Python Lib <http://github.com/quatanium/foscam-python-lib>`_
-        
 Keywords: ONVIF,Camera,IPC
-Platform: UNKNOWN
 Requires-Python: >=3
+License-File: LICENSE
+
+python-onvif-zeep-async
+=======================
+
+ONVIF Client Implementation in Python 3
+
+Dependencies
+------------
+`zeep[async] <http://docs.python-zeep.org>`_ >= 4.1.0, < 5.0.0
+`httpx <https://www.python-httpx.org/>`_ >= 0.19.0, < 1.0.0
+
+Install python-onvif-zeep-async
+-------------------------------
+**From Source**
+
+You should clone this repository and run setup.py::
+
+    cd python-onvif-zeep-async && python setup.py install
+
+Alternatively, you can run::
+
+    pip install --upgrade onvif-zeep-async
+
+
+Getting Started
+---------------
+
+Initialize an ONVIFCamera instance
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    from onvif import ONVIFCamera
+    mycam = ONVIFCamera('192.168.0.2', 80, 'user', 'passwd', '/etc/onvif/wsdl/')
+    await mycam.update_xaddrs()
+
+Now, an ONVIFCamera instance is available. By default, a devicemgmt service is also available if everything is OK.
+
+So, all operations defined in the WSDL document::
+
+/etc/onvif/wsdl/devicemgmt.wsdl
+
+are available.
+
+Get information from your camera
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+::
+
+    # Get Hostname
+    resp = await mycam.devicemgmt.GetHostname()
+    print 'My camera`s hostname: ' + str(resp.Name)
+
+    # Get system date and time
+    dt = await mycam.devicemgmt.GetSystemDateAndTime()
+    tz = dt.TimeZone
+    year = dt.UTCDateTime.Date.Year
+    hour = dt.UTCDateTime.Time.Hour
+
+Configure (Control) your camera
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To configure your camera, there are two ways to pass parameters to service methods.
+
+**Dict**
+
+This is the simpler way::
+
+    params = {'Name': 'NewHostName'}
+    await device_service.SetHostname(params)
+
+**Type Instance**
+
+This is the recommended way. Type instance will raise an
+exception if you set an invalid (or non-existent) parameter.
+
+::
+
+    params = mycam.devicemgmt.create_type('SetHostname')
+    params.Hostname = 'NewHostName'
+    await mycam.devicemgmt.SetHostname(params)
+
+    time_params = mycam.devicemgmt.create_type('SetSystemDateAndTime')
+    time_params.DateTimeType = 'Manual'
+    time_params.DaylightSavings = True
+    time_params.TimeZone.TZ = 'CST-8:00:00'
+    time_params.UTCDateTime.Date.Year = 2014
+    time_params.UTCDateTime.Date.Month = 12
+    time_params.UTCDateTime.Date.Day = 3
+    time_params.UTCDateTime.Time.Hour = 9
+    time_params.UTCDateTime.Time.Minute = 36
+    time_params.UTCDateTime.Time.Second = 11
+    await mycam.devicemgmt.SetSystemDateAndTime(time_params)
+
+Use other services
+~~~~~~~~~~~~~~~~~~
+ONVIF protocol has defined many services.
+You can find all the services and operations `here <http://www.onvif.org/onvif/ver20/util/operationIndex.html>`_.
+ONVIFCamera has support methods to create new services::
+
+    # Create ptz service
+    ptz_service = mycam.create_ptz_service()
+    # Get ptz configuration
+    await mycam.ptz.GetConfiguration()
+    # Another way
+    # await ptz_service.GetConfiguration()
+
+Or create an unofficial service::
+
+    xaddr = 'http://192.168.0.3:8888/onvif/yourservice'
+    yourservice = mycam.create_onvif_service('service.wsdl', xaddr, 'yourservice')
+    await yourservice.SomeOperation()
+    # Another way
+    # await mycam.yourservice.SomeOperation()
+
+ONVIF CLI
+---------
+python-onvif also provides a command line interactive interface: onvif-cli.
+onvif-cli is installed automatically.
+
+Single command example
+~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    $ onvif-cli devicemgmt GetHostname --user 'admin' --password '12345' --host '192.168.0.112' --port 80
+    True: {'FromDHCP': True, 'Name': hision}
+    $ onvif-cli devicemgmt SetHostname "{'Name': 'NewerHostname'}" --user 'admin' --password '12345' --host '192.168.0.112' --port 80
+    True: {}
+
+Interactive mode
+~~~~~~~~~~~~~~~~
+
+::
+
+    $ onvif-cli -u 'admin' -a '12345' --host '192.168.0.112' --port 80 --wsdl /etc/onvif/wsdl/
+    ONVIF >>> cmd
+    analytics   devicemgmt  events      imaging     media       ptz
+    ONVIF >>> cmd devicemgmt GetWsdlUrl
+    True: http://www.onvif.org/
+    ONVIF >>> cmd devicemgmt SetHostname {'Name': 'NewHostname'}
+    ONVIF >>> cmd devicemgmt GetHostname
+    True: {'Name': 'NewHostName'}
+    ONVIF >>> cmd devicemgmt SomeOperation
+    False: No Operation: SomeOperation
+
+NOTE: Tab completion is supported for interactive mode.
+
+Batch mode
+~~~~~~~~~~
+
+::
+
+    $ vim batchcmds
+    $ cat batchcmds
+    cmd devicemgmt GetWsdlUrl
+    cmd devicemgmt SetHostname {'Name': 'NewHostname', 'FromDHCP': True}
+    cmd devicemgmt GetHostname
+    $ onvif-cli --host 192.168.0.112 -u admin -a 12345 -w /etc/onvif/wsdl/ < batchcmds
+    ONVIF >>> True: http://www.onvif.org/
+    ONVIF >>> True: {}
+    ONVIF >>> True: {'FromDHCP': False, 'Name': NewHostname}
+
+References
+----------
+
+* `ONVIF Offical Website <http://www.onvif.com>`_
+
+* `Operations Index <http://www.onvif.org/onvif/ver20/util/operationIndex.html>`_
+
+* `ONVIF Develop Documents <http://www.onvif.org/specs/DocMap-2.4.2.html>`_
+
+* `Foscam Python Lib <http://github.com/quatanium/foscam-python-lib>`_
```

### Comparing `onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-1.2.5/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+.gitignore
+.pre-commit-config.yaml
 CHANGES.txt
 LICENSE
 MANIFEST.in
+Makefile
 README.rst
+bandit.yaml
+pylintrc
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
+examples/events.py
+examples/rotate_image.py
+examples/streaming.py
 onvif/__init__.py
 onvif/client.py
 onvif/definition.py
 onvif/exceptions.py
 onvif/version.txt
 onvif/wsdl/__init__.py
 onvif/wsdl/accesscontrol.wsdl
@@ -46,8 +55,9 @@
 onvif/wsdl/xmlmime
 onvif_zeep_async.egg-info/PKG-INFO
 onvif_zeep_async.egg-info/SOURCES.txt
 onvif_zeep_async.egg-info/dependency_links.txt
 onvif_zeep_async.egg-info/entry_points.txt
 onvif_zeep_async.egg-info/not-zip-safe
 onvif_zeep_async.egg-info/requires.txt
-onvif_zeep_async.egg-info/top_level.txt
+onvif_zeep_async.egg-info/top_level.txt
+tests/test.py
```

### Comparing `onvif-zeep-async-1.2.4/setup.py` & `onvif-zeep-async-1.2.5/setup.py`

 * *Files identical despite different names*

