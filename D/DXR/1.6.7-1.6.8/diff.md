# Comparing `tmp/DXR-1.6.7.tar.gz` & `tmp/DXR-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR-1.6.7.tar", last modified: Thu Apr 13 01:30:49 2023, max compression
+gzip compressed data, was "DXR-1.6.8.tar", last modified: Fri Apr 14 07:14:53 2023, max compression
```

## Comparing `DXR-1.6.7.tar` & `DXR-1.6.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.376507 DXR-1.6.7/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.330310 DXR-1.6.7/DXR.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1291 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      114 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/top_level.txt
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.331985 DXR-1.6.7/Dxr_Chat/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.6.7/Dxr_Chat/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.6.7/Dxr_Chat/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.6.7/Dxr_Chat/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.333937 DXR-1.6.7/Dxr_bytes/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.6.7/Dxr_bytes/Dxr_bytes.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_bytes/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.337215 DXR-1.6.7/Dxr_file/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.6.7/Dxr_file/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.6.7/Dxr_file/dxr_file.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2724 2023-02-24 03:25:36.000000 DXR-1.6.7/Dxr_file/dxr_request.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2715 2023-02-24 03:33:13.000000 DXR-1.6.7/Dxr_file/dxr_request_ros.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.6.7/Dxr_file/dxr_ssh.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.343263 DXR-1.6.7/Dxr_grpc/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.6.7/Dxr_grpc/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.6.7/Dxr_grpc/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.6.7/Dxr_grpc/audios_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.6.7/Dxr_grpc/audios_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.6.7/Dxr_grpc/dxr_grpc_audio_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.6.7/Dxr_grpc/dxr_grpc_audio_server.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.6.7/Dxr_grpc/dxr_grpc_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.6.7/Dxr_grpc/dxr_grpc_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.346635 DXR-1.6.7/Dxr_isapi/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.6.7/Dxr_isapi/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    28811 2023-04-13 01:29:11.000000 DXR-1.6.7/Dxr_isapi/api.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.6.7/Dxr_isapi/constants.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.6.7/Dxr_isapi/error.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.6.7/Dxr_isapi/ir_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.348302 DXR-1.6.7/Dxr_log/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_log/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_log/log.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.353774 DXR-1.6.7/Dxr_mqtt/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_mqtt/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_mqtt/dxr_log.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    13811 2023-04-13 01:29:11.000000 DXR-1.6.7/Dxr_mqtt/dxr_mqtt.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_mqtt/dxr_mqtt_2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.6.7/Dxr_mqtt/msg.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.357704 DXR-1.6.7/Dxr_serial/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.6.7/Dxr_serial/Dxr_serial.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_serial/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.361499 DXR-1.6.7/Dxr_utils/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_utils/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_utils/dxr_ftp.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_utils/dxr_utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_utils/gvalues.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.370169 DXR-1.6.7/Dxr_video/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/HCNetSDK.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/PlayCtrl.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/global_values.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/test_main.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/video.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/video_hk.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/video_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.373849 DXR-1.6.7/Dxr_voice/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.6.7/Dxr_voice/dxr_tts.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.6.7/Dxr_voice/dxr_whisper.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.375128 DXR-1.6.7/Dxr_yaml/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.6.7/Dxr_yaml/Dxr_yaml.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_yaml/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-13 01:30:49.375797 DXR-1.6.7/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.6.7/README.md
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-13 01:30:49.376739 DXR-1.6.7/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      563 2023-04-13 01:30:43.000000 DXR-1.6.7/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.977959 DXR-1.6.8/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.886055 DXR-1.6.8/DXR.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1291 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      114 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/top_level.txt
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.892933 DXR-1.6.8/Dxr_Chat/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.6.8/Dxr_Chat/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.6.8/Dxr_Chat/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.6.8/Dxr_Chat/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.901272 DXR-1.6.8/Dxr_bytes/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.6.8/Dxr_bytes/Dxr_bytes.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_bytes/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.920457 DXR-1.6.8/Dxr_file/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.6.8/Dxr_file/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.6.8/Dxr_file/dxr_file.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2724 2023-02-24 03:25:36.000000 DXR-1.6.8/Dxr_file/dxr_request.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2715 2023-02-24 03:33:13.000000 DXR-1.6.8/Dxr_file/dxr_request_ros.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.6.8/Dxr_file/dxr_ssh.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.944034 DXR-1.6.8/Dxr_grpc/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.6.8/Dxr_grpc/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.6.8/Dxr_grpc/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.6.8/Dxr_grpc/audios_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.6.8/Dxr_grpc/audios_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.6.8/Dxr_grpc/dxr_grpc_audio_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.6.8/Dxr_grpc/dxr_grpc_audio_server.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.6.8/Dxr_grpc/dxr_grpc_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.6.8/Dxr_grpc/dxr_grpc_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.948708 DXR-1.6.8/Dxr_isapi/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.6.8/Dxr_isapi/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28811 2023-04-13 01:29:11.000000 DXR-1.6.8/Dxr_isapi/api.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.6.8/Dxr_isapi/constants.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.6.8/Dxr_isapi/error.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.6.8/Dxr_isapi/ir_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.950724 DXR-1.6.8/Dxr_log/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_log/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_log/log.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.955634 DXR-1.6.8/Dxr_mqtt/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_mqtt/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_mqtt/dxr_log.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.6.8/Dxr_mqtt/dxr_mqtt.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_mqtt/dxr_mqtt_2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.6.8/Dxr_mqtt/msg.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.958259 DXR-1.6.8/Dxr_serial/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.6.8/Dxr_serial/Dxr_serial.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_serial/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.961505 DXR-1.6.8/Dxr_utils/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_utils/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_utils/dxr_ftp.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_utils/dxr_utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_utils/gvalues.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.972410 DXR-1.6.8/Dxr_video/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/HCNetSDK.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/PlayCtrl.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/global_values.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/test_main.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/video.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/video_hk.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/video_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.975367 DXR-1.6.8/Dxr_voice/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.6.8/Dxr_voice/dxr_tts.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.6.8/Dxr_voice/dxr_whisper.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.976563 DXR-1.6.8/Dxr_yaml/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.6.8/Dxr_yaml/Dxr_yaml.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_yaml/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-14 07:14:53.977081 DXR-1.6.8/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.6.8/README.md
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-14 07:14:53.978145 DXR-1.6.8/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      563 2023-04-14 07:14:44.000000 DXR-1.6.8/setup.py
```

### Comparing `DXR-1.6.7/DXR.egg-info/SOURCES.txt` & `DXR-1.6.8/DXR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_Chat/ChatGPT.py` & `DXR-1.6.8/Dxr_Chat/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_Chat/utils.py` & `DXR-1.6.8/Dxr_Chat/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_bytes/Dxr_bytes.py` & `DXR-1.6.8/Dxr_bytes/Dxr_bytes.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_file/dxr_file.py` & `DXR-1.6.8/Dxr_file/dxr_file.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_file/dxr_request.py` & `DXR-1.6.8/Dxr_file/dxr_request.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_file/dxr_request_ros.py` & `DXR-1.6.8/Dxr_file/dxr_request_ros.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_file/dxr_ssh.py` & `DXR-1.6.8/Dxr_file/dxr_ssh.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_grpc/Datas_pb2.py` & `DXR-1.6.8/Dxr_grpc/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_grpc/Datas_pb2_grpc.py` & `DXR-1.6.8/Dxr_grpc/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_grpc/audios_pb2.py` & `DXR-1.6.8/Dxr_grpc/audios_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_grpc/audios_pb2_grpc.py` & `DXR-1.6.8/Dxr_grpc/audios_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_grpc/dxr_grpc_audio_client.py` & `DXR-1.6.8/Dxr_grpc/dxr_grpc_audio_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_grpc/dxr_grpc_audio_server.py` & `DXR-1.6.8/Dxr_grpc/dxr_grpc_audio_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_grpc/dxr_grpc_client.py` & `DXR-1.6.8/Dxr_grpc/dxr_grpc_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_grpc/dxr_grpc_server.py` & `DXR-1.6.8/Dxr_grpc/dxr_grpc_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_isapi/api.py` & `DXR-1.6.8/Dxr_isapi/api.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_isapi/error.py` & `DXR-1.6.8/Dxr_isapi/error.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_isapi/ir_client.py` & `DXR-1.6.8/Dxr_isapi/ir_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_log/log.py` & `DXR-1.6.8/Dxr_log/log.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_mqtt/dxr_mqtt.py` & `DXR-1.6.8/Dxr_mqtt/dxr_mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,31 +149,43 @@
     global callback_dit
     msg = str(msg.payload.decode("utf-8"))
     if type(msg) is str:
         msg = json.loads(msg)
     if topic not in callback_dit:
         isTongPei = False
         keys = callback_dit.keys()
+        topic_arr = topic.split("/")[1:]
+        # 遇到+号的topic，需要进行通配符匹配, 遇到#号，后面的topic不需要再匹配
         for item in keys:
-            if "+" in item:
-                item_arr = item.split("/")[1:]
-                topic_arr = topic.split("/")[1:]
-                if item_arr[0] == topic_arr[0]:
-                    isTongPei = True
+            item_arr = item.split("/")[1:]
+            tmp_TonPei = True
+            for i in range(len(item_arr)):
+                if item_arr[i] == "+":
+                    continue
+                if item_arr[i] == "#":
                     break
+                if item_arr[i] != topic_arr[i]:
+                    tmp_TonPei = False
+                    break
+            if tmp_TonPei:
+                isTongPei = True
+                callback_dit[topic] = {'func': callback_dit[item]['func'], 'cond': callback_dit[item]['cond'], 'msg': None}
+                break
         if not isTongPei:
             callback_dit[topic] = {'func': None, 'cond': threading.Event(), 'msg': None}
     callback_dit[topic]['msg'] = msg
     cond = get_cond(topic)
     cond.set()
     cond.clear()
     if callback_dit[topic]['func'] is not None:
         func = callback_dit[topic]['func']
         if '+' in topic:
             func(msg, client)
+        elif '#' in topic:
+            func(msg, client)
         else:
             func(msg, topic)
 
 
 # 一旦订阅成功，回调此方法
 def on_subscribe(mqttc, obj, mid, granted_qos):
     # print("Subscribed: " + str(mid) + " " + str(granted_qos))
@@ -341,16 +353,14 @@
             if isinstance(topic, str):
                 await_topic = topic
             else:
                 await_topic = topic.topic
         if await_topic is None:
             return None
         await_topic = await_topic.replace('pc', 'client')
-        if await_topic in callback_dit:
-            callback_dit[await_topic]['msg'] = None
         cond = get_cond(await_topic)
         if cond is None:
             return None
         if timeout is None:
             cond.wait()
         else:
             cond.wait(timeout)
@@ -424,8 +434,8 @@
                 else:
                     final_str = final_str + str(arg) + end
             except:
                 final_str = final_str + str(arg) + end
         logger.opt(colors=True).info(f'<yellow>{file_name}:{line}</yellow>(<blue>{thread_name}:{thread_count}</blue>)\r\n{final_str}')
     
         
-# print = monky_print
+print = monky_print
```

### Comparing `DXR-1.6.7/Dxr_mqtt/dxr_mqtt_2.py` & `DXR-1.6.8/Dxr_mqtt/dxr_mqtt_2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_mqtt/msg.py` & `DXR-1.6.8/Dxr_mqtt/msg.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_serial/Dxr_serial.py` & `DXR-1.6.8/Dxr_serial/Dxr_serial.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_utils/dxr_ftp.py` & `DXR-1.6.8/Dxr_utils/dxr_ftp.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_utils/dxr_utils.py` & `DXR-1.6.8/Dxr_utils/dxr_utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_video/Datas_pb2.py` & `DXR-1.6.8/Dxr_video/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_video/Datas_pb2_grpc.py` & `DXR-1.6.8/Dxr_video/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_video/HCNetSDK.py` & `DXR-1.6.8/Dxr_video/HCNetSDK.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_video/PlayCtrl.py` & `DXR-1.6.8/Dxr_video/PlayCtrl.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_video/test_main.py` & `DXR-1.6.8/Dxr_video/test_main.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_video/video.py` & `DXR-1.6.8/Dxr_video/video.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_video/video_hk.py` & `DXR-1.6.8/Dxr_video/video_hk.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_video/video_server.py` & `DXR-1.6.8/Dxr_video/video_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_voice/dxr_tts.py` & `DXR-1.6.8/Dxr_voice/dxr_tts.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/Dxr_yaml/Dxr_yaml.py` & `DXR-1.6.8/Dxr_yaml/Dxr_yaml.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/README.md` & `DXR-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `DXR-1.6.7/setup.py` & `DXR-1.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='DXR',
-    version='1.6.7',
+    version='1.6.8',
     packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat'],
     install_requires=['paho-mqtt', 'pyyaml', 'pyserial', 'loguru','tabulate', 'pymysql', 'sqlalchemy', 'oss2', 'imagezmq', 'simplejpeg', 'pexpect', 'aiortsp'],
     author='luzhipeng',
     author_email='402087139@qq.com',
     license='MIT',
     url='http://pycn.me',
     description='DXR is a python library for DXR_mqtt',
```

