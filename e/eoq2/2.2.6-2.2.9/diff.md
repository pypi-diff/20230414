# Comparing `tmp/eoq2-2.2.6.tar.gz` & `tmp/eoq2-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eoq2-2.2.6.tar", last modified: Tue May 25 12:18:44 2021, max compression
+gzip compressed data, was "eoq2-2.2.9.tar", last modified: Wed Aug 18 07:59:15 2021, max compression
```

## Comparing `eoq2-2.2.6.tar` & `eoq2-2.2.9.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.722209 eoq2-2.2.6/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      505 2021-05-25 12:18:44.721209 eoq2-2.2.6/PKG-INFO
--rw-rw-r--   0 bastian   (1000) bastian   (1000)        0 2020-05-13 09:52:07.000000 eoq2-2.2.6/README.md
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.691209 eoq2-2.2.6/eoq2/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      116 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/__init__.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.694209 eoq2-2.2.6/eoq2/action/
--rw-r--r--   0 bastian   (1000) bastian   (1000)      142 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/action/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      856 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/action/action.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2958 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/action/call.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      754 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/action/callhandler.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1030 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/action/callmanager.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     8169 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/action/cmdrunnerbasedcallmanager.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.695209 eoq2-2.2.6/eoq2/action/externalpy/
--rw-r--r--   0 bastian   (1000) bastian   (1000)       40 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/action/externalpy/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)    24055 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/action/externalpy/externalpyscripthandler.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     5080 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/action/util.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.696209 eoq2-2.2.6/eoq2/command/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/command/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     8047 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/command/command.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    54352 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/command/commandrunner.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    43028 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/command/diff.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      854 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/command/result.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.698209 eoq2-2.2.6/eoq2/domain/
--rw-r--r--   0 bastian   (1000) bastian   (1000)       60 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/domain/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1583 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/domain/cmdrunnerbaseddomain.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      613 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/domain/domain.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.699209 eoq2-2.2.6/eoq2/domain/local/
--rw-r--r--   0 bastian   (1000) bastian   (1000)       31 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/domain/local/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      613 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/domain/local/localmdbdomain.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.700209 eoq2-2.2.6/eoq2/domain/multiprocessing/
--rw-r--r--   0 bastian   (1000) bastian   (1000)       86 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/domain/multiprocessing/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1089 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/domain/multiprocessing/multiprocessingcallmanager.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2668 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/domain/multiprocessing/multiprocessingdomainclient.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     3535 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/domain/multiprocessing/multiprocessingdomainhost.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.707209 eoq2-2.2.6/eoq2/event/
--rw-r--r--   0 bastian   (1000) bastian   (1000)       22 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/event/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     5500 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/event/event.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.709209 eoq2-2.2.6/eoq2/frame/
--rw-r--r--   0 bastian   (1000) bastian   (1000)      127 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/frame/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1670 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/frame/domainframehandler.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      458 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/frame/frame.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      746 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/frame/framehandler.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     2186 2021-01-14 06:26:08.000000 eoq2-2.2.6/eoq2/frame/multiversionframehandler.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.710209 eoq2-2.2.6/eoq2/legacy/
--rw-r--r--   0 bastian   (1000) bastian   (1000)       23 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/legacy/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    12199 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/legacy/legacy.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.712209 eoq2-2.2.6/eoq2/mdb/
--rw-r--r--   0 bastian   (1000) bastian   (1000)       99 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/mdb/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      429 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/mdb/mdb.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     2670 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/mdb/mdbaccessor.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      266 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/mdb/nocodec.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.714209 eoq2-2.2.6/eoq2/mdb/pyecore/
--rw-r--r--   0 bastian   (1000) bastian   (1000)      213 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/mdb/pyecore/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1697 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/mdb/pyecore/pyecoreidcodec.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     2205 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/mdb/pyecore/pyecoremdb.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    34035 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/mdb/pyecore/pyecoremdbaccessor.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      518 2021-01-19 14:05:41.000000 eoq2-2.2.6/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     5813 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    80288 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.715209 eoq2-2.2.6/eoq2/mdb/pyecore/workspacemdbmodel/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1326 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     5277 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.716209 eoq2-2.2.6/eoq2/mdb/pyecore/xmlresourcemodel/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1092 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     3591 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      175 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/mdb/valuecodec.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.716209 eoq2-2.2.6/eoq2/query/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/query/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    11815 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/query/query.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    36235 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/query/queryrunner.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.718209 eoq2-2.2.6/eoq2/serialization/
--rw-r--r--   0 bastian   (1000) bastian   (1000)      204 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/serialization/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1203 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/serialization/jsonserializer.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     6436 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/serialization/jsserializer.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     5871 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/serialization/pyserializer.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      314 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/serialization/serializer.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    31738 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/serialization/textserializer.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.721209 eoq2-2.2.6/eoq2/util/
--rw-r--r--   0 bastian   (1000) bastian   (1000)      118 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/util/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     2491 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/util/backup.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    13851 2020-05-13 09:55:15.000000 eoq2-2.2.6/eoq2/util/csvconnector.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1272 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/util/error.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     4511 2021-05-25 12:18:14.000000 eoq2-2.2.6/eoq2/util/logger.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2634 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/util/model.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     4037 2020-10-25 08:49:21.000000 eoq2-2.2.6/eoq2/util/util.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-05-25 12:18:44.691209 eoq2-2.2.6/eoq2.egg-info/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      505 2021-05-25 12:18:44.000000 eoq2-2.2.6/eoq2.egg-info/PKG-INFO
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     2133 2021-05-25 12:18:44.000000 eoq2-2.2.6/eoq2.egg-info/SOURCES.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)        1 2021-05-25 12:18:44.000000 eoq2-2.2.6/eoq2.egg-info/dependency_links.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)        5 2021-05-25 12:18:44.000000 eoq2-2.2.6/eoq2.egg-info/top_level.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       38 2021-05-25 12:18:44.722209 eoq2-2.2.6/setup.cfg
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      710 2020-05-13 13:00:29.000000 eoq2-2.2.6/setup.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.477278 eoq2-2.2.9/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      505 2021-08-18 07:59:15.476278 eoq2-2.2.9/PKG-INFO
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)        0 2020-05-13 09:52:07.000000 eoq2-2.2.9/README.md
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.467278 eoq2-2.2.9/eoq2/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      116 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/__init__.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.468278 eoq2-2.2.9/eoq2/action/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      142 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/action/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      856 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/action/action.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2958 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/action/call.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      754 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/action/callhandler.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1030 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/action/callmanager.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     8117 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/action/cmdrunnerbasedcallmanager.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.469278 eoq2-2.2.9/eoq2/action/externalpy/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       40 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/action/externalpy/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)    24055 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/action/externalpy/externalpyscripthandler.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     5080 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/action/util.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.469278 eoq2-2.2.9/eoq2/command/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/command/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     8312 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/command/command.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    55066 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/command/commandrunner.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    43028 2021-05-25 12:18:14.000000 eoq2-2.2.9/eoq2/command/diff.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      854 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/command/result.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.470278 eoq2-2.2.9/eoq2/domain/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       60 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/domain/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     2055 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/domain/cmdrunnerbaseddomain.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      698 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/domain/domain.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.470278 eoq2-2.2.9/eoq2/domain/local/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       31 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/domain/local/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      699 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/domain/local/localmdbdomain.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.471278 eoq2-2.2.9/eoq2/domain/multiprocessing/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       86 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/domain/multiprocessing/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1089 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/domain/multiprocessing/multiprocessingcallmanager.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2668 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/domain/multiprocessing/multiprocessingdomainclient.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     3535 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/domain/multiprocessing/multiprocessingdomainhost.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.471278 eoq2-2.2.9/eoq2/event/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       22 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/event/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     5500 2021-05-25 12:18:14.000000 eoq2-2.2.9/eoq2/event/event.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.471278 eoq2-2.2.9/eoq2/frame/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      127 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/frame/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1670 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/frame/domainframehandler.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      458 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/frame/frame.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      746 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/frame/framehandler.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     2186 2021-01-14 06:26:08.000000 eoq2-2.2.9/eoq2/frame/multiversionframehandler.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.472278 eoq2-2.2.9/eoq2/legacy/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       23 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/legacy/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    12199 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/legacy/legacy.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.472278 eoq2-2.2.9/eoq2/mdb/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       99 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/mdb/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      471 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/mdb/mdb.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     2670 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/mdb/mdbaccessor.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      266 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/mdb/nocodec.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.473278 eoq2-2.2.9/eoq2/mdb/pyecore/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      213 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/mdb/pyecore/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1697 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/mdb/pyecore/pyecoreidcodec.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     2388 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/mdb/pyecore/pyecoremdb.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    34131 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/mdb/pyecore/pyecoremdbaccessor.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      518 2021-01-19 14:05:41.000000 eoq2-2.2.9/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     5811 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    80155 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.474278 eoq2-2.2.9/eoq2/mdb/pyecore/workspacemdbmodel/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1326 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     5277 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.474278 eoq2-2.2.9/eoq2/mdb/pyecore/xmlresourcemodel/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1092 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     3591 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      175 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/mdb/valuecodec.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.474278 eoq2-2.2.9/eoq2/query/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/query/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    11924 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/query/query.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    36494 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/query/queryrunner.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.475278 eoq2-2.2.9/eoq2/serialization/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      204 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/serialization/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1203 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/serialization/jsonserializer.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     6436 2021-05-25 12:18:14.000000 eoq2-2.2.9/eoq2/serialization/jsserializer.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     5871 2021-05-25 12:18:14.000000 eoq2-2.2.9/eoq2/serialization/pyserializer.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      314 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/serialization/serializer.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    35101 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/serialization/textserializer.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.476278 eoq2-2.2.9/eoq2/util/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      118 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/util/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     2491 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/util/backup.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     4033 2021-08-18 07:56:52.000000 eoq2-2.2.9/eoq2/util/benchmark.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    13851 2020-05-13 09:55:15.000000 eoq2-2.2.9/eoq2/util/csvconnector.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1272 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/util/error.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     4511 2021-05-25 12:18:14.000000 eoq2-2.2.9/eoq2/util/logger.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2634 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/util/model.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     4037 2020-10-25 08:49:21.000000 eoq2-2.2.9/eoq2/util/util.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2021-08-18 07:59:15.468278 eoq2-2.2.9/eoq2.egg-info/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      505 2021-08-18 07:59:15.000000 eoq2-2.2.9/eoq2.egg-info/PKG-INFO
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     2156 2021-08-18 07:59:15.000000 eoq2-2.2.9/eoq2.egg-info/SOURCES.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)        1 2021-08-18 07:59:15.000000 eoq2-2.2.9/eoq2.egg-info/dependency_links.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)        5 2021-08-18 07:59:15.000000 eoq2-2.2.9/eoq2.egg-info/top_level.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       38 2021-08-18 07:59:15.477278 eoq2-2.2.9/setup.cfg
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      710 2020-05-13 13:00:29.000000 eoq2-2.2.9/setup.py
```

### Comparing `eoq2-2.2.6/eoq2/action/action.py` & `eoq2-2.2.9/eoq2/action/action.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/action/call.py` & `eoq2-2.2.9/eoq2/action/call.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/action/callhandler.py` & `eoq2-2.2.9/eoq2/action/callhandler.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/action/callmanager.py` & `eoq2-2.2.9/eoq2/action/callmanager.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/action/cmdrunnerbasedcallmanager.py` & `eoq2-2.2.9/eoq2/action/cmdrunnerbasedcallmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,16 @@
  2019 Bjoern Annighoefer
 '''
 from ..action.callmanager import CallManager
 from ..action.call import CallOptions
 
 from .call import CallTypes,CallStatus,Call,CALL_STATUS_FINAL_TYPES
 from ..event import CstEvt,CvaEvt,OupEvt,ALL_EVENT_TYPES
-from ..command.command import Obs,Ubs
 from ..util import EoqError,DATE_TIME_STR_FORMAT
 
-import time
 from datetime import datetime
 
 
 '''
   CmdRunnerBaseCallManager
 '''
```

### Comparing `eoq2-2.2.6/eoq2/action/externalpy/externalpyscripthandler.py` & `eoq2-2.2.9/eoq2/action/externalpy/externalpyscripthandler.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/action/util.py` & `eoq2-2.2.9/eoq2/action/util.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/command/command.py` & `eoq2-2.2.9/eoq2/command/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,21 @@
     LOG = 'LOG' #log: LST + creates a log file (info.log) with detailed information on every object
     DET = 'DET' #detailed: LOG + creates a file with all objects and their #1234 number
 
 class Cmd:
     def __init__(self,t : str,args):
         self.cmd = t
         self.a = args
+    def __repr__(self):
+        cmdStr = str(self.cmd)
+        if(type(self.a)==list and len(self.a) > 0):
+            cmdStr += ' ' + ' '.join([str(arg) for arg in self.a])
+        elif(self.a):
+            cmdStr += ' ' + str(self.a)
+        return cmdStr
         
 class Get(Cmd):
     def __init__(self,target):
         super().__init__(CmdTypes.GET,target)
         
 class Set(Cmd):
     def __init__(self,target,feature,value):
```

### Comparing `eoq2-2.2.6/eoq2/command/commandrunner.py` & `eoq2-2.2.9/eoq2/command/commandrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from .command import CmdTypes, CloModes, MrgModes
+from .command import CmdTypes, MrgModes
 from .result import Res,ResTypes
 from .diff import DifferenceFinder
 from ..query.query import Qry,Obj,ObjSeg
 from ..query.queryrunner import QryRunner
 from ..util.error import EoqError
 from ..action import CmdRunnerBasedCallManager
 from ..event.event import EvtProvider,ChgEvt,ChgTypes,ALL_EVENT_TYPES
 from ..util.util import IsListOfObjects,IsNoList,IsList,ApplyToAllElements
 from ..util.logger import NoLogging
+from ..util.benchmark import Benchmark
 from ..serialization.jsonserializer import JsonSerializer
 
 from datetime import time
 from uuid import uuid4
 
 import traceback
-import re
+
 
 class Session:
     def __init__(self,sessionId,sessionNumber):
         self.sessionId = sessionId
         self.sessionNumber = sessionNumber
         self.user = None
         self.begin = time
@@ -36,33 +37,34 @@
         self.history = []
         self.isMuted = False
         
 '''
  Cmd Runner
 '''   
 class CmdRunner(EvtProvider):
-    def __init__(self,mdbAccessor,maxChanges=10000,logger=NoLogging()):
+    def __init__(self,mdbAccessor,maxChanges=10000,logger=NoLogging(),enableBenchmark=False):
         super().__init__()
         self.mdbAccessor = mdbAccessor
         self.maxChanges = maxChanges #the number of changes that are preserved
         #logging
         self.logger = logger
+        self.enableBenchmark = enableBenchmark
         self.logSerializer = JsonSerializer()
         #initialize internals
         self.latestTransactionId = 0
         self.sessionCount = 0
         self.transactions = {}
         #sessions
         self.sessions = {} #dict containing sessions keys and related session informations
         #changes
         self.earliestChangeId = 0
         self.latestChangeId = 0
         self.changes = {}
         #query runner
-        self.qryEvaluator = QryRunner(self.mdbAccessor)
+        self.qryEvaluator = QryRunner(self.mdbAccessor,enableBenchmark=enableBenchmark)
         self.callManager = CmdRunnerBasedCallManager(self)        
         #init command evaluators functor table
         self.cmdEvaluators = {}
         self.cmdEvaluators[CmdTypes.GET] = self.ExecGet
         self.cmdEvaluators[CmdTypes.SET] = self.ExecSet
         self.cmdEvaluators[CmdTypes.ADD] = self.ExecAdd
         self.cmdEvaluators[CmdTypes.REM] = self.ExecRem
@@ -92,14 +94,22 @@
         self.cmdEvaluators[CmdTypes.UMT] = self.ExecUmt
         
         #start listening to external events
         if(self.mdbAccessor):
             self.mdbAccessor.Observe(self.OnCallMdbAccessorEvent)
         if(self.callManager):
             self.callManager.Observe(self.OnCallManagerEvent)
+            
+        #benchmark
+        if(self.enableBenchmark):
+            self.benchmark = Benchmark()
+            allCmdTypes = [getattr(CmdTypes,k) for k in CmdTypes.__dict__ if not k.startswith('_')]
+            for t in allCmdTypes:
+                self.benchmark.InitMessure(t)
+
 
         # merge / diff
         self.oldRoot = None
         self.newRoot = None
         self.postponedMergeReferences = []
         self.diffcommands = []
         self.mDummies = 1
@@ -118,21 +128,27 @@
             self.logger.Error(errorMsg)
             traceback.print_exc()
             res = Res(cmd.cmd,ResTypes.ERR,str(e),tid,self.latestChangeId)     
         self.EndTransaction(res,tid)
         return res
     
     def ExecOnTransaction(self,cmd,tid):
-        
         self.logger.PassivatableLog('transaction',lambda : self.logSerializer.Ser(cmd))
+        cmdType = cmd.cmd
         try:
-            evaluator = self.cmdEvaluators[cmd.cmd]
+            evaluator = self.cmdEvaluators[cmdType]
         except KeyError:
             raise EoqError(0,"Error evaluating command: Unknown command type: %s."%(cmd.cmd))
-        res = evaluator(cmd.a,tid)
+        if self.enableBenchmark: self.benchmark.Start()
+        try:
+            res = evaluator(cmd.a,tid)
+        except Exception as e: 
+            if self.enableBenchmark: self.benchmark.Stop(cmdType)
+            raise e #forward exception
+        if self.enableBenchmark: self.benchmark.Stop(cmdType)
         self.logger.PassivatableLog('transaction',lambda: self.logSerializer.Ser(res))
         return res
     
     def ExecCmp(self,args,tid):
         transaction = self.GetTransaction(tid)
         status = ResTypes.OKY
         subresults = []
```

### Comparing `eoq2-2.2.6/eoq2/command/diff.py` & `eoq2-2.2.9/eoq2/command/diff.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/command/result.py` & `eoq2-2.2.9/eoq2/command/result.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/domain/cmdrunnerbaseddomain.py` & `eoq2-2.2.9/eoq2/domain/cmdrunnerbaseddomain.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from .domain import Domain
 from ..util.logger import NoLogging,LogLevels
 from ..serialization import TextSerializer
 from ..command.command import Get
 from ..event import ALL_EVENT_TYPES
 
 class CmdRunnerBasedDomain(Domain):
-    def __init__(self,cmdRunner,logger=NoLogging(),serializer=TextSerializer()):
+    def __init__(self,cmdRunner,logger=NoLogging(),serializer=TextSerializer(),enableBenchmark=False):
         super().__init__(logger)
         self.serializer = serializer
+        self.enableBenchmark = enableBenchmark
         self.doCounter = 0
         self.cmdRunner = cmdRunner
 #         if(self.cmdRunner):
 #             self.cmdRunner.Observe(self._OnCmdRunnerEvents)
         
     def RawDo(self,cmd,sessionId=None):
         self.doCounter += 1
@@ -37,8 +38,16 @@
     def Unobserve(self,callback,context=None):
         self.cmdRunner.Unobserve(callback,context)
         
     #@Override
     def NotifyObservers(self,evts,excludedCallback=None,excludedContext=None):
         self.cmdRunner.NotifyObservers(evts,excludedCallback,excludedContext)
         
+    def Close(self):
+        #benchmark:
+        if self.enableBenchmark:
+            self.cmdRunner.benchmark.SaveToFile('CmdBenchmark.csv')
+            self.logger.Info("Command benchmark saved to CmdBenchmark.csv")
+            self.cmdRunner.qryEvaluator.benchmark.SaveToFile('QryBenchmark.csv')
+            self.logger.Info("Query segment benchmark saved to QryBenchmark.csv")
+
```

### Comparing `eoq2-2.2.6/eoq2/domain/local/localmdbdomain.py` & `eoq2-2.2.9/eoq2/domain/local/localmdbdomain.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..cmdrunnerbaseddomain import CmdRunnerBasedDomain
 from ...command.commandrunner import CmdRunner
 from ...util.logger import NoLogging
 from ...serialization import TextSerializer
 
 class LocalMdbDomain(CmdRunnerBasedDomain):
-    def __init__(self,mdbAccessor,maxChanges=100,logger=NoLogging(),serializer=TextSerializer()):
+    def __init__(self,mdbAccessor,maxChanges=100,logger=NoLogging(),serializer=TextSerializer(),enableBenchmark=False):
         self.mdbAccessor = mdbAccessor
-        self.cmdRunner = CmdRunner(mdbAccessor,maxChanges=maxChanges,logger=logger)
-        super().__init__(self.cmdRunner,logger=logger,serializer=serializer)
+        self.cmdRunner = CmdRunner(mdbAccessor,maxChanges=maxChanges,logger=logger,enableBenchmark=enableBenchmark)
+        super().__init__(self.cmdRunner,logger=logger,serializer=serializer,enableBenchmark=enableBenchmark)
```

### Comparing `eoq2-2.2.6/eoq2/domain/multiprocessing/multiprocessingcallmanager.py` & `eoq2-2.2.9/eoq2/domain/multiprocessing/multiprocessingcallmanager.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/domain/multiprocessing/multiprocessingdomainclient.py` & `eoq2-2.2.9/eoq2/domain/multiprocessing/multiprocessingdomainclient.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/domain/multiprocessing/multiprocessingdomainhost.py` & `eoq2-2.2.9/eoq2/domain/multiprocessing/multiprocessingdomainhost.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/event/event.py` & `eoq2-2.2.9/eoq2/event/event.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/frame/domainframehandler.py` & `eoq2-2.2.9/eoq2/frame/domainframehandler.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/frame/framehandler.py` & `eoq2-2.2.9/eoq2/frame/framehandler.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/frame/multiversionframehandler.py` & `eoq2-2.2.9/eoq2/frame/multiversionframehandler.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/legacy/legacy.py` & `eoq2-2.2.9/eoq2/legacy/legacy.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/mdb/mdbaccessor.py` & `eoq2-2.2.9/eoq2/mdb/mdbaccessor.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/pyecoreidcodec.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/pyecoreidcodec.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/pyecoremdb.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/pyecoremdb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from ..mdb import Mdb
 
 from pyecore.ecore import EProxy,MetaEClass
 import types
 import traceback
+from threading import Lock
 
 class PyEcoreMdb(Mdb):
     def __init__(self,root,metamodelRegistry,provider=None):#must be the original meta model registry and allow for modifications
         super().__init__()
         self.root = root
         self.metamodelRegistry = metamodelRegistry
         self.provider = provider;
+        self.lock = Lock()
+        
+    def Lock(self):
+        self.lock.acquire()
+            
+    def Release(self):
+        self.lock.release()
     
     def Root(self):
         return self.root
     
     def Metamodels(self):
         return [(p.eClass if(isinstance(p,types.ModuleType)) else p) for p in self.metamodelRegistry.values()]
```

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/pyecoremdbaccessor.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/pyecoremdbaccessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 #Definition of pyecore based accessors
 from pyecore.ecore import EPackage,EObject,EClass,EProxy,MetaEClass,\
     EClassifier
 from pyecore.valuecontainer import EOrderedSet
 
 import types
 from itertools import chain
-import traceback
 
 
 class PyEcoreMdbAccessor(MdbAccessor):
     def __init__(self,mdb=None,valueCodec=None):
         super().__init__()
         self.mdb = mdb #is necessary for creating classes by name
         self.vc = valueCodec
         ##make sure the root gets the primary encoding
         self.root = self.__ResolveAndEnc(self.mdb.Root())
         
         #internal caching
         #self.allReferencesLut = {}
         
+    def Lock(self):
+        self.mdb.Lock()
+    
+    def Release(self):
+        self.mdb.Release()
+        
     ''' METAMODEL ACESSORS '''
    
     def GetAllMetamodels(self):
         ePackages = self.mdb.Metamodels()
         metamodels = [self.__ResolveAndEnc(m) for m in ePackages]
         return metamodels
```

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.valueCodec = None #is set during coupling
         self.domain = None #is set during coupling
         self.mdb = None #is created later
         
         if(autoload):
             self.Load()
             
-    def __del__(self):
+    def Close(self):
         #make sure any changes are saved
         #self.logger.Info("Closing single %s ..."%(self.modelfile)) #makes problems when main thread has ended already
         
         self.__StopDelayedSaving()
         self.__Save()
         
 #     def Root(self):
```

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,28 +16,25 @@
 from .workspacemdbmodel import Workspace,ModelResource,Directory,FileResourceTypesE,PathElementA,FileResourceA,XmlResource
 from .xmlresourcemodel import Document,Element,Attribute
 
 from pyecore.resources import ResourceSet, URI
 from pyecore.ecore import EPackage,EObject
 
 
-from eoq2 import His, Cmp, Set, Crn, Add, Obj, Get, Pth, Qry, Met, Rem
+from eoq2 import Cmp, Set, Add
 import os
 import platform
 import shutil
 import glob
-import sys
 import time
-import logging
-from copy import copy
 import xml.etree.ElementTree
 import xml.dom.minidom
-from pathlib import Path,PureWindowsPath
+from pathlib import Path
 from timeit import default_timer
-from threading import Timer,Lock
+from threading import Timer
 import traceback
 
 # try importing for watchdog functions
 try:
     from watchdog.observers import Observer
     from watchdog.events import PatternMatchingEventHandler, FileSystemEvent, FileCreatedEvent
 except ImportError:
@@ -79,25 +76,24 @@
 #     RESOURCE_DEL = "RESOURCE_DEL"
 #     DIRECTORY_ADD = "DIRECTORY_ADD"
 #     DIRECTORY_MOV = "DIRECTORY_MOV"
 #     DIRECTORY_DEL = "DIRECTORY_DEL"
         
         
 class PyEcoreWorkspaceMdbProvider():
-    def __init__(self,baseDir,metaDir=['./.meta'],saveTimeout=10.0,logger=NoLogging(),autoload=True,trackFileChanges=True):
+    def __init__(self,baseDir,metaDir=['./.meta'],saveTimeout=10.0,logger=NoLogging(),autoload=True,trackFileChanges=False):
         super().__init__()
 
         self.baseDir = os.path.normpath(baseDir)
         self.baseDirAbs = os.path.join(os.getcwd(),self.baseDir)
         self.baseDirUri = URI(self.baseDir) 
         self.rset = ResourceSet()
         self.modelResourceLut = {}  #a look-up table between eResources and ModelResource objects
         self.eResourceLut = {}  #a look-up table between ModelResource and eResources objects
         self.eResourcesConnected = False
-        self.eResourceLock = Lock()
         self.metaDir = metaDir  #the directory that contains model definitions
         
         self.logger = logger
         
         self.modelroot = Workspace(name='.')  #clone behavior of the old localdomain
         self.lastPersistentPaths = {}  # dir or resources -> path
         self.dirtyResources = []  #stores all modified resources, such that they can be saved
@@ -127,15 +123,15 @@
             self.Load()
             
         #register this as an singelton
         global PROVIDER_INSTANCE
         PROVIDER_INSTANCE = self
         
         
-    def __del__(self):
+    def Close(self):
         #make sure any changes are saved
         #self.logger.Info("Closing workspace MDB ...") #makes problems when main thread has ended already
 
         self.__StopDelayedSaving()
         self.__SaveAllDirtyResources()
 
         #todo: there is a problem with the del which has to be investigated
@@ -538,14 +534,15 @@
             self.saveTimer = None
             
     def __DelayedSaving(self):
         self.__SaveAllDirtyResources()
         self.saveTimer = None
         
     def __SaveAllDirtyResources(self):
+        self.Lock()
         evts = []
         self.__ConnectAllEResources()  # necessary for model resources
         for resource in self.dirtyResources:
             try:
                 # add entry to the modified event list to ensure the resource wont get reloaded
                 self.AddFileEventToSkipList(FileSystemEvent(self.__GetLastPersitentPath(resource)),2)
                 self.__SaveResource(resource)
@@ -556,15 +553,15 @@
         self.__DisconnectAllEResources()  # necessary for model resources
 
         self.dirtyResources.clear()
         self.dirtyObjects.clear()
         
         #notify observers
         self.domain.NotifyObservers(evts, self)
-    
+        self.Release()
     
     ''' resource handling functions '''
 
     def __SetResourceDirty(self,resource):
         if(resource and resource not in self.dirtyResources):
             self.dirtyResources.append(resource)
             self.__InitSave()
@@ -813,15 +810,15 @@
         try:
             return self.eResourceLut[modelResource]
         except:
             return None
         
     def __ConnectAllEResources(self):
         if(not self.eResourcesConnected):
-            self.eResourceLock.acquire()
+            #self.eResourceLock.acquire()
             for resourceUri in self.rset.resources:
                 resource = self.rset.resources[resourceUri]
                 modelResource = self.__GetModelResourceForEResource(resource)
                 if(modelResource):
                     for content in resource.contents:
                         resource.remove(content)
                     for content in modelResource.contents:
@@ -829,15 +826,15 @@
                         #modelResource.contents.discard(content)
                     #HACK1: elements must be removed from the Resource in order to make save work
                     modelResource.contents.clear()
             self.eResourcesConnected = True
         
     def __DisconnectAllEResources(self):
         if(self.eResourcesConnected):
-            self.eResourceLock.release()
+            #self.eResourceLock.release()
             for resourceUri in self.rset.resources:
                 resource = self.rset.resources[resourceUri]
                 modelResource = self.__GetModelResourceForEResource(resource)
                 if(modelResource):
                     #HACK2: now read the content
                     for content in resource.contents:
                         modelResource.contents.add(content)
@@ -1514,11 +1511,11 @@
         return False
     
     def AddFileEventToSkipList(self,fileEvent,n):
         if(self.trackFileChanges):
             self.modifiedEventSkipList.append([fileEvent,n])
             
     def Lock(self):
-        self.__ConnectAllEResources()
+        self.mdb.Lock()
 
-    def Unlock(self):
-        self.__DisconnectAllEResources()
+    def Release(self):
+        self.mdb.Release()
```

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py` & `eoq2-2.2.9/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/query/query.py` & `eoq2-2.2.9/eoq2/query/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     'SUB' : '&SUB', 
     'MUL' : '&MUL', 
     'DIV' : '&DIV', 
     'ORR' : '&ORR', 
     'XOR' : '&XOR', 
     'AND' : '&AND', 
     'NAD' : '&NAD', 
-    'CSP' : '%', 
+    'CSP' : '&CSP', 
     'ITS' : '^', 
     'DIF' : '\\',
     'UNI' : '_', 
     'CON' : '|'
 }  
 #free symbols: *`´;
 #reserved symbols: {}()[]'"+-.,
@@ -384,14 +384,19 @@
         self.Not()
         
 class Idx(Qry):
     def __init__(self,n):
         super().__init__()
         self.Idx(n)
         
+class Sel(Qry):
+    def __init__(self,query):
+        super().__init__()
+        self.Sel(query)
+        
 class Arr(Qry):
     def __init__(self,elements):
         super().__init__()
         self.Arr(elements)       
     
 class Zip(Qry):
     def __init__(self,elements):
```

### Comparing `eoq2-2.2.6/eoq2/query/queryrunner.py` & `eoq2-2.2.9/eoq2/query/queryrunner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 from .query import QrySegTypes,QryMetaSegTypes,QryIdxTypes,ObjSeg,Qry,Seg
 from ..util.error import EoqError
 from ..util.util import ApplyToAllElements,ApplyToAllElementsInA,ApplyToAllElementsInB,ApplyToAllListsOfElementsInA,ApplyToSimilarElementStrutures,ApplyToSimilarListsOfObjects,IsList,IsListOfObjects,Terminator,Determinate,IsNoList
+from ..util.benchmark import Benchmark
 
 import re
+from eoq2.query.query import Try
 '''
     QueryRunner
     
     Evaluates a essential object query using a mdb accessor and value codec. Only the EvalOnContextAndScope function should be called
     
 '''
 
 class QryRunner:
-    def __init__(self,mdbAccessor):
+    def __init__(self,mdbAccessor,enableBenchmark=False):
         #self.mdb = mdb
         self.mdbAccessor = mdbAccessor
+        self.enableBenchmark = enableBenchmark
         self.segmentEvaluators = {}
         
+        #benchmark
+        if self.enableBenchmark:
+            self.benchmark = Benchmark()
+            allQryTypes = [getattr(QrySegTypes,k) for k in QrySegTypes.__dict__ if not k.startswith('_')]
+            for t in allQryTypes:
+                self.benchmark.InitMessure(t)
+        
         
         #Segment oparators
         self.segmentEvaluators[QrySegTypes.OBJ] = self.EvalObj
         self.segmentEvaluators[QrySegTypes.HIS] = self.EvalHis
         
         self.segmentEvaluators[QrySegTypes.PTH] = self.EvalPth
         self.segmentEvaluators[QrySegTypes.CLS] = self.EvalCls
@@ -276,42 +286,31 @@
         context = modelroot
         return self.EvalOnContextAndScope(context,qry,context,history)
         
     def EvalOnContextAndScope(self,context,seg,scope,history):
         res = None
         
         if(isinstance(seg,Seg)):
-            t = seg.qry
+            qryType = seg.qry
+            try:
+                evalFunction = self.segmentEvaluators[qryType] 
+            except KeyError as e:
+                raise EoqError(0,"Unknown segment type: %s: %s"%(qryType,str(e)))
+            if self.enableBenchmark: self.benchmark.Start()
             try:
-                evalFunction = self.segmentEvaluators[t]
                 v = seg.v 
                 res = evalFunction(context,v,scope,history)
-            except KeyError as e:
-                raise EoqError(0,"Unknown segment type: %s: %s"%(t,str(e)))
+            except Exception as e:
+                if self.enableBenchmark: self.benchmark.Stop(qryType)
+                raise e         
+            if self.enableBenchmark: self.benchmark.Stop(qryType)
         elif(IsList(seg)):
             res = self.EvalArr(context,seg,scope,history)
         else:
             res = seg #its a primitive value, do nothing
-#         try: 
-#             t = seg.qry
-#         except:
-#             if(IsList(seg)):
-#                 t = QrySegTypes.ARR
-#             else:
-#                 return seg
-#         #get eval function for the segment type
-#         try:
-#             evalFunction = self.segmentEvaluators[t]
-#         except KeyError as e:
-#             raise EoqError(0,"Unknown segment type: %s: %s"%(t,str(e)))
-#         
-#         #eval the current segment
-#         v = seg.v 
-#         res = evalFunction(context,v,scope,history)
-#         
         return res   
     
     '''
         SEGMENT EVALUATORS
     '''
         
     def EvalQry(self,context,args,scope,history):
@@ -417,19 +416,20 @@
             res = None
             query = b[0]
             default = b[1]
             history = b[2]
             try:
                 res = self.EvalOnContextAndScope(a,query,a,history)
             except:
-                res = default
+                res = self.EvalOnContextAndScope(a,default,a,history)
             return res
         
         query = args[0] #do not evaluate here but element-wise inside try
-        default = self.EvalOnContextAndScope(context,args[1],context,history)
+        default = args[1]
+        #default = self.EvalOnContextAndScope(context,args[1],context,history)
         
         res = ApplyToAllElementsInA(context,(query,default,history),tryFunctor)
         
         return res
     
     def EvalIdx(self,context,args,scope,history):
         res = None
```

### Comparing `eoq2-2.2.6/eoq2/serialization/jsonserializer.py` & `eoq2-2.2.9/eoq2/serialization/jsonserializer.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/serialization/jsserializer.py` & `eoq2-2.2.9/eoq2/serialization/jsserializer.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/serialization/pyserializer.py` & `eoq2-2.2.9/eoq2/serialization/pyserializer.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/serialization/textserializer.py` & `eoq2-2.2.9/eoq2/serialization/textserializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 from ..command.command import CmdTypes, Get, Set, Add, Rem, Mov, Clo, Crt, Crn, Qrf, Sts, Chg, Gaa, Cal, Asc, Abc, Cmp, Umm, \
     Rmm, Gmm, Obs, Ubs, Hel, Ses, Gby, Cpr, Mrg, Mut, Umt
 from ..util.error import EoqError
 
 from copy import deepcopy
 from enum import Enum
 import re
+import traceback
 
 """
     CONSTANTS & SETTINGS
 """
 
 # Create dictionary from external symbol definition.
 # This will be needed later to convert i.e. "!" -> "CLS"
 SYMBOLS_2_QRY_DICT = dict((v, k) for k, v in QRY_SYMBOLS.items())
 
 # List all commands that need a list of args and not *args or a mix
-QRY_CMDS_W_LIST_INPUT = ["[", "&ZIP", "&EQA"]
-QRY_CMDS_W_SINGLE_OR_LIST_INPUT = [":"]
+QRY_CMDS_W_LIST_INPUT = ["[","&ZIP"]
+QRY_CMDS_W_SINGLE_OR_LIST_INPUT = [":","&EQA"]
 QRY_CMDS_W_MIXED_INPUT = ["@"]
 
 # Settings of divider symbols
 EXPRESSION_DIVIDERS = [";", "\r", "\n"]
 QRY_ARG_DIVIDER = ","
 CMD_ARG_DIVIDER = " "
 
@@ -46,14 +47,16 @@
 # Assign stop symbols to starters
 STOPPING_SYMBOL_DICT = {
     "(": ")",
     "{": "}",
     "[": "]",
 }
 
+WHITESPACE_REGEX = re.compile("\s")
+
 
 def DoNothing(*args, **kwargs):
     """ placeholder for unimplemented functions """
     pass
 
 
 class ParsingCmds(Enum):
@@ -80,62 +83,60 @@
 
         """
             PY2TXT Translators
         """
         self.cmdTranslator = lambda o: o.cmd + " " + self._StripOuterQry(self.Ser(o.a))
 
         self.qryTranslators = {
-            QrySegTypes.OBJ: lambda o: QRY_SYMBOLS[QrySegTypes.OBJ] + self.Ser(o.v),
-            QrySegTypes.HIS: lambda o: QRY_SYMBOLS[QrySegTypes.HIS] + self.Ser(o.v),
-            QrySegTypes.PTH: lambda o: QRY_SYMBOLS[QrySegTypes.PTH] + self.Ser(o.v),
-            QrySegTypes.CLS: lambda o: QRY_SYMBOLS[QrySegTypes.CLS] + self.Ser(o.v),
-            QrySegTypes.INO: lambda o: QRY_SYMBOLS[QrySegTypes.INO] + self.Ser(o.v),
-            QrySegTypes.MET: lambda o: QRY_SYMBOLS[QrySegTypes.MET] + self.Ser(o.v),
+            QrySegTypes.OBJ: lambda o: QRY_SYMBOLS[QrySegTypes.OBJ] + self._TranslateQryArgs(o.v),
+            QrySegTypes.HIS: lambda o: QRY_SYMBOLS[QrySegTypes.HIS] + self._TranslateQryArgs(o.v),
+            QrySegTypes.PTH: lambda o: QRY_SYMBOLS[QrySegTypes.PTH] + self._TranslateQryArgs(o.v),
+            QrySegTypes.CLS: lambda o: QRY_SYMBOLS[QrySegTypes.CLS] + self._TranslateQryArgs(o.v),
+            QrySegTypes.INO: lambda o: QRY_SYMBOLS[QrySegTypes.INO] + self._TranslateQryArgs(o.v),
+            QrySegTypes.MET: lambda o: QRY_SYMBOLS[QrySegTypes.MET] + self._TranslateQryArgs(o.v,True),
             #QrySegTypes.MET: lambda o: QRY_SYMBOLS[QrySegTypes.MET] + "(" + self.Ser(o.v[0]) + (
             #    "," + self.Ser(o.v[1:]) if len(o.v) > 1 else "") + ")",
             QrySegTypes.NOT: lambda o: QRY_SYMBOLS[QrySegTypes.NOT],
-            QrySegTypes.TRM: lambda o: QRY_SYMBOLS[QrySegTypes.TRM] + "(" + self.Ser(o.v[0]) + "," + self.Ser(
-                o.v[1]) + ")",
-            QrySegTypes.TRY: lambda o: QRY_SYMBOLS[QrySegTypes.TRY] + "(" + self.Ser(o.v[0]) + "," + self.Ser(
-                o.v[1]) + ")",
-            QrySegTypes.IDX: lambda o: QRY_SYMBOLS[QrySegTypes.IDX] + self.Ser(o.v),
-            QrySegTypes.SEL: lambda o: "{" + self.Ser(o.v) + "}",
-            QrySegTypes.ARR: lambda o: "[" + ",".join([self.Ser(a) for a in o.v]) + "]",
-            QrySegTypes.ZIP: lambda o: QRY_SYMBOLS[QrySegTypes.ZIP] + self.Ser(o.v),
-            QrySegTypes.QRY: lambda o: "(" + "".join([self.Ser(a) for a in o.v]) + ")",
-            QrySegTypes.ANY: lambda o: QRY_SYMBOLS[QrySegTypes.ANY] + self.Ser(o.v),
-            QrySegTypes.ALL: lambda o: QRY_SYMBOLS[QrySegTypes.ALL] + self.Ser(o.v),
-            QrySegTypes.EQU: lambda o: QRY_SYMBOLS[QrySegTypes.EQU] + self.Ser(o.v),
-            QrySegTypes.EQA: lambda o: QRY_SYMBOLS[QrySegTypes.EQA] + self.Ser(o.v),
-            QrySegTypes.NEQ: lambda o: QRY_SYMBOLS[QrySegTypes.NEQ] + self.Ser(o.v),
-            QrySegTypes.LES: lambda o: QRY_SYMBOLS[QrySegTypes.LES] + self.Ser(o.v),
-            QrySegTypes.GRE: lambda o: QRY_SYMBOLS[QrySegTypes.GRE] + self.Ser(o.v),
-            QrySegTypes.RGX: lambda o: QRY_SYMBOLS[QrySegTypes.RGX] + self.Ser(o.v),
-            QrySegTypes.ADD: lambda o: QRY_SYMBOLS[QrySegTypes.ADD] + self.Ser(o.v),
-            QrySegTypes.SUB: lambda o: QRY_SYMBOLS[QrySegTypes.SUB] + self.Ser(o.v),
-            QrySegTypes.MUL: lambda o: QRY_SYMBOLS[QrySegTypes.MUL] + self.Ser(o.v),
-            QrySegTypes.DIV: lambda o: QRY_SYMBOLS[QrySegTypes.DIV] + self.Ser(o.v),
-            QrySegTypes.ORR: lambda o: QRY_SYMBOLS[QrySegTypes.ORR] + self.Ser(o.v),
-            QrySegTypes.XOR: lambda o: QRY_SYMBOLS[QrySegTypes.XOR] + self.Ser(o.v),
-            QrySegTypes.AND: lambda o: QRY_SYMBOLS[QrySegTypes.AND] + self.Ser(o.v),
-            QrySegTypes.NAD: lambda o: QRY_SYMBOLS[QrySegTypes.NAD] + self.Ser(o.v),
-            QrySegTypes.CSP: lambda o: QRY_SYMBOLS[QrySegTypes.CSP] + self.Ser(o.v),
-            QrySegTypes.ITS: lambda o: QRY_SYMBOLS[QrySegTypes.ITS] + self.Ser(o.v),
-            QrySegTypes.DIF: lambda o: QRY_SYMBOLS[QrySegTypes.DIF] + self.Ser(o.v),
-            QrySegTypes.UNI: lambda o: QRY_SYMBOLS[QrySegTypes.UNI] + self.Ser(o.v),
-            QrySegTypes.CON: lambda o: QRY_SYMBOLS[QrySegTypes.CON] + self.Ser(o.v)
+            QrySegTypes.TRM: lambda o: QRY_SYMBOLS[QrySegTypes.TRM] + self._TranslateQryArgs(o.v,True),
+            QrySegTypes.TRY: lambda o: QRY_SYMBOLS[QrySegTypes.TRY] + self._TranslateQryArgs(o.v,True),
+            QrySegTypes.IDX: lambda o: QRY_SYMBOLS[QrySegTypes.IDX] + self._TranslateQryArgs(o.v,True),
+            QrySegTypes.SEL: lambda o: self._TranslateQryArgs(o.v,False,'{','}',True), #"{" + self.Ser(o.v) + "}",
+            QrySegTypes.ARR: lambda o: self._TranslateQryArgs(o.v,True,'[',']',True), #"[" + ",".join([self.Ser(a) for a in o.v]) + "]",
+            QrySegTypes.ZIP: lambda o: QRY_SYMBOLS[QrySegTypes.ZIP] + self._TranslateQryArgs(o.v,True),
+            QrySegTypes.QRY: lambda o: self._TranslateQryArgs(o.v,True,'(',')',True,''), #"(" + "".join([self.Ser(a) for a in o.v]) + ")",
+            QrySegTypes.ANY: lambda o: QRY_SYMBOLS[QrySegTypes.ANY] + self._TranslateQryArgs(o.v),
+            QrySegTypes.ALL: lambda o: QRY_SYMBOLS[QrySegTypes.ALL] + self._TranslateQryArgs(o.v),
+            QrySegTypes.EQU: lambda o: QRY_SYMBOLS[QrySegTypes.EQU] + self._TranslateQryArgs(o.v),
+            QrySegTypes.EQA: lambda o: QRY_SYMBOLS[QrySegTypes.EQA] + self._TranslateQryArgs(o.v),
+            QrySegTypes.NEQ: lambda o: QRY_SYMBOLS[QrySegTypes.NEQ] + self._TranslateQryArgs(o.v),
+            QrySegTypes.LES: lambda o: QRY_SYMBOLS[QrySegTypes.LES] + self._TranslateQryArgs(o.v),
+            QrySegTypes.GRE: lambda o: QRY_SYMBOLS[QrySegTypes.GRE] + self._TranslateQryArgs(o.v),
+            QrySegTypes.RGX: lambda o: QRY_SYMBOLS[QrySegTypes.RGX] + self._TranslateQryArgs(o.v),
+            QrySegTypes.ADD: lambda o: QRY_SYMBOLS[QrySegTypes.ADD] + self._TranslateQryArgs(o.v),
+            QrySegTypes.SUB: lambda o: QRY_SYMBOLS[QrySegTypes.SUB] + self._TranslateQryArgs(o.v),
+            QrySegTypes.MUL: lambda o: QRY_SYMBOLS[QrySegTypes.MUL] + self._TranslateQryArgs(o.v),
+            QrySegTypes.DIV: lambda o: QRY_SYMBOLS[QrySegTypes.DIV] + self._TranslateQryArgs(o.v),
+            QrySegTypes.ORR: lambda o: QRY_SYMBOLS[QrySegTypes.ORR] + self._TranslateQryArgs(o.v),
+            QrySegTypes.XOR: lambda o: QRY_SYMBOLS[QrySegTypes.XOR] + self._TranslateQryArgs(o.v),
+            QrySegTypes.AND: lambda o: QRY_SYMBOLS[QrySegTypes.AND] + self._TranslateQryArgs(o.v),
+            QrySegTypes.NAD: lambda o: QRY_SYMBOLS[QrySegTypes.NAD] + self._TranslateQryArgs(o.v),
+            QrySegTypes.CSP: lambda o: QRY_SYMBOLS[QrySegTypes.CSP] + self._TranslateQryArgs(o.v),
+            QrySegTypes.ITS: lambda o: QRY_SYMBOLS[QrySegTypes.ITS] + self._TranslateQryArgs(o.v),
+            QrySegTypes.DIF: lambda o: QRY_SYMBOLS[QrySegTypes.DIF] + self._TranslateQryArgs(o.v),
+            QrySegTypes.UNI: lambda o: QRY_SYMBOLS[QrySegTypes.UNI] + self._TranslateQryArgs(o.v),
+            QrySegTypes.CON: lambda o: QRY_SYMBOLS[QrySegTypes.CON] + self._TranslateQryArgs(o.v)
         }
         self.priTranslators = {
             # primitive types
             bool: lambda o: str(o),
             int: lambda o: str(o),
             float: lambda o: str(o),
             str: lambda o: self._StringTranslator(o),
             list: lambda o: self._ListTranslator(o),
-            type(None): lambda o: ""
+            type(None): lambda o: "%"
         }
 
         self.lastTranslation = None
 
         """
             TXT2PY Constructors
         """
@@ -220,31 +221,64 @@
 
     @staticmethod
     def _IsNumerical(string):
         for c in string:
             if not c in ["0","1","2","3","4","5","6","7","8","9","-","+","E","e","."]:
                 return False
         return True
+    
+    @staticmethod
+    def _IsNone(string):
+        return string == '%'
+    
+    @staticmethod
+    def _ContainsForbiddenCharacter(string):
+        # string contains any whitespaces
+        if(WHITESPACE_REGEX.search(string)):
+            return True
+        #conflict with other primitives
+        if(string.startswith('+') or 
+           string.startswith('-') or 
+           string.startswith('.') or 
+           string.startswith('%') or 
+           string.startswith('0') or 
+           string.startswith('1') or 
+           string.startswith('2') or 
+           string.startswith('3') or 
+           string.startswith('4') or 
+           string.startswith('5') or 
+           string.startswith('6') or 
+           string.startswith('7') or 
+           string.startswith('8') or
+           string.startswith('9') or
+           string.lower() == "false" or 
+           string.lower() == "true" ):
+            return False
+        #string contains any query symbol or 
+        elif(any(s in string for s in ['#', '$', '/', '!', '?', '@', '&', ':', '{', '[', '(', '=', '~', '<', '>', '^', '\\', '_','|'])):
+            return False
+        return False
+        
 
     def _StringTranslator(self, string):
         idx = 0
         while idx < len(string):
             if any([self._IsCmdOrQry(x) for x in [string[idx], string[idx:min(idx+3,len(string))], string[idx:min(idx+4,len(string))]]])\
-                    or self._IsNumerical(string[0]):
+               or self._ContainsForbiddenCharacter(string):
                 return "'"+string+"'"
             idx += 1
         return string
 
     def _ListTranslator(self, li):
         if len(li)>1:
-            return "[%s]" % (",".join([self.Ser(x) for x in li]))
+            return "(%s)" % (",".join([self.Ser(x) for x in li]))
         elif len(li) == 1:
-            return "[%s]" % (self.Ser(li[0]))
+            return "(%s)" % (self.Ser(li[0]))
         else:
-            return "[]"
+            return "()"
 
     def _StripOuterQry(self, string):
         if REMOVE_OUTER_QRY_PARENTHESES and type(string) == str:
             try:
                 # pre-evaluating conditions to avoid out of range string slicing
                 cond1 = string[0] == "(" and string[-1] == ")"
             except:
@@ -262,31 +296,47 @@
             else:
                 return string
         else:
             return string
 
     def _TranslateCmd(self, o):
         if o.cmd:
-            if o.cmd == "CMP":
-                return ";".join([self.Ser(v) for v in o.a])
+            if o.cmd == CmdTypes.CMP:
+                return "\n".join([self.Ser(v) for v in o.a])
             elif type(o.a) == list:
-                return o.cmd + "(" + ",".join([self._StripOuterQry(self.Ser(v)) for v in o.a])+")"
+                return o.cmd + " " + " ".join([self._StripOuterQry(self.Ser(v)) for v in o.a])
             else:
                 argStr = self._StripOuterQry(self.Ser(o.a))
                 if(0 < len(argStr)):
                     return o.cmd + " " + argStr
                 else: #commands with no arguments
                     return o.cmd
 
     def _TranslateQry(self, o):
         if o.qry:
             return self.qryTranslators[o.qry](o)
+        
+    def _TranslateQryArgs(self,a,multiArgs=False,prefix="(",postfix=")",prePostFixForSingleElement=False,separator=","):
+        if(multiArgs and type(a) == list):
+            if(prePostFixForSingleElement or len(a)>1):
+                return prefix + separator.join([self.Ser(v) for v in a]) + postfix
+            elif(len(a)==1):
+                return self.Ser(a[0])
+            else: #0 element list
+                return ''
+        else:
+            if(prePostFixForSingleElement):
+                return prefix + self.Ser(a) + postfix
+            else:
+                return self.Ser(a)
 
     def _TranslatePri(self, o):
         return self.priTranslators[type(o)](o)
+    
+    
 
     def Ser(self, val):
         """
             Translates a Python command to EOQ code
         """
         try:
             return self._TranslateCmd(val)
@@ -474,15 +524,36 @@
 
         return func
 
     def _GetBaseConstructor(self, cmd):
         """
             returns a base constructor
         """
-        return self.combinedConstructors[cmd]
+        key = cmd.upper()
+        
+        # check if cmd takes list input
+        takesList = (key in QRY_SYMBOLS) and (QRY_SYMBOLS[key] in QRY_CMDS_W_LIST_INPUT)
+        takesSingleOrList = (cmd in QRY_SYMBOLS) and (QRY_SYMBOLS[key] in QRY_CMDS_W_SINGLE_OR_LIST_INPUT)
+        takesMix = (key in QRY_SYMBOLS) and (QRY_SYMBOLS[key] in QRY_CMDS_W_MIXED_INPUT)
+
+        # construct function
+        constructor = self.combinedConstructors[key]
+        
+        def func(args):
+            if takesList:
+                return constructor(args)
+            elif takesMix:
+                return constructor(args)
+            elif takesSingleOrList:
+                return constructor(args if len(args)>1 else args[0])
+            else:
+                return constructor(args)
+
+        return func
+        
 
     def _ConvertSegmentToFunction(self, seg, res):
         """
             Converts segment symbol to function if possible. I.e. "!" -> Cls()
         """
         if self._IsCmdOrQry(seg):
             if self._IsQry(seg):
@@ -494,50 +565,49 @@
             except:
                 func = self._GetBaseConstructor(cmd)
                 isBoundCmd = False
             return func, isBoundCmd
         else:
             raise EoqError(0, f"Segment {seg} is not convertible to a Python Function.")
 
-    @staticmethod
-    def _BalanceSteps(parsingList):
-        """
-            closes unclosed STEP_IN cmds, (currently unused)
-        """
-        toClose = 0
-        for seg in parsingList:
-            if seg == ParsingCmds.STEP_IN:
-                toClose += 1
-            elif seg == ParsingCmds.STEP_OUT:
-                toClose -= 1
-        for closing in range(toClose):
-            parsingList.append(ParsingCmds.STEP_OUT)
-        return parsingList
+#     @staticmethod
+#     def _BalanceSteps(parsingList):
+#         """
+#             closes unclosed STEP_IN cmds, (currently unused)
+#         """
+#         toClose = 0
+#         for seg in parsingList:
+#             if seg == ParsingCmds.STEP_IN:
+#                 toClose += 1
+#             elif seg == ParsingCmds.STEP_OUT:
+#                 toClose -= 1
+#         for closing in range(toClose):
+#             parsingList.append(ParsingCmds.STEP_OUT)
+#         return parsingList
 
     def _HandlePrimitives(self, code):
         #find out the right primitive type
         #use the first char to decide
         val = None
         c = code[0]
         if c == '\'': #quoted string
             val = code.strip("\'") #strip quotes
+        elif self._IsNone(code):
+            val = None
         elif self._IsNumerical(code): #number
             if '.' in code : #float
                 val = float(code)
             elif 'E' in code : #engineering float
                 val = float(code)
             else: #int
                 val = int(code)
-        elif c in ['T','t','F','f'] : #possible boolean
-            if code.lower() == 'true': #Boolean True
+        elif code.lower() == 'true': #Boolean True
                 val = True
-            elif code.lower() == 'false': #Boolean False
-                val = False
-            else: #unquoted string
-                val = code  
+        elif code.lower() == 'false': #Boolean False
+            val = False
         else: #unquoted string
             val = code 
         return val
 
     @staticmethod
     def _StripOuterWhitespace(code):
         return code.strip()
@@ -623,31 +693,33 @@
                     # count step ins within separated cmd arg blocks
                     stepInSinceCmdDivider += 1
 
 
             elif self._IsCmdDivider(seg):
                 if not cmdDividerSeen:
                     cmdDividerSeen = True
-                while cmdDividerSeen and stepInSinceCmdDivider:
-                    # balancing step outs
-                    parsingList.append(ParsingCmds.STEP_OUT)
-                    stepInSinceCmdDivider -= 1
-
-
-            elif self._IsQryDivider(seg):
-                if stepInSinceQryStart:
-                    # reset step-ins since qry to 1 start if qry divider met
-                    stepIns = stepInSinceQryStart.pop()
-                    while (stepIns - 1):
+                else: 
+                    while cmdDividerSeen and stepInSinceCmdDivider:
+                        # balancing step outs
                         parsingList.append(ParsingCmds.STEP_OUT)
-                        stepIns -= 1
-                    stepInSinceQryStart.append(1)
+                        stepInSinceCmdDivider -= 1
                     parsingList.append(seg)
 
 
+#             elif self._IsQryDivider(seg):
+#                 if stepInSinceQryStart:
+#                     # reset step-ins since qry to 1 start if qry divider met
+#                     stepIns = stepInSinceQryStart.pop()
+#                     while (stepIns - 1):
+#                         parsingList.append(ParsingCmds.STEP_OUT)
+#                         stepIns -= 1
+#                     stepInSinceQryStart.append(1)
+#                     parsingList.append(seg)
+
+
             elif self._IsStopperSymbol(seg):
                 if not expectedStoppingSymbols:
                     # found stopping symbol without query start
                     faultyIdx = len(segmentsCopy) - len(segments)
                     errorMsg = f"\nSolving of code failed at segment {faultyIdx}\n" \
                                f"Unexpected stopping symbol {seg}\n" \
                                f"...{segmentsCopy[faultyIdx - ERROR_MSG_VIEW_DISTANCE:faultyIdx]}" \
@@ -703,15 +775,15 @@
             lastSeg = seg
             seg = parsingList.pop(0)
 
             if self._IsCmdOrQry(seg):
                 if self._debugMode:
                     # print(f"converting {seg} using res {res}")
                     debugCounter.append(seg)
-                if self._IsQryDivider(lastSeg):
+                if self._IsQryDivider(lastSeg) or self._IsCmdDivider(lastSeg):
                     cmd, isBoundCmd = self._ConvertSegmentToFunction(seg, None)
                 else:
                     cmd, isBoundCmd = self._ConvertSegmentToFunction(seg, res)
 
             elif seg == ParsingCmds.STEP_IN:
                 if self._debugMode:
                     if isBoundCmd:
@@ -727,15 +799,15 @@
                 else:
                     res = [cmd(res_)]
 
             elif seg == ParsingCmds.STEP_OUT:
                 if self._debugMode:
                     print(f"stepping out returning {res}")
                 return res
-            elif not self._IsQryDivider(seg):
+            elif not self._IsQryDivider(seg) and not self._IsCmdDivider(seg):
                 res.append(self._HandlePrimitives(seg))
 
         if self._debugMode:
             print(f"stepping out with args {res}")
         return res
 
     def _ConstructCompound(self, commandList):
@@ -773,17 +845,19 @@
             parsingList = self._GetParsingList(segments)
             if self._debugMode:
                 print(parsingList)
             # deepcopy parsingList for error handling
             parsingListCopy = deepcopy(parsingList)
             # solve combined segments and parsing commands
             try:
-                results += self._SolveParsingList(parsingList)
+                command = self._SolveParsingList(parsingList)
+                results += command
             except:
                 # solver failed
+                traceback.print_exc()
                 faultyIdx = len(parsingListCopy) - max(1, len(parsingList))
                 errorMsg = f"\nSolving of code failed at segment {faultyIdx}\n" \
                            f"...{(parsingListCopy[faultyIdx - ERROR_MSG_VIEW_DISTANCE:faultyIdx])}" \
                            f" -->{parsingListCopy[faultyIdx]}<-- " \
                            f"{(parsingListCopy[faultyIdx + 1:faultyIdx + 1 + ERROR_MSG_VIEW_DISTANCE])}...\n"
                 raise EoqError(0, errorMsg)
```

### Comparing `eoq2-2.2.6/eoq2/util/backup.py` & `eoq2-2.2.9/eoq2/util/backup.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/util/csvconnector.py` & `eoq2-2.2.9/eoq2/util/csvconnector.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/util/error.py` & `eoq2-2.2.9/eoq2/util/error.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/util/logger.py` & `eoq2-2.2.9/eoq2/util/logger.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/util/model.py` & `eoq2-2.2.9/eoq2/util/model.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2/util/util.py` & `eoq2-2.2.9/eoq2/util/util.py`

 * *Files identical despite different names*

### Comparing `eoq2-2.2.6/eoq2.egg-info/SOURCES.txt` & `eoq2-2.2.9/eoq2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -60,12 +60,13 @@
 eoq2/serialization/jsonserializer.py
 eoq2/serialization/jsserializer.py
 eoq2/serialization/pyserializer.py
 eoq2/serialization/serializer.py
 eoq2/serialization/textserializer.py
 eoq2/util/__init__.py
 eoq2/util/backup.py
+eoq2/util/benchmark.py
 eoq2/util/csvconnector.py
 eoq2/util/error.py
 eoq2/util/logger.py
 eoq2/util/model.py
 eoq2/util/util.py
```

### Comparing `eoq2-2.2.6/setup.py` & `eoq2-2.2.9/setup.py`

 * *Files identical despite different names*

