# Comparing `tmp/onvif-zeep-async-1.2.3.tar.gz` & `tmp/onvif-zeep-async-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-1.2.3.tar", last modified: Tue Mar 28 22:58:25 2023, max compression
+gzip compressed data, was "onvif-zeep-async-1.2.4.tar", last modified: Thu Apr 13 23:24:59 2023, max compression
```

## Comparing `onvif-zeep-async-1.2.3.tar` & `onvif-zeep-async-1.2.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-28 22:58:25.723210 onvif-zeep-async-1.2.3/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/CHANGES.txt
--rw-r--r--   0 jason     (1000) jason     (1000)     1087 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)      100 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/MANIFEST.in
--rw-rw-r--   0 jason     (1000) jason     (1000)     6667 2023-03-28 22:58:25.723210 onvif-zeep-async-1.2.3/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)     4926 2021-08-27 21:44:54.000000 onvif-zeep-async-1.2.3/README.rst
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-28 22:58:25.711210 onvif-zeep-async-1.2.3/onvif/
--rw-rw-r--   0 jason     (1000) jason     (1000)      599 2020-10-18 04:42:45.000000 onvif-zeep-async-1.2.3/onvif/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)    18182 2023-03-28 22:53:30.000000 onvif-zeep-async-1.2.3/onvif/client.py
--rw-r--r--   0 jason     (1000) jason     (1000)     2190 2020-05-18 19:22:35.000000 onvif-zeep-async-1.2.3/onvif/definition.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      886 2020-10-18 04:42:45.000000 onvif-zeep-async-1.2.3/onvif/exceptions.py
--rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-03-28 22:56:56.000000 onvif-zeep-async-1.2.3/onvif/version.txt
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-28 22:58:25.723210 onvif-zeep-async-1.2.3/onvif/wsdl/
--rw-r--r--   0 jason     (1000) jason     (1000)       26 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)    38072 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    57255 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     7263 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/addressing
--rw-r--r--   0 jason     (1000) jason     (1000)    79284 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    24131 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    31976 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    23300 2020-05-07 15:00:34.000000 onvif-zeep-async-1.2.3/onvif/wsdl/b-2.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     5100 2020-05-07 04:46:04.000000 onvif-zeep-async-1.2.3/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)    20498 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    60231 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)   163209 2020-05-07 14:59:35.000000 onvif-zeep-async-1.2.3/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    24593 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/display.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    53648 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     6249 2020-05-07 14:59:35.000000 onvif-zeep-async-1.2.3/onvif/wsdl/envelope
--rw-r--r--   0 jason     (1000) jason     (1000)    37870 2020-05-18 19:48:12.000000 onvif-zeep-async-1.2.3/onvif/wsdl/events.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    17998 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)      511 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/include
--rw-r--r--   0 jason     (1000) jason     (1000)   174812 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/media.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)   363349 2020-05-07 14:59:35.000000 onvif-zeep-async-1.2.3/onvif/wsdl/onvif.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)    54058 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     3660 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/r-2.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)    17214 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    40704 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/recording.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     5596 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    10581 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/replay.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     3727 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)    43139 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/search.wsdl
--rw-r--r--   0 jason     (1000) jason     (1000)     8960 2020-05-07 04:45:04.000000 onvif-zeep-async-1.2.3/onvif/wsdl/t-1.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     3738 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/types.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     5849 2020-05-07 04:44:07.000000 onvif-zeep-async-1.2.3/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)    10455 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     8836 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/xml.xsd
--rw-r--r--   0 jason     (1000) jason     (1000)     1639 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.3/onvif/wsdl/xmlmime
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-03-28 22:58:25.723210 onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/
--rw-rw-r--   0 jason     (1000) jason     (1000)     6667 2023-03-28 22:58:25.000000 onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)     1255 2023-03-28 22:58:25.000000 onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/SOURCES.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-03-28 22:58:25.000000 onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/dependency_links.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)       46 2023-03-28 22:58:25.000000 onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/entry_points.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-03-28 22:58:25.000000 onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/not-zip-safe
--rw-rw-r--   0 jason     (1000) jason     (1000)       47 2023-03-28 22:58:25.000000 onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/requires.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-03-28 22:58:25.000000 onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/top_level.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)       77 2020-10-18 04:42:45.000000 onvif-zeep-async-1.2.3/pyproject.toml
--rw-rw-r--   0 jason     (1000) jason     (1000)      409 2023-03-28 22:58:25.723210 onvif-zeep-async-1.2.3/setup.cfg
--rw-rw-r--   0 jason     (1000) jason     (1000)     1801 2021-08-27 21:44:54.000000 onvif-zeep-async-1.2.3/setup.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/CHANGES.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)     1087 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/LICENSE
+-rw-r--r--   0 jason     (1000) jason     (1000)      100 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/MANIFEST.in
+-rw-rw-r--   0 jason     (1000) jason     (1000)     6667 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4926 2021-08-27 21:44:54.000000 onvif-zeep-async-1.2.4/README.rst
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-13 23:24:59.953377 onvif-zeep-async-1.2.4/onvif/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      599 2020-10-18 04:42:45.000000 onvif-zeep-async-1.2.4/onvif/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)    18227 2023-04-13 23:24:18.000000 onvif-zeep-async-1.2.4/onvif/client.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     2190 2020-05-18 19:22:35.000000 onvif-zeep-async-1.2.4/onvif/definition.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      886 2020-10-18 04:42:45.000000 onvif-zeep-async-1.2.4/onvif/exceptions.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-04-13 23:24:33.000000 onvif-zeep-async-1.2.4/onvif/version.txt
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/onvif/wsdl/
+-rw-r--r--   0 jason     (1000) jason     (1000)       26 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)    38072 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    57255 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)     7263 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/addressing
+-rw-r--r--   0 jason     (1000) jason     (1000)    79284 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    24131 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    31976 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    23300 2020-05-07 15:00:34.000000 onvif-zeep-async-1.2.4/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 jason     (1000) jason     (1000)     5100 2020-05-07 04:46:04.000000 onvif-zeep-async-1.2.4/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 jason     (1000) jason     (1000)    20498 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    60231 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)   163209 2020-05-07 14:59:35.000000 onvif-zeep-async-1.2.4/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    24593 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/display.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    53648 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)     6249 2020-05-07 14:59:35.000000 onvif-zeep-async-1.2.4/onvif/wsdl/envelope
+-rw-r--r--   0 jason     (1000) jason     (1000)    37870 2020-05-18 19:48:12.000000 onvif-zeep-async-1.2.4/onvif/wsdl/events.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    17998 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)      511 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/include
+-rw-r--r--   0 jason     (1000) jason     (1000)   174812 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/media.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)   363349 2020-05-07 14:59:35.000000 onvif-zeep-async-1.2.4/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 jason     (1000) jason     (1000)    54058 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)     3660 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 jason     (1000) jason     (1000)    17214 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    40704 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)     5596 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    10581 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)     3727 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)    43139 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/search.wsdl
+-rw-r--r--   0 jason     (1000) jason     (1000)     8960 2020-05-07 04:45:04.000000 onvif-zeep-async-1.2.4/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 jason     (1000) jason     (1000)     3738 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/types.xsd
+-rw-r--r--   0 jason     (1000) jason     (1000)     5849 2020-05-07 04:44:07.000000 onvif-zeep-async-1.2.4/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 jason     (1000) jason     (1000)    10455 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 jason     (1000) jason     (1000)     8836 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/xml.xsd
+-rw-r--r--   0 jason     (1000) jason     (1000)     1639 2020-05-06 02:42:46.000000 onvif-zeep-async-1.2.4/onvif/wsdl/xmlmime
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     6667 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1255 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)       46 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/entry_points.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/not-zip-safe
+-rw-rw-r--   0 jason     (1000) jason     (1000)       47 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/requires.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-04-13 23:24:59.000000 onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/top_level.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)       77 2020-10-18 04:42:45.000000 onvif-zeep-async-1.2.4/pyproject.toml
+-rw-rw-r--   0 jason     (1000) jason     (1000)      409 2023-04-13 23:24:59.965377 onvif-zeep-async-1.2.4/setup.cfg
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1801 2021-08-27 21:44:54.000000 onvif-zeep-async-1.2.4/setup.py
```

### Comparing `onvif-zeep-async-1.2.3/LICENSE` & `onvif-zeep-async-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/PKG-INFO` & `onvif-zeep-async-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: onvif-zeep-async
-Version: 1.2.3
+Version: 1.2.4
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.2.3/README.rst` & `onvif-zeep-async-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/__init__.py` & `onvif-zeep-async-1.2.4/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/client.py` & `onvif-zeep-async-1.2.4/onvif/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,22 +26,23 @@
 logging.basicConfig(level=logging.INFO)
 logging.getLogger("zeep.client").setLevel(logging.CRITICAL)
 
 
 def create_no_verify_ssl_context() -> ssl.SSLContext:
     """Return an SSL context that does not verify the server certificate.
     This is a copy of aiohttp's create_default_context() function, with the
-    ssl verify turned off.
+    ssl verify turned off and old SSL versions enabled.
+
     https://github.com/aio-libs/aiohttp/blob/33953f110e97eecc707e1402daa8d543f38a189b/aiohttp/connector.py#L911
     """
     sslcontext = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-    sslcontext.options |= ssl.OP_NO_SSLv2
-    sslcontext.options |= ssl.OP_NO_SSLv3
     sslcontext.check_hostname = False
     sslcontext.verify_mode = ssl.CERT_NONE
+    # Allow all ciphers rather than only Python 3.10 default
+    sslcontext.set_ciphers("DEFAULT")
     with contextlib.suppress(AttributeError):
         # This only works for OpenSSL >= 1.0.0
         sslcontext.options |= ssl.OP_NO_COMPRESSION
     sslcontext.set_default_verify_paths()
     return sslcontext
```

### Comparing `onvif-zeep-async-1.2.3/onvif/definition.py` & `onvif-zeep-async-1.2.4/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/exceptions.py` & `onvif-zeep-async-1.2.4/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/addressing` & `onvif-zeep-async-1.2.4/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-1.2.4/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-1.2.4/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/display.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/envelope` & `onvif-zeep-async-1.2.4/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/events.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/media.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-1.2.4/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-1.2.4/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/search.wsdl` & `onvif-zeep-async-1.2.4/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-1.2.4/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/types.xsd` & `onvif-zeep-async-1.2.4/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-1.2.4/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-1.2.4/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/xml.xsd` & `onvif-zeep-async-1.2.4/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif/wsdl/xmlmime` & `onvif-zeep-async-1.2.4/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: onvif-zeep-async
-Version: 1.2.3
+Version: 1.2.4
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.2.3/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-1.2.4/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.3/setup.py` & `onvif-zeep-async-1.2.4/setup.py`

 * *Files identical despite different names*

