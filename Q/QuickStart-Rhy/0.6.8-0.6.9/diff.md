# Comparing `tmp/QuickStart_Rhy-0.6.8.tar.gz` & `tmp/QuickStart_Rhy-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickStart_Rhy-0.6.8.tar", last modified: Thu Feb 24 11:30:13 2022, max compression
+gzip compressed data, was "QuickStart_Rhy-0.6.9.tar", last modified: Wed Mar  2 09:21:30 2022, max compression
```

## Comparing `QuickStart_Rhy-0.6.8.tar` & `QuickStart_Rhy-0.6.9.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.710536 QuickStart_Rhy-0.6.8/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1067 2019-09-20 01:32:29.000000 QuickStart_Rhy-0.6.8/LICENSE
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      878 2022-02-24 11:30:13.710605 QuickStart_Rhy-0.6.8/PKG-INFO
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.705326 QuickStart_Rhy-0.6.8/QuickStart_Rhy/
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.707337 QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     5540 2021-06-02 09:40:32.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/AliCloud.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3312 2022-01-25 08:11:19.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/BaiduCloud.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1207 2022-01-14 15:40:03.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/Lolicon.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     5783 2021-06-02 09:41:17.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/QiniuOSS.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     8909 2022-02-20 18:53:33.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/SimpleAPI.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     6365 2021-05-15 16:08:12.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/TencentCloud.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1110 2021-02-23 18:02:37.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/__init__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    20384 2022-01-31 06:47:25.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/alapi.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.708166 QuickStart_Rhy-0.6.8/QuickStart_Rhy/ImageTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     2307 2021-08-07 06:49:25.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/ImageTools/ColorTools.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    10325 2022-02-18 15:11:23.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/ImageTools/ImagePreview.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      478 2021-08-07 06:47:43.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/ImageTools/ImageTools.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4005 2021-10-29 01:06:50.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/ImageTools/VideoTools.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       75 2021-01-14 15:40:19.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/ImageTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.709132 QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1716 2021-04-14 06:04:07.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/HttpServer.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4934 2021-06-11 16:15:17.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/M3u8DL.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    11344 2022-02-18 15:22:20.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/NormalDL.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3673 2021-04-25 15:34:28.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/WiFi.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3103 2021-01-27 06:50:19.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/WiFiDarwin.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     5763 2021-02-23 14:24:09.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.709712 QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     8861 2021-04-27 13:27:14.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/Compress.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4941 2021-04-30 07:48:42.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/Diff.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1127 2021-01-14 16:13:24.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/FileHash.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1786 2021-04-04 02:34:42.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/Monitor.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      623 2021-06-11 16:14:44.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.709830 QuickStart_Rhy-0.6.8/QuickStart_Rhy/ThreadTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     2794 2021-01-14 16:19:31.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/ThreadTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.710302 QuickStart_Rhy-0.6.8/QuickStart_Rhy/TuiTools/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3859 2022-02-19 14:40:16.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/TuiTools/Bar.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1292 2021-04-04 02:31:01.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/TuiTools/Line.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      549 2021-04-25 15:17:49.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/TuiTools/Table.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      102 2022-02-19 14:45:24.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/TuiTools/__init__.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.710426 QuickStart_Rhy-0.6.8/QuickStart_Rhy/Wrapper/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4765 2021-01-25 08:16:22.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/Wrapper/__init__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     9563 2022-02-19 14:36:18.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/__config__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     7076 2022-02-20 18:27:06.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/__init__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    36640 2022-02-24 10:00:27.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/api.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)    12754 2022-02-24 10:06:39.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/funcList.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     5368 2021-10-27 04:35:12.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/imageDeal.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3648 2022-02-13 16:31:26.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/main.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     9085 2022-01-29 04:45:18.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/netTools.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     2288 2022-02-14 15:11:41.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/qsLesson.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     4882 2021-08-07 07:00:24.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy/system.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-02-24 11:30:13.706151 QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      878 2022-02-24 11:30:13.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/PKG-INFO
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1650 2022-02-24 11:30:13.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/SOURCES.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-02-24 11:30:13.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/dependency_links.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       49 2022-02-24 11:30:13.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/entry_points.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       56 2022-02-24 11:30:13.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/requires.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       15 2022-02-24 11:30:13.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/top_level.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2020-04-02 18:40:53.000000 QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/zip-safe
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      425 2021-10-31 04:57:47.000000 QuickStart_Rhy-0.6.8/README.md
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      140 2022-02-24 11:30:13.710843 QuickStart_Rhy-0.6.8/setup.cfg
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      930 2022-02-24 11:29:58.000000 QuickStart_Rhy-0.6.8/setup.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288929 QuickStart_Rhy-0.6.9/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1067 2019-09-20 01:32:29.000000 QuickStart_Rhy-0.6.9/LICENSE
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      878 2022-03-02 09:21:30.289005 QuickStart_Rhy-0.6.9/PKG-INFO
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.283704 QuickStart_Rhy-0.6.9/QuickStart_Rhy/
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.285666 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     5540 2021-06-02 09:40:32.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/AliCloud.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3312 2022-01-25 08:11:19.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/BaiduCloud.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1207 2022-01-14 15:40:03.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/Lolicon.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     5783 2021-06-02 09:41:17.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/QiniuOSS.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     8909 2022-02-20 18:53:33.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/SimpleAPI.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     6365 2021-05-15 16:08:12.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/TencentCloud.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1110 2021-02-23 18:02:37.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/__init__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    20384 2022-01-31 06:47:25.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/alapi.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.286469 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     2307 2021-08-07 06:49:25.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ColorTools.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    10325 2022-02-18 15:11:23.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ImagePreview.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      478 2021-08-07 06:47:43.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ImageTools.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4005 2021-10-29 01:06:50.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/VideoTools.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       75 2021-01-14 15:40:19.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.287544 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1716 2021-04-14 06:04:07.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/HttpServer.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4934 2021-06-11 16:15:17.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/M3u8DL.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3649 2022-03-02 09:15:49.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/MultiSingleDL.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    11332 2022-03-02 05:36:33.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/NormalDL.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3673 2021-04-25 15:34:28.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFi.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3103 2021-01-27 06:50:19.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFiDarwin.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     5763 2021-02-23 14:24:09.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288114 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     8861 2021-04-27 13:27:14.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Compress.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4941 2021-04-30 07:48:42.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Diff.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1127 2021-01-14 16:13:24.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/FileHash.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1786 2021-04-04 02:34:42.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Monitor.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      623 2021-06-11 16:14:44.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288228 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ThreadTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     2794 2021-01-14 16:19:31.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ThreadTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288698 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4118 2022-03-02 05:29:22.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Bar.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1292 2021-04-04 02:31:01.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Line.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      549 2021-04-25 15:17:49.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Table.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      102 2022-02-19 14:45:24.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288813 QuickStart_Rhy-0.6.9/QuickStart_Rhy/Wrapper/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4765 2021-01-25 08:16:22.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/Wrapper/__init__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     9563 2022-02-19 14:36:18.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/__config__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     7076 2022-02-20 18:27:06.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/__init__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    36966 2022-02-25 17:33:50.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/api.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    12754 2022-02-24 10:06:39.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/funcList.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     5368 2021-10-27 04:35:12.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/imageDeal.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3648 2022-02-13 16:31:26.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/main.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     9085 2022-01-29 04:45:18.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/netTools.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     2288 2022-02-14 15:11:41.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/qsLesson.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4882 2021-08-07 07:00:24.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/system.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.284587 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      878 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/PKG-INFO
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1636 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/SOURCES.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/dependency_links.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       49 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/entry_points.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       56 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/requires.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       15 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/top_level.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2020-04-02 18:40:53.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/zip-safe
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      425 2021-10-31 04:57:47.000000 QuickStart_Rhy-0.6.9/README.md
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      140 2022-03-02 09:21:30.289244 QuickStart_Rhy-0.6.9/setup.cfg
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      930 2022-03-02 09:21:22.000000 QuickStart_Rhy-0.6.9/setup.py
```

### Comparing `QuickStart_Rhy-0.6.8/LICENSE` & `QuickStart_Rhy-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/PKG-INFO` & `QuickStart_Rhy-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickStart_Rhy
-Version: 0.6.8
+Version: 0.6.9
 Summary: Simplify the operation in terminal!
 Home-page: https://github.com/Rhythmicc/qs
 Author: RhythmLian
 License: MIT
 Keywords: Simplify the operation in terminal!
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/AliCloud.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/AliCloud.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/BaiduCloud.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/BaiduCloud.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/Lolicon.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/Lolicon.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/QiniuOSS.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/QiniuOSS.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/SimpleAPI.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/SimpleAPI.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/TencentCloud.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/TencentCloud.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/__init__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/__init__.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/API/alapi.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/alapi.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/ImageTools/ColorTools.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ColorTools.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/ImageTools/ImagePreview.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ImagePreview.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/ImageTools/VideoTools.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/VideoTools.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/HttpServer.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/HttpServer.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/M3u8DL.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/M3u8DL.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/NormalDL.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/NormalDL.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             qs_default_console.print(qs_error_string if failed2exit else qs_warning_string,
                                      'Get File information failed, please check network!'
                                      if user_lang != 'zh' else '获取文件信息失败，请检查网络!')
             if failed2exit:
                 self.enabled = False
                 return
         if self.name and '.' not in self.name:
-            self.name = self.name = os.path.basename(url)
+            self.name = os.path.basename(url)
         if name:
             self.name = name
 
         if os.path.exists(self.name) and self.exit_if_exist:
             self.enabled = False
             return
```

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/WiFi.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFi.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/WiFiDarwin.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFiDarwin.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/NetTools/__init__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/__init__.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/Compress.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Compress.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/Diff.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Diff.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/FileHash.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/FileHash.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/Monitor.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Monitor.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/SystemTools/__init__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/__init__.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/ThreadTools/__init__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ThreadTools/__init__.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/TuiTools/Bar.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,7 +137,15 @@
                 ('Unknow size' if user_lang != 'zh' else '未知大小'),
                 justify="right"
             ),
             BarColumn(bar_width=None),
             DownloadColumn(),
             console=qs_default_console
         )
+
+
+def NormalProgressBar(task_name, total):
+    from .. import qs_default_console
+    from rich.progress import Progress
+    progress = Progress()
+    task_id = progress.add_task(task_name, total=total, console=qs_default_console)
+    return progress, task_id
```

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/TuiTools/Line.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Line.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/TuiTools/Table.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Table.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/Wrapper/__init__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/Wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/__config__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/__config__.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/__init__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/__init__.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/api.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -948,36 +948,47 @@
 
 def d2m():
     """
     番号搜索并复制磁力链
 
     :return:
     """
+    global url
     try:
         designation = sys.argv[2]
-    except:
+    except IndexError:
         return qs_default_console.print(qs_error_string, 'qs m2u <designation>')
 
     from PyInquirer import prompt
     from .API.SimpleAPI import Designation2magnet
 
     copy = requirePackage('pyperclip', 'copy', not_ask=True)
+    PyperclipException = requirePackage('pyperclip', 'PyperclipException')
+    copied = False
 
     searcher = Designation2magnet(designation)
     infos = searcher.search_designation()
     choices = [f'[{n + 1}] ' + i[1] + ': ' + i[-1] for n, i in enumerate(infos)]
 
-    (copy if copy is not None else qs_default_console.print)(
-        searcher.get_magnet(
-            infos[
-                choices.index(prompt({
-                    'type': 'list',
-                    'message': 'Select | 选择',
-                    'name': 'sub-url',
-                    'choices': choices
-                })['sub-url'])
-            ][0]
+    try:
+        url = searcher.get_magnet(
+                infos[
+                    choices.index(prompt({
+                        'type': 'list',
+                        'message': 'Select | 选择',
+                        'name': 'sub-url',
+                        'choices': choices
+                    })['sub-url'])
+                ][0]
         )
-    )
+        if copy:
+            copy(url)
+            copied = True
+        else:
+            raise PyperclipException
+    except KeyError:
+        return
+    except PyperclipException:
+        qs_default_console.print(qs_info_string, url)
 
-    if copy is not None:
+    if copied:
         qs_default_console.print(qs_info_string, 'magnet url copied to clipboard' if user_lang != 'zh' else '磁力链接已拷贝至粘贴板')
```

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/funcList.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/funcList.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/imageDeal.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/imageDeal.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/main.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/main.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/netTools.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/netTools.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/qsLesson.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/qsLesson.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy/system.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/system.py`

 * *Files identical despite different names*

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/PKG-INFO` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickStart-Rhy
-Version: 0.6.8
+Version: 0.6.9
 Summary: Simplify the operation in terminal!
 Home-page: https://github.com/Rhythmicc/qs
 Author: RhythmLian
 License: MIT
 Keywords: Simplify the operation in terminal!
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `QuickStart_Rhy-0.6.8/QuickStart_Rhy.egg-info/SOURCES.txt` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 setup.cfg
 setup.py
 QuickStart_Rhy/__config__.py
 QuickStart_Rhy/__init__.py
 QuickStart_Rhy/api.py
 QuickStart_Rhy/funcList.py
 QuickStart_Rhy/imageDeal.py
-QuickStart_Rhy/imagedeal.py
 QuickStart_Rhy/main.py
 QuickStart_Rhy/netTools.py
-QuickStart_Rhy/nettools.py
 QuickStart_Rhy/qsLesson.py
 QuickStart_Rhy/system.py
 QuickStart_Rhy.egg-info/PKG-INFO
 QuickStart_Rhy.egg-info/SOURCES.txt
 QuickStart_Rhy.egg-info/dependency_links.txt
 QuickStart_Rhy.egg-info/entry_points.txt
 QuickStart_Rhy.egg-info/requires.txt
@@ -31,14 +29,15 @@
 QuickStart_Rhy/ImageTools/ColorTools.py
 QuickStart_Rhy/ImageTools/ImagePreview.py
 QuickStart_Rhy/ImageTools/ImageTools.py
 QuickStart_Rhy/ImageTools/VideoTools.py
 QuickStart_Rhy/ImageTools/__init__.py
 QuickStart_Rhy/NetTools/HttpServer.py
 QuickStart_Rhy/NetTools/M3u8DL.py
+QuickStart_Rhy/NetTools/MultiSingleDL.py
 QuickStart_Rhy/NetTools/NormalDL.py
 QuickStart_Rhy/NetTools/WiFi.py
 QuickStart_Rhy/NetTools/WiFiDarwin.py
 QuickStart_Rhy/NetTools/__init__.py
 QuickStart_Rhy/SystemTools/Compress.py
 QuickStart_Rhy/SystemTools/Diff.py
 QuickStart_Rhy/SystemTools/FileHash.py
```

### Comparing `QuickStart_Rhy-0.6.8/setup.py` & `QuickStart_Rhy-0.6.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-VERSION = '0.6.8'
+VERSION = '0.6.9'
 
 setup(
     name='QuickStart_Rhy',
     version=VERSION,
     description='Simplify the operation in terminal!',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

