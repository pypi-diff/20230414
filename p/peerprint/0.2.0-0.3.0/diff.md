# Comparing `tmp/peerprint-0.2.0.tar.gz` & `tmp/peerprint-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/oprint/continuousprint/peerprint/dist/tmpyb6dt3v3/peerprint-0.2.0.tar", last modified: Fri Nov 18 15:45:15 2022, max compression
+gzip compressed data, was "/volume/dist/.tmp-32lta849/peerprint-0.3.0.tar", last modified: Fri Apr 14 21:23:42 2023, max compression
```

## Comparing `peerprint-0.2.0.tar` & `peerprint-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 oprint    (1000) oprint    (1000)        0 2022-11-18 15:45:15.000000 peerprint-0.2.0/
--rw-r--r--   0 oprint    (1000) oprint    (1000)    11357 2022-08-25 19:29:48.000000 peerprint-0.2.0/LICENSE
--rw-r--r--   0 oprint    (1000) oprint    (1000)     3152 2022-11-18 15:45:15.000000 peerprint-0.2.0/PKG-INFO
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2608 2022-11-11 03:04:57.000000 peerprint-0.2.0/README.md
-drwxr-xr-x   0 oprint    (1000) oprint    (1000)        0 2022-11-18 15:45:15.000000 peerprint-0.2.0/peerprint/
--rw-r--r--   0 oprint    (1000) oprint    (1000)        0 2022-09-03 16:19:30.000000 peerprint-0.2.0/peerprint/__init__.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     4292 2022-11-16 23:53:16.000000 peerprint-0.2.0/peerprint/discovery.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     7230 2022-11-17 14:06:54.000000 peerprint-0.2.0/peerprint/filesharing.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     4922 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/filesharing_test.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     6310 2022-10-20 01:36:38.000000 peerprint-0.2.0/peerprint/lan_queue.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     3458 2022-09-03 16:19:30.000000 peerprint-0.2.0/peerprint/lan_queue_test.py
-drwxr-xr-x   0 oprint    (1000) oprint    (1000)        0 2022-11-18 15:45:15.000000 peerprint-0.2.0/peerprint/server/
--rw-r--r--   0 oprint    (1000) oprint    (1000)        0 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/server/__init__.py
-drwxr-xr-x   0 oprint    (1000) oprint    (1000)        0 2022-11-18 15:45:15.000000 peerprint-0.2.0/peerprint/server/proto/
--rw-r--r--   0 oprint    (1000) oprint    (1000)        0 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/server/proto/__init__.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2229 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/server/proto/jobs_pb2.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     3849 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/server/proto/peers_pb2.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     1664 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/server/proto/state_pb2.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)        0 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/server/proto/test.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2590 2022-08-25 19:29:48.000000 peerprint-0.2.0/peerprint/shell.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     9477 2022-09-03 16:19:30.000000 peerprint-0.2.0/peerprint/sync_objects.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2724 2022-09-03 16:19:30.000000 peerprint-0.2.0/peerprint/sync_objects_test.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)       22 2022-11-18 15:42:11.000000 peerprint-0.2.0/peerprint/version.py
-drwxr-xr-x   0 oprint    (1000) oprint    (1000)        0 2022-11-18 15:45:15.000000 peerprint-0.2.0/peerprint/wan/
--rw-r--r--   0 oprint    (1000) oprint    (1000)        0 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/__init__.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2955 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/comms.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     3390 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/comms_test.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     3671 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/demo.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     3101 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/ipfs.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2837 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/ipfs_test.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2593 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/proc.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2095 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/proc_test.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2955 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/registry.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     1069 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/registry_test.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     4677 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/wan_queue.py
--rw-r--r--   0 oprint    (1000) oprint    (1000)     2488 2022-11-11 03:04:57.000000 peerprint-0.2.0/peerprint/wan/wan_queue_test.py
-drwxr-xr-x   0 oprint    (1000) oprint    (1000)        0 2022-11-18 15:45:15.000000 peerprint-0.2.0/peerprint.egg-info/
--rw-r--r--   0 oprint    (1000) oprint    (1000)     3152 2022-11-18 15:45:14.000000 peerprint-0.2.0/peerprint.egg-info/PKG-INFO
--rw-r--r--   0 oprint    (1000) oprint    (1000)      969 2022-11-18 15:45:15.000000 peerprint-0.2.0/peerprint.egg-info/SOURCES.txt
--rw-r--r--   0 oprint    (1000) oprint    (1000)        1 2022-11-18 15:45:14.000000 peerprint-0.2.0/peerprint.egg-info/dependency_links.txt
--rw-r--r--   0 oprint    (1000) oprint    (1000)       96 2022-11-18 15:45:14.000000 peerprint-0.2.0/peerprint.egg-info/requires.txt
--rw-r--r--   0 oprint    (1000) oprint    (1000)       10 2022-11-18 15:45:14.000000 peerprint-0.2.0/peerprint.egg-info/top_level.txt
--rw-r--r--   0 oprint    (1000) oprint    (1000)       85 2022-08-25 19:29:48.000000 peerprint-0.2.0/pyproject.toml
--rw-r--r--   0 oprint    (1000) oprint    (1000)      808 2022-11-18 15:45:15.000000 peerprint-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:23:42.000000 peerprint-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-09-06 19:45:34.000000 peerprint-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3132 2023-04-14 21:23:42.000000 peerprint-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-01-31 21:26:13.000000 peerprint-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-06 19:45:34.000000 peerprint-0.3.0/peerprint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7213 2023-04-14 21:13:51.000000 peerprint-0.3.0/peerprint/client.py
+-rw-r--r--   0 root         (0) root         (0)     5593 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/comms.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/comms_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      353 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/data/psk_gen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint/example/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/example/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3609 2023-04-13 13:33:44.000000 peerprint-0.3.0/peerprint/example/main.py
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/filesharing.py
+-rw-r--r--   0 root         (0) root         (0)     4922 2023-01-31 21:26:13.000000 peerprint-0.3.0/peerprint/filesharing_test.py
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/ipfs.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/ipfs_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint/pkg/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/pkg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint/pkg/proto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/pkg/proto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7531 2023-04-10 13:35:41.000000 peerprint-0.3.0/peerprint/pkg/proto/command_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27766 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/pkg/proto/command_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3685 2023-04-10 13:35:41.000000 peerprint-0.3.0/peerprint/pkg/proto/peers_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/pkg/proto/state_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-04-13 13:31:40.000000 peerprint-0.3.0/peerprint/proc.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/proc_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/scripts/cert_gen.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/scripts/psk_gen.py
+-rw-r--r--   0 root         (0) root         (0)    10768 2023-03-10 00:28:43.000000 peerprint-0.3.0/peerprint/scripts/trust_sim.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-04-13 13:32:34.000000 peerprint-0.3.0/peerprint/server.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-04-14 21:18:05.000000 peerprint-0.3.0/peerprint/server_test.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 21:23:24.000000 peerprint-0.3.0/peerprint/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3132 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      922 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-14 21:23:42.000000 peerprint-0.3.0/peerprint.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2022-09-06 19:45:34.000000 peerprint-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      735 2023-04-14 21:23:42.000000 peerprint-0.3.0/setup.cfg
```

### Comparing `peerprint-0.2.0/LICENSE` & `peerprint-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peerprint-0.2.0/PKG-INFO` & `peerprint-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: peerprint
-Version: 0.2.0
+Version: 0.3.0
 Summary: Peer-to-peer networked 3d printing
 Home-page: https://github.com/smartin015/peerprint
 Author: Scott Martin
 Author-email: smartin015+peerprint@gmali.com
 Project-URL: Bug Tracker, https://github.com/smartin015/peerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: DEV
 License-File: LICENSE
 
 # PeerPrint
 
 ![build status](https://img.shields.io/travis/smartin015/peerprint/main?style=plastic)
 
 **PeerPrint is a framework for sharing 3D printing tasks across a peer-to-peer network of 3D printers.**
```

### Comparing `peerprint-0.2.0/README.md` & `peerprint-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `peerprint-0.2.0/peerprint/filesharing_test.py` & `peerprint-0.3.0/peerprint/filesharing_test.py`

 * *Files identical despite different names*

### Comparing `peerprint-0.2.0/peerprint/server/proto/jobs_pb2.py` & `peerprint-0.3.0/peerprint/pkg/proto/peers_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: proto/jobs.proto
+# source: peers.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10proto/jobs.proto\x12\x04jobs\"%\n\x04Lock\x12\x0c\n\x04peer\x18\x01 \x01(\t\x12\x0f\n\x07\x63reated\x18\x02 \x01(\x04\"Z\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12\x18\n\x04lock\x18\x03 \x01(\x0b\x32\n.jobs.Lock\x12\x10\n\x08protocol\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"\x10\n\x0eGetJobsRequest\"\'\n\rSetJobRequest\x12\x16\n\x03job\x18\x01 \x01(\x0b\x32\t.jobs.Job\"\x1e\n\x10\x44\x65leteJobRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x1f\n\x11\x41\x63quireJobRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x1f\n\x11ReleaseJobRequest\x12\n\n\x02id\x18\x01 \x01(\t\".\n\x13JobMutationResponse\x12\x17\n\x04jobs\x18\x01 \x03(\x0b\x32\t.jobs.JobB.Z,github.com/smartin015/peerprint/pubsub/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bpeers.proto\x12\x05peers\"/\n\x08Location\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\"@\n\nPeerStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x07\x63lients\x18\x02 \x03(\x0b\x32\x13.peers.ClientStatus\"\x9f\x01\n\x0c\x43lientStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\ractive_record\x18\x02 \x01(\t\x12\x13\n\x0b\x61\x63tive_unit\x18\x03 \x01(\t\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x0f\n\x07profile\x18\x05 \x01(\t\x12!\n\x08location\x18\x06 \x01(\x0b\x32\x0f.peers.Location\x12\x11\n\ttimestamp\x18\x07 \x01(\x03\"%\n\x08\x41\x64\x64rInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05\x61\x64\x64rs\x18\x02 \x03(\t\"\x11\n\x0fGetPeersRequest\"6\n\x10GetPeersResponse\x12\"\n\tAddresses\x18\x01 \x03(\x0b\x32\x0f.peers.AddrInfo\"\x12\n\x10GetStatusRequest\"\xdf\x01\n\rNetworkConfig\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\r\n\x05links\x18\x05 \x03(\t\x12\x10\n\x08location\x18\x06 \x01(\t\x12\x12\n\nrendezvous\x18\x07 \x01(\t\x12\x0f\n\x07\x63reator\x18\t \x01(\t\x12\x0f\n\x07\x63reated\x18\n \x01(\x03\x12\x1d\n\x15\x65xtra_bootstrap_peers\x18\x0b \x03(\t\x12\x19\n\x11\x65xtra_relay_peers\x18\x0c \x03(\t\"\x85\x01\n\x0cNetworkStats\x12\x12\n\npopulation\x18\x01 \x01(\x03\x12\x1d\n\x15\x63ompletions_last7days\x18\x02 \x01(\x03\x12\x0f\n\x07records\x18\x03 \x01(\x03\x12\x14\n\x0cidle_records\x18\x04 \x01(\x03\x12\x1b\n\x13\x61vg_completion_time\x18\x05 \x01(\x03\"f\n\x07Network\x12$\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x14.peers.NetworkConfig\x12\x11\n\tsignature\x18\x02 \x01(\x0c\x12\"\n\x05stats\x18\x03 \x01(\x0b\x32\x13.peers.NetworkStats\".\n\x0ePubKeyExchange\x12\x0e\n\x06pubkey\x18\x01 \x01(\x0c\x12\x0c\n\x04salt\x18\x02 \x01(\x0c\"!\n\x0c\x45ncryptedPSK\x12\x11\n\tencrypted\x18\x01 \x01(\x0c\x42.Z,github.com/smartin015/peerprint/pubsub/protob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.jobs_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'peers_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z,github.com/smartin015/peerprint/pubsub/proto'
-  _LOCK._serialized_start=26
-  _LOCK._serialized_end=63
-  _JOB._serialized_start=65
-  _JOB._serialized_end=155
-  _GETJOBSREQUEST._serialized_start=157
-  _GETJOBSREQUEST._serialized_end=173
-  _SETJOBREQUEST._serialized_start=175
-  _SETJOBREQUEST._serialized_end=214
-  _DELETEJOBREQUEST._serialized_start=216
-  _DELETEJOBREQUEST._serialized_end=246
-  _ACQUIREJOBREQUEST._serialized_start=248
-  _ACQUIREJOBREQUEST._serialized_end=279
-  _RELEASEJOBREQUEST._serialized_start=281
-  _RELEASEJOBREQUEST._serialized_end=312
-  _JOBMUTATIONRESPONSE._serialized_start=314
-  _JOBMUTATIONRESPONSE._serialized_end=360
+  _LOCATION._serialized_start=22
+  _LOCATION._serialized_end=69
+  _PEERSTATUS._serialized_start=71
+  _PEERSTATUS._serialized_end=135
+  _CLIENTSTATUS._serialized_start=138
+  _CLIENTSTATUS._serialized_end=297
+  _ADDRINFO._serialized_start=299
+  _ADDRINFO._serialized_end=336
+  _GETPEERSREQUEST._serialized_start=338
+  _GETPEERSREQUEST._serialized_end=355
+  _GETPEERSRESPONSE._serialized_start=357
+  _GETPEERSRESPONSE._serialized_end=411
+  _GETSTATUSREQUEST._serialized_start=413
+  _GETSTATUSREQUEST._serialized_end=431
+  _NETWORKCONFIG._serialized_start=434
+  _NETWORKCONFIG._serialized_end=657
+  _NETWORKSTATS._serialized_start=660
+  _NETWORKSTATS._serialized_end=793
+  _NETWORK._serialized_start=795
+  _NETWORK._serialized_end=897
+  _PUBKEYEXCHANGE._serialized_start=899
+  _PUBKEYEXCHANGE._serialized_end=945
+  _ENCRYPTEDPSK._serialized_start=947
+  _ENCRYPTEDPSK._serialized_end=980
 # @@protoc_insertion_point(module_scope)
```

### Comparing `peerprint-0.2.0/peerprint/wan/comms_test.py` & `peerprint-0.3.0/peerprint/comms_test.py`

 * *Files identical despite different names*

### Comparing `peerprint-0.2.0/peerprint/wan/ipfs.py` & `peerprint-0.3.0/peerprint/ipfs.py`

 * *Files identical despite different names*

### Comparing `peerprint-0.2.0/peerprint/wan/ipfs_test.py` & `peerprint-0.3.0/peerprint/ipfs_test.py`

 * *Files identical despite different names*

### Comparing `peerprint-0.2.0/peerprint/wan/proc.py` & `peerprint-0.3.0/peerprint/proc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,72 @@
 import subprocess
-import atexit
 import signal
+import asyncio
 from dataclasses import dataclass, fields
 
-@dataclass
-class ServerProcessOpts():
-    # See ../server/main.go for flag defs and defaults
-    addr: str = None
-    raftAddr: str = None
-    raftPath: str = None
-    rendezvous: str = None
-    trustedPeers: str = None
-    queue: str = None
-    ipfs_server: str = None
-    local: bool = None
-    privkeyfile: str = None
-    pubkeyfile: str = None
-    connectTimeout: str = None
-    zmq: str = None
-    zmqpush: str = None
-    zmqlog: str = None
-
+class ProcessOptsBase():
     def render(self, binary_path):
         args = [binary_path]
         for field in fields(self):
             val = getattr(self, field.name)
             if val is not None:
                 args.append(f"-{field.name}={val}")
         return args
 
-class DependentProcess:
-    def __init__(self):
-        atexit.register(self.destroy)
-
-    def _signal(self, sig, timeout=5):
-        self._proc.send_signal(sig)
-        try:
-            self._proc.wait(timeout)
-        except subprocess.TimeoutExpired:
-            pass
-        return self._proc.returncode is not None
-
-    def destroy(self):
-        atexit.unregister(self.destroy)
-
-        if getattr(self, "_proc", None) is None or self._proc.returncode is not None:
-            return
-        self._logger.info(f"PID {self._proc.pid} (SIGINT)")
-        if self._signal(signal.SIGINT):
-            return
-
-        self._logger.info(f"PID {self._proc.pid} (SIGKILL)")
-        if self._signal(signal.SIGKILL):
-            return
+@dataclass
+class ServerProcessOpts(ProcessOptsBase):
+    # See cmd/server/main.go for flag defs and defaults
+    baseDir: str = None
+    addr: str = None
+    certsDir: str = None
+    connDir: str = None
+    driverCfg: str = None
+    rootCert: str = None
+    regDBLocal: str = None
+    regDBWorld: str = None
+    serverCert: str = None
+    serverKey: str = None
+    www: str = None
+    wwwCfg: str = None
+    wwwDir: str = None
 
-        self._logger.info(f"PID {self._proc.pid} (SIGTERM)")
-        self._signal(signal.SIGTERM, timeout=None)
 
-class IPFSDaemonProcess(DependentProcess):
+class IPFSDaemonProcess():
     def __init__(self, logger):
         self._logger = logger
         if self.is_running():
             self._logger.warning("IPFS daemon already running; skipping daemon creation")
             self._proc = None
         else:
-            self._proc = subprocess.Popen(["ipfs", "daemon", "--init", "--enable-pubsub-experiment"])
+            self._proc = subprocess.Popen(("ipfs", "daemon", "--init", "--enable-pubsub-experiment"))
             self._logger.info("Launched IPFS daemon")
-        super().__init__()
 
     def is_running(self):
-        p = subprocess.Popen(["ipfs", "stats", "bw"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        p = subprocess.Popen(("ipfs", "stats", "bw"), stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         p.communicate()
         return (p.returncode == 0)
 
 
-class ServerProcess(DependentProcess):
+class ServerProcess():
     def __init__(self, opts, binary_path, logger):
         self._logger = logger
         args = opts.render(binary_path)
         self._proc = subprocess.Popen(args)
-        self._logger.debug(f"Launch: {args}")
+        self._logger.debug(f"Launch: {' '.join(args)}")
+
+    def _signal(self, sig, timeout=1):
+        if getattr(self, "_proc", None) is None or self._proc.returncode is not None:
+            return True
+        self._logger.info(f"SIGNAL PID {self._proc.pid} ({sig})")
+        self._proc.send_signal(sig)
+        try:
+            self._proc.wait(timeout)
+        except subprocess.TimeoutExpired:
+            pass
+        rc = self._proc.returncode
+        return rc is not None
 
-    def is_ready(self):
+    def destroy(self):
+        return self._signal(signal.SIGINT) or self._signal(signal.SIGKILL) or self._signal(signal.SIGTERM) 
+
+    def is_running(self):
         return self._proc.returncode is None
```

### Comparing `peerprint-0.2.0/peerprint/wan/proc_test.py` & `peerprint-0.3.0/peerprint/proc_test.py`

 * *Files identical despite different names*

### Comparing `peerprint-0.2.0/peerprint.egg-info/PKG-INFO` & `peerprint-0.3.0/peerprint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: peerprint
-Version: 0.2.0
+Version: 0.3.0
 Summary: Peer-to-peer networked 3d printing
 Home-page: https://github.com/smartin015/peerprint
 Author: Scott Martin
 Author-email: smartin015+peerprint@gmali.com
 Project-URL: Bug Tracker, https://github.com/smartin015/peerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: DEV
 License-File: LICENSE
 
 # PeerPrint
 
 ![build status](https://img.shields.io/travis/smartin015/peerprint/main?style=plastic)
 
 **PeerPrint is a framework for sharing 3D printing tasks across a peer-to-peer network of 3D printers.**
```

### Comparing `peerprint-0.2.0/setup.cfg` & `peerprint-0.3.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -14,22 +14,17 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	pysyncobj==0.3.10
-	pyzmq==24.0.1
+	grpcio==1.51.1
 	protobuf==4.21.8
-	requests>=2.2
-	pyyaml==6.0
-
-[options.extras_require]
-DEV = pyzmq>=22.3.0
+	pyopenssl>=23.0.0
 
 [options.packages.find]
 exclude = *_test
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

