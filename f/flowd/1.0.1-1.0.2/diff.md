# Comparing `tmp/flowd-1.0.1.tar.gz` & `tmp/flowd-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowd-1.0.1.tar", last modified: Tue Mar 28 14:20:57 2023, max compression
+gzip compressed data, was "/root/flowd/dist/tmpn0udflfb/flowd-1.0.2.tar", last modified: Fri Apr 14 12:23:50 2023, max compression
```

## Comparing `flowd-1.0.1.tar` & `flowd-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 mbabik     (502) staff       (20)        0 2023-03-28 14:20:57.905434 flowd-1.0.1/
--rw-r--r--   0 mbabik     (502) staff       (20)      775 2023-01-23 09:33:15.000000 flowd-1.0.1/LICENSE
--rw-r--r--   0 mbabik     (502) staff       (20)       94 2022-07-26 09:55:04.000000 flowd-1.0.1/MANIFEST.in
--rw-r--r--   0 mbabik     (502) staff       (20)     1125 2023-03-28 14:20:57.905648 flowd-1.0.1/PKG-INFO
--rw-r--r--   0 mbabik     (502) staff       (20)    15186 2023-03-28 08:36:12.000000 flowd-1.0.1/README.md
-drwxr-xr-x   0 mbabik     (502) staff       (20)        0 2023-03-28 14:20:57.864069 flowd-1.0.1/etc/
--rw-r--r--   0 mbabik     (502) staff       (20)      273 2022-07-26 09:55:04.000000 flowd-1.0.1/etc/flowd.cfg
--rw-r--r--   0 mbabik     (502) staff       (20)      349 2023-03-28 08:36:12.000000 flowd-1.0.1/etc/flowd.service
--rw-r--r--   0 mbabik     (502) staff       (20)      352 2023-01-23 09:33:15.000000 flowd-1.0.1/etc/flowd@.service
-drwxr-xr-x   0 mbabik     (502) staff       (20)        0 2023-03-28 14:20:57.866904 flowd-1.0.1/flowd.egg-info/
--rw-r--r--   0 mbabik     (502) staff       (20)     1125 2023-03-28 14:20:57.000000 flowd-1.0.1/flowd.egg-info/PKG-INFO
--rw-r--r--   0 mbabik     (502) staff       (20)      807 2023-03-28 14:20:57.000000 flowd-1.0.1/flowd.egg-info/SOURCES.txt
--rw-r--r--   0 mbabik     (502) staff       (20)        1 2023-03-28 14:20:57.000000 flowd-1.0.1/flowd.egg-info/dependency_links.txt
--rw-r--r--   0 mbabik     (502) staff       (20)       55 2023-03-28 14:20:57.000000 flowd-1.0.1/flowd.egg-info/requires.txt
--rw-r--r--   0 mbabik     (502) staff       (20)        8 2023-03-28 14:20:57.000000 flowd-1.0.1/flowd.egg-info/top_level.txt
-drwxr-xr-x   0 mbabik     (502) staff       (20)        0 2023-03-28 14:20:57.867532 flowd-1.0.1/sbin/
--rwxr-xr-x   0 mbabik     (502) staff       (20)     3556 2023-03-28 08:36:12.000000 flowd-1.0.1/sbin/flowd
-drwxr-xr-x   0 mbabik     (502) staff       (20)        0 2023-03-28 14:20:57.871420 flowd-1.0.1/scitags/
--rw-r--r--   0 mbabik     (502) staff       (20)     1989 2023-03-28 09:48:37.000000 flowd-1.0.1/scitags/__init__.py
-drwxr-xr-x   0 mbabik     (502) staff       (20)        0 2023-03-28 14:20:57.875908 flowd-1.0.1/scitags/backends/
--rw-r--r--   0 mbabik     (502) staff       (20)        0 2022-07-26 09:55:04.000000 flowd-1.0.1/scitags/backends/__init__.py
--rw-r--r--   0 mbabik     (502) staff       (20)     7391 2023-01-23 12:42:19.000000 flowd-1.0.1/scitags/backends/ebpf_rhel8.py
--rw-r--r--   0 mbabik     (502) staff       (20)     6207 2023-01-23 12:39:58.000000 flowd-1.0.1/scitags/backends/ebpf_rhel9.py
--rw-r--r--   0 mbabik     (502) staff       (20)     6213 2023-01-23 09:51:55.000000 flowd-1.0.1/scitags/backends/prometheus.py
--rw-r--r--   0 mbabik     (502) staff       (20)     6201 2022-09-16 09:22:24.000000 flowd-1.0.1/scitags/backends/udp_firefly.py
--rw-r--r--   0 mbabik     (502) staff       (20)      534 2022-07-26 09:55:04.000000 flowd-1.0.1/scitags/config.py
-drwxr-xr-x   0 mbabik     (502) staff       (20)        0 2023-03-28 14:20:57.894664 flowd-1.0.1/scitags/netlink/
--rw-r--r--   0 mbabik     (502) staff       (20)        0 2023-03-28 08:07:15.000000 flowd-1.0.1/scitags/netlink/__init__.py
--rw-r--r--   0 mbabik     (502) staff       (20)     2387 2023-03-28 08:38:02.000000 flowd-1.0.1/scitags/netlink/cache.py
--rw-r--r--   0 mbabik     (502) staff       (20)     8212 2023-03-28 08:38:02.000000 flowd-1.0.1/scitags/netlink/cache_ss.py
--rw-r--r--   0 mbabik     (502) staff       (20)    12415 2022-09-16 09:22:24.000000 flowd-1.0.1/scitags/netlink/pyroute_tcp.py
-drwxr-xr-x   0 mbabik     (502) staff       (20)        0 2023-03-28 14:20:57.902020 flowd-1.0.1/scitags/plugins/
--rw-r--r--   0 mbabik     (502) staff       (20)        0 2022-07-26 09:55:04.000000 flowd-1.0.1/scitags/plugins/__init__.py
--rw-r--r--   0 mbabik     (502) staff       (20)     2783 2022-09-16 09:22:24.000000 flowd-1.0.1/scitags/plugins/firefly.py
--rw-r--r--   0 mbabik     (502) staff       (20)     6229 2023-01-23 09:33:15.000000 flowd-1.0.1/scitags/plugins/iperf.py
--rw-r--r--   0 mbabik     (502) staff       (20)     5764 2023-01-23 09:50:08.000000 flowd-1.0.1/scitags/plugins/netlink.py
--rw-r--r--   0 mbabik     (502) staff       (20)     6118 2023-01-23 09:33:07.000000 flowd-1.0.1/scitags/plugins/netstat.py
--rw-r--r--   0 mbabik     (502) staff       (20)     3060 2022-09-16 09:22:24.000000 flowd-1.0.1/scitags/plugins/np_api.py
--rw-r--r--   0 mbabik     (502) staff       (20)     8619 2023-03-28 08:46:20.000000 flowd-1.0.1/scitags/service.py
--rw-r--r--   0 mbabik     (502) staff       (20)      494 2023-01-23 09:51:35.000000 flowd-1.0.1/scitags/settings.py
-drwxr-xr-x   0 mbabik     (502) staff       (20)        0 2023-03-28 14:20:57.904519 flowd-1.0.1/scitags/stun/
--rw-r--r--   0 mbabik     (502) staff       (20)     9840 2022-07-26 09:55:04.000000 flowd-1.0.1/scitags/stun/__init__.py
--rw-r--r--   0 mbabik     (502) staff       (20)     2086 2022-07-26 09:55:04.000000 flowd-1.0.1/scitags/stun/services.py
--rw-r--r--   0 mbabik     (502) staff       (20)      103 2023-03-28 14:20:57.906515 flowd-1.0.1/setup.cfg
--rw-r--r--   0 mbabik     (502) staff       (20)     1944 2023-03-28 14:20:37.000000 flowd-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:23:50.000000 flowd-1.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:23:50.000000 flowd-1.0.2/etc/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-04-14 09:06:26.000000 flowd-1.0.2/etc/flowd.cfg
+-rw-r--r--   0 root         (0) root         (0)      349 2023-04-14 09:06:26.000000 flowd-1.0.2/etc/flowd.service
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-14 09:06:26.000000 flowd-1.0.2/etc/flowd@.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:23:50.000000 flowd-1.0.2/flowd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-04-14 12:23:50.000000 flowd-1.0.2/flowd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-04-14 12:23:50.000000 flowd-1.0.2/flowd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 12:23:50.000000 flowd-1.0.2/flowd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-14 12:23:50.000000 flowd-1.0.2/flowd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-14 12:23:50.000000 flowd-1.0.2/flowd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:23:50.000000 flowd-1.0.2/sbin/
+-rwxr-xr-x   0 root         (0) root         (0)     3200 2023-04-14 09:13:57.000000 flowd-1.0.2/sbin/flowd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:23:50.000000 flowd-1.0.2/scitags/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:23:50.000000 flowd-1.0.2/scitags/backends/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7391 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/backends/ebpf_rhel8.py
+-rw-r--r--   0 root         (0) root         (0)     6207 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/backends/ebpf_rhel9.py
+-rw-r--r--   0 root         (0) root         (0)     6213 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/backends/prometheus.py
+-rw-r--r--   0 root         (0) root         (0)     6200 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/backends/udp_firefly.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:23:50.000000 flowd-1.0.2/scitags/netlink/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/netlink/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/netlink/cache.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/netlink/cache_ss.py
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/netlink/pyroute_tcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:23:50.000000 flowd-1.0.2/scitags/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/plugins/firefly.py
+-rw-r--r--   0 root         (0) root         (0)     6229 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/plugins/iperf.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/plugins/netlink.py
+-rw-r--r--   0 root         (0) root         (0)     6118 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/plugins/netstat.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/plugins/np_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 12:23:50.000000 flowd-1.0.2/scitags/stun/
+-rw-r--r--   0 root         (0) root         (0)     9840 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/stun/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/stun/services.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-04-14 10:30:48.000000 flowd-1.0.2/scitags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/config.py
+-rw-r--r--   0 root         (0) root         (0)     8619 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/service.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-14 09:06:26.000000 flowd-1.0.2/scitags/settings.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-04-14 09:06:26.000000 flowd-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-14 09:06:26.000000 flowd-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15186 2023-04-14 09:06:26.000000 flowd-1.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-14 12:23:50.000000 flowd-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-04-14 12:22:08.000000 flowd-1.0.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-04-14 12:23:50.000000 flowd-1.0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `flowd-1.0.1/LICENSE` & `flowd-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/PKG-INFO` & `flowd-1.0.2/flowd.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: flowd
-Version: 1.0.1
+Version: 1.0.2
 Summary: Flow and Packet Marking Service
 Home-page: https://github.com/scitags/flowd
-Download-URL: https://github.com/scitags/flowd/archive/refs/tags/1.0.1.tar.gz
 Author: Marian Babik <Marian.Babik@cern.ch>, Tristan Sullivan <tssulliv@uvic.ca>
 Author-email: <net-wg-dev@cern.ch>
 License: ASL 2.0
+Download-URL: https://github.com/scitags/flowd/archive/refs/tags/1.0.2.tar.gz
 Keywords: operations python network flow packet marking
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
 License-File: LICENSE
 
 
 Flow and Packet Marking Service (flowd) implementation based on the SciTags specification (www.scitags.org).
+
+
```

### Comparing `flowd-1.0.1/README.md` & `flowd-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/flowd.egg-info/PKG-INFO` & `flowd-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: flowd
-Version: 1.0.1
+Version: 1.0.2
 Summary: Flow and Packet Marking Service
 Home-page: https://github.com/scitags/flowd
-Download-URL: https://github.com/scitags/flowd/archive/refs/tags/1.0.1.tar.gz
 Author: Marian Babik <Marian.Babik@cern.ch>, Tristan Sullivan <tssulliv@uvic.ca>
 Author-email: <net-wg-dev@cern.ch>
 License: ASL 2.0
+Download-URL: https://github.com/scitags/flowd/archive/refs/tags/1.0.2.tar.gz
 Keywords: operations python network flow packet marking
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
 License-File: LICENSE
 
 
 Flow and Packet Marking Service (flowd) implementation based on the SciTags specification (www.scitags.org).
+
+
```

### Comparing `flowd-1.0.1/flowd.egg-info/SOURCES.txt` & `flowd-1.0.2/flowd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/sbin/flowd` & `flowd-1.0.2/sbin/flowd`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 
 import logging
 import logging.handlers
 import argparse
 import os.path
 
-import systemd.journal
 import fcntl
 import sys
 
 import scitags
 import scitags.settings
 
 import socket
@@ -31,26 +30,19 @@
     if args.debug:
         log.setLevel(logging.DEBUG)
         formatter = logging.Formatter(fmt='%(asctime)s %(levelname)s %(module)s[%(process)d]: %(message)s',
                                       datefmt='%b %d %H:%M:%S')
         fh = logging.StreamHandler(stream=sys.stdout)
         fh.setFormatter(formatter)
         log.addHandler(fh)
-    elif args.fg:
-        log.setLevel(logging.INFO)
-        formatter = logging.Formatter(fmt='%(asctime)s %(levelname)s %(module)s[%(process)d]: %(message)s',
-                                      datefmt='%b %d %H:%M:%S')
-        fh = logging.StreamHandler(stream=sys.stdout)
-        fh.setFormatter(formatter)
-        log.addHandler(fh)
     else:
         log.setLevel(logging.INFO)
         formatter = logging.Formatter(fmt='%(asctime)s %(levelname)s %(module)s[%(process)d]: %(message)s',
                                       datefmt='%b %d %H:%M:%S')
-        fh = systemd.journal.JournalHandler()
+        fh = logging.StreamHandler(stream=sys.stdout)
         fh.setFormatter(formatter)
         log.addHandler(fh)
 
     if args.config:
         scitags.settings.CONFIG_PATH = args.config
 
     from scitags.config import config
```

### Comparing `flowd-1.0.1/scitags/__init__.py` & `flowd-1.0.2/scitags/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 try:
     import queue
 except ImportError:
     import Queue as queue
 
 AUTHOR = "Marian Babik <Marian.Babik@cern.ch>, Tristan Sullivan <tssulliv@uvic.ca>"
 AUTHOR_EMAIL = "<net-wg-dev@cern.ch>"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DATE = "13 Jul 2021"
 __author__ = AUTHOR
 __version__ = VERSION
 __date__ = DATE
 
 
 class FlowConfigException(Exception):
```

### Comparing `flowd-1.0.1/scitags/backends/ebpf_rhel8.py` & `flowd-1.0.2/scitags/backends/ebpf_rhel8.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/backends/ebpf_rhel9.py` & `flowd-1.0.2/scitags/backends/ebpf_rhel9.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/backends/prometheus.py` & `flowd-1.0.2/scitags/backends/prometheus.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/backends/udp_firefly.py` & `flowd-1.0.2/scitags/backends/udp_firefly.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             dst = flow_id.dst
             syslog_header = '<{}>{} {} {} {} {} {} {} '.format(SYSLOG_PRIORITY, SYSLOG_VERSION,
                                                                datetime.utcnow().isoformat() + '+00:00',
                                                                SYSLOG_HOSTNAME,
                                                                SYSLOG_APP_NAME, SYSLOG_PROCID, SYSLOG_MSGID,
                                                                SYSLOG_STRUCT_DATA)
             udp_payload = syslog_header + json.dumps(firefly_json(flow_id, flow_map, ip_config, netlink_cache))
-            log.debug(udp_payload)
+            log.info(udp_payload)
             if ':' in flow_id.dst:
                 sock6.sendto(udp_payload.encode('utf-8'), (dst, scitags.settings.UDP_FIREFLY_PORT))
             else:
                 sock4.sendto(udp_payload.encode('utf-8'), (dst, scitags.settings.UDP_FIREFLY_PORT))
             if 'UDP_FIREFLY_DST' in config.keys():
                 dst = config['UDP_FIREFLY_DST']
                 sock4.sendto(udp_payload.encode('utf-8'), (dst, scitags.settings.UDP_FIREFLY_PORT))
```

### Comparing `flowd-1.0.1/scitags/config.py` & `flowd-1.0.2/scitags/config.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/netlink/cache.py` & `flowd-1.0.2/scitags/netlink/cache.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/netlink/cache_ss.py` & `flowd-1.0.2/scitags/netlink/cache_ss.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/netlink/pyroute_tcp.py` & `flowd-1.0.2/scitags/netlink/pyroute_tcp.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/plugins/firefly.py` & `flowd-1.0.2/scitags/plugins/firefly.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/plugins/iperf.py` & `flowd-1.0.2/scitags/plugins/iperf.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/plugins/netlink.py` & `flowd-1.0.2/scitags/plugins/netlink.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/plugins/netstat.py` & `flowd-1.0.2/scitags/plugins/netstat.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/plugins/np_api.py` & `flowd-1.0.2/scitags/plugins/np_api.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/service.py` & `flowd-1.0.2/scitags/service.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/stun/__init__.py` & `flowd-1.0.2/scitags/stun/__init__.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/scitags/stun/services.py` & `flowd-1.0.2/scitags/stun/services.py`

 * *Files identical despite different names*

### Comparing `flowd-1.0.1/setup.py` & `flowd-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 AUTHOR_EMAIL = scitags.AUTHOR_EMAIL
 LICENSE = "ASL 2.0"
 PLATFORMS = "Any"
 URL = "https://github.com/scitags/flowd"
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
-    "Operating System :: POSIX :: Linux",
+    "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -44,15 +44,14 @@
                 'scitags.backends',
                 'scitags.plugins',
                 'scitags.stun',
                 'scitags.netlink'],
       install_requires=['psutil',
                         'requests',
                         'pyroute2',
-                        'systemd',
                         'prometheus_client',
                         'bcc'],
       data_files=[
           ('/usr/sbin', ['sbin/flowd']),
           ('/etc/flowd', ['etc/flowd.cfg']),
           ('/usr/lib/systemd/system', ['etc/flowd.service']),
       ])
```

