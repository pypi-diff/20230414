# Comparing `tmp/router_log_preprocessor-0.1.3.tar.gz` & `tmp/router_log_preprocessor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "router_log_preprocessor-0.1.3.tar", max compression
+gzip compressed data, was "router_log_preprocessor-0.1.4.tar", max compression
```

## Comparing `router_log_preprocessor-0.1.3.tar` & `router_log_preprocessor-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.3/LICENSE
--rw-r--r--   0        0        0     8920 2023-04-13 12:24:43.831463 router_log_preprocessor-0.1.3/README.md
--rw-r--r--   0        0        0      794 2023-04-14 08:30:46.328283 router_log_preprocessor-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.3/router_log_preprocessor/__init__.py
--rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.3/router_log_preprocessor/__main__.py
--rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__init__.py
--rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
--rw-r--r--   0        0        0     1317 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
--rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_dnsmasq_dhcp.py
--rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_message.py
--rw-r--r--   0        0        0     1536 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_wlc.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__init__.py
--rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
--rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/abc.py
--rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__init__.py
--rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
--rw-r--r--   0        0        0     1907 2023-04-13 12:48:57.905739 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
--rw-r--r--   0        0        0     4217 2023-04-13 12:50:18.950272 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
--rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_known_clients.py
--rw-r--r--   0        0        0     2654 2023-04-13 12:48:56.785731 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_mapper.py
--rw-r--r--   0        0        0     5820 2023-04-13 12:50:17.498262 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_trapper.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__init__.py
--rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
--rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
--rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/handler.py
--rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/server.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__init__.py
--rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
--rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
--rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
--rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/typing.py
--rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/wlc.py
--rw-r--r--   0        0        0     2327 2023-04-05 19:10:32.809547 router_log_preprocessor-0.1.3/router_log_preprocessor/settings.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/util/__init__.py
--rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
--rw-r--r--   0        0        0     3026 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
--rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/util/logging.py
--rw-r--r--   0        0        0     3588 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/util/rfc3164_parser.py
--rw-r--r--   0        0        0    10333 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.3/setup.py
--rw-r--r--   0        0        0     9790 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.4/LICENSE
+-rw-r--r--   0        0        0     8920 2023-04-13 12:24:43.831463 router_log_preprocessor-0.1.4/README.md
+-rw-r--r--   0        0        0      794 2023-04-14 18:52:31.036646 router_log_preprocessor-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.4/router_log_preprocessor/__init__.py
+-rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.4/router_log_preprocessor/__main__.py
+-rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
+-rw-r--r--   0        0        0     1317 2023-04-14 18:44:34.268234 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
+-rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_dnsmasq_dhcp.py
+-rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_message.py
+-rw-r--r--   0        0        0     1560 2023-04-14 18:44:28.564220 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_wlc.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
+-rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/abc.py
+-rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
+-rw-r--r--   0        0        0     1898 2023-04-14 18:44:34.272234 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
+-rw-r--r--   0        0        0     4217 2023-04-13 12:50:18.950272 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
+-rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_known_clients.py
+-rw-r--r--   0        0        0     2644 2023-04-14 18:44:28.588220 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_mapper.py
+-rw-r--r--   0        0        0     5820 2023-04-13 12:50:17.498262 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_trapper.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
+-rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
+-rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/handler.py
+-rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/server.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
+-rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
+-rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
+-rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/typing.py
+-rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/wlc.py
+-rw-r--r--   0        0        0     2327 2023-04-05 19:10:32.809547 router_log_preprocessor-0.1.4/router_log_preprocessor/settings.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/util/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
+-rw-r--r--   0        0        0     3026 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
+-rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/util/logging.py
+-rw-r--r--   0        0        0     3588 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/util/rfc3164_parser.py
+-rw-r--r--   0        0        0    10333 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.4/setup.py
+-rw-r--r--   0        0        0     9790 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.4/PKG-INFO
```

### Comparing `router_log_preprocessor-0.1.3/LICENSE` & `router_log_preprocessor-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/README.md` & `router_log_preprocessor-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/pyproject.toml` & `router_log_preprocessor-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "router-log-preprocessor"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 repository = "https://github.com/mastdi/router-log-preprocessor"
 authors = ["Martin Storgaard Dieu <martin@storgaarddieu.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "router_log_preprocessor"}]
```

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/__init__.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/__main__.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/__main__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__init__.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_message.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_message.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_wlc.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_wlc.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import pydantic.dataclasses
 
 from router_log_preprocessor.domain._message import Message
 
 
 class WlcEvent(enum.Enum):
     DISASSOCIATION = 0
-    DEAUTH_IND = 1
-    AUTHENTICATE = 2
-    ASSOCIATION = 3
-    REASSOCIATION = 4
+    DEAUTH_IND = 1000000
+    AUTHENTICATE = 2000000
+    ASSOCIATION = 3000000
+    REASSOCIATION = 4000000
 
     @classmethod
     def from_event(cls, event: str) -> "WlcEvent":
         event = event.lstrip().lower()
         if event.startswith("disassoc"):
             return cls.DISASSOCIATION
         if event.startswith("deauth_ind"):
```

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__init__.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/abc.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/abc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__init__.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 13 12:48:56 2023 UTC, .py size: 2654 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,120 +1,119 @@
-00000000: 550d 0d0a 0000 0000 38fa 3764 5e0a 0000  U.......8.7d^...
+00000000: 550d 0d0a 0000 0000 0c9f 3964 540a 0000  U.........9dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 6d07 5a07 0100 6400 6401 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 0200 0100 6d0a 0200 0100 6d0b 5a0b  m.....m.....m.Z.
 00000080: 0100 6507 6a0c 6507 6a0d 6504 6a0e 6505  ..e.j.e.j.e.j.e.
 00000090: 6a0f 6401 6401 6603 1900 6402 9c03 6403  j.d.d.f...d...d.
 000000a0: 6404 8404 5a10 6507 6a0c 650b 6a11 6505  d...Z.e.j.e.j.e.
 000000b0: 6a12 6405 9c03 6406 6407 8404 5a13 6401  j.d...d.d...Z.d.
 000000c0: 5300 2908 e900 0000 004e 2903 da06 7265  S.)......N)...re
 000000d0: 636f 7264 da07 6d65 7373 6167 65da 0672  cord..message..r
 000000e0: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
-000000f0: 0000 0800 0000 0a00 0000 6300 0000 73d8  ..........c...s.
+000000f0: 0000 0800 0000 0a00 0000 6300 0000 73d4  ..........c...s.
 00000100: 0000 007c 006a 0064 006b 0973 0e74 0182  ...|.j.d.k.s.t..
 00000110: 017c 006a 00a0 02a1 00a0 0364 0164 02a1  .|.j.......d.d..
 00000120: 027d 0274 047c 006a 05a0 05a1 0083 017d  .}.t.|.j.......}
 00000130: 0364 007d 0474 067c 0174 076a 0883 0272  .d.}.t.|.t.j...r
-00000140: 4a7c 016a 096a 0a64 0314 007d 0474 0ba0  J|.j.j.d...}.t..
-00000150: 0c7c 01a1 017d 057c 0544 005d 7a7d 067c  .|...}.|.D.]z}.|
-00000160: 066a 0d64 046b 0272 6871 5874 0e7c 017c  .j.d.k.rhqXt.|.|
-00000170: 066a 0d83 027d 0774 067c 0774 0f6a 1083  .j...}.t.|.t.j..
-00000180: 0272 887c 076a 0a7d 076e 1a74 067c 0774  .r.|.j.}.n.t.|.t
-00000190: 116a 1274 116a 1366 0283 0272 a274 147c  .j.t.j.f...r.t.|
-000001a0: 0783 017d 0774 156a 167c 006a 1764 057c  ...}.t.j.|.j.d.|
-000001b0: 029b 0064 067c 066a 0d9b 0064 077c 016a  ...d.|.j...d.|.j
-000001c0: 189b 0064 089d 077c 077c 037c 0464 098d  ...d...|.|.|.d..
-000001d0: 0556 0001 0071 5864 0053 0029 0a4e fa01  .V...qXd.S.).N..
-000001e0: 2dda 015f 6940 420f 00da 0b6d 6163 5f61  -.._i@B....mac_a
-000001f0: 6464 7265 7373 7a04 726c 702e fa01 5bfa  ddressz.rlp...[.
-00000200: 012c fa01 5d29 05da 0468 6f73 74da 036b  .,..])...host..k
-00000210: 6579 da05 7661 6c75 65da 0563 6c6f 636b  ey..value..clock
-00000220: da02 6e73 2919 da07 7072 6f63 6573 73da  ..ns)...process.
-00000230: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
-00000240: 056c 6f77 6572 da07 7265 706c 6163 65da  .lower..replace.
-00000250: 0369 6e74 da09 7469 6d65 7374 616d 70da  .int..timestamp.
-00000260: 0a69 7369 6e73 7461 6e63 65da 0664 6f6d  .isinstance..dom
-00000270: 6169 6eda 0d57 6c63 4576 656e 744d 6f64  ain..WlcEventMod
-00000280: 656c da05 6576 656e 7472 0d00 0000 da0b  el..eventr......
-00000290: 6461 7461 636c 6173 7365 73da 0666 6965  dataclasses..fie
-000002a0: 6c64 73da 046e 616d 65da 0767 6574 6174  lds..name..getat
-000002b0: 7472 da04 656e 756d da04 456e 756d da09  tr..enum..Enum..
-000002c0: 6970 6164 6472 6573 73da 0b49 5076 3441  ipaddress..IPv4A
-000002d0: 6464 7265 7373 da0b 4950 7636 4164 6472  ddress..IPv6Addr
-000002e0: 6573 73da 0373 7472 da15 6173 796e 6369  ess..str..asynci
-000002f0: 6f5f 7a61 6262 6978 5f73 656e 6465 72da  o_zabbix_sender.
-00000300: 0b4d 6561 7375 7265 6d65 6e74 da08 686f  .Measurement..ho
-00000310: 7374 6e61 6d65 7207 0000 0029 0872 0200  stnamer....).r..
-00000320: 0000 7203 0000 0072 1000 0000 720e 0000  ..r....r....r...
-00000330: 0072 0f00 0000 5a0c 6d6f 6465 6c5f 6669  .r....Z.model_fi
-00000340: 656c 6473 da05 6669 656c 6472 0d00 0000  elds..fieldr....
-00000350: a900 7228 0000 00fa 692f 686f 6d65 2f6d  ..r(....i/home/m
-00000360: 7973 2f44 6f63 756d 656e 7473 2f47 6974  ys/Documents/Git
-00000370: 4875 622f 6d61 7374 6469 2f72 6f75 7465  Hub/mastdi/route
-00000380: 722d 6c6f 672d 7072 6570 726f 6365 7373  r-log-preprocess
-00000390: 6f72 2f72 6f75 7465 725f 6c6f 675f 7072  or/router_log_pr
-000003a0: 6570 726f 6365 7373 6f72 2f68 6f6f 6b73  eprocessor/hooks
-000003b0: 2f7a 6162 6269 782f 5f6d 6170 7065 722e  /zabbix/_mapper.
-000003c0: 7079 da12 6d61 705f 636c 6965 6e74 5f6d  py..map_client_m
-000003d0: 6573 7361 6765 1a00 0000 732c 0000 0000  essage....s,....
-000003e0: 030e 0312 020e 0104 010c 010c 030a 0108  ................
-000003f0: 010a 0102 010c 010c 0108 0112 0108 0104  ................
-00000400: 0104 011a 0102 0102 0102 fb72 2a00 0000  ...........r*...
-00000410: 2903 7202 0000 00da 0d6b 6e6f 776e 5f63  ).r......known_c
-00000420: 6c69 656e 7473 7204 0000 0063 0200 0000  lientsr....c....
-00000430: 0000 0000 0000 0000 0300 0000 0900 0000  ................
-00000440: 4300 0000 7364 0000 007c 006a 0064 006b  C...sd...|.j.d.k
-00000450: 0973 0e74 0182 0174 026a 0364 0164 0284  .s.t...t.j.d.d..
-00000460: 007c 01a0 047c 006a 00a1 0144 0083 0164  .|...|.j...D...d
-00000470: 0064 0364 048d 037d 0274 05a0 0674 056a  .d.d...}.t...t.j
-00000480: 077c 006a 0864 057c 006a 00a0 09a1 009b  .|.j.d.|.j......
-00000490: 0064 069d 037c 0274 0a7c 006a 0ba0 0ba1  .d...|.t.|.j....
-000004a0: 0083 0164 078d 0467 01a1 0153 0029 084e  ...d...g...S.).N
-000004b0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000004c0: 0005 0000 0053 0000 0073 1800 0000 6700  .....S...s....g.
-000004d0: 7c00 5d10 7d01 6400 7400 7c01 8301 6901  |.].}.d.t.|...i.
-000004e0: 9102 7104 5300 2901 da03 6d61 6329 0172  ..q.S.)...mac).r
-000004f0: 2300 0000 2902 da02 2e30 722c 0000 0072  #...)....0r,...r
-00000500: 2800 0000 7228 0000 0072 2900 0000 da0a  (...r(...r).....
-00000510: 3c6c 6973 7463 6f6d 703e 3f00 0000 7304  <listcomp>?...s.
-00000520: 0000 0006 0002 007a 286d 6170 5f63 6c69  .......z(map_cli
-00000530: 656e 745f 6469 7363 6f76 6572 792e 3c6c  ent_discovery.<l
-00000540: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000550: 3e29 0272 0900 0000 fa01 3a29 02da 0669  >).r......:)...i
-00000560: 6e64 656e 74da 0a73 6570 6172 6174 6f72  ndent..separator
-00000570: 737a 1572 6c70 2e63 6c69 656e 745f 6469  sz.rlp.client_di
-00000580: 7363 6f76 6572 795b 720a 0000 0029 0472  scovery[r....).r
-00000590: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
-000005a0: 0000 0029 0c72 1000 0000 7211 0000 00da  ...).r....r.....
-000005b0: 046a 736f 6eda 0564 756d 7073 da07 636c  .json..dumps..cl
-000005c0: 6965 6e74 7372 2400 0000 da0c 4d65 6173  ientsr$.....Meas
-000005d0: 7572 656d 656e 7473 7225 0000 0072 2600  urementsr%...r&.
-000005e0: 0000 7212 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000005f0: 0029 0372 0200 0000 722b 0000 0072 0d00  .).r....r+...r..
-00000600: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
-00000610: 00da 146d 6170 5f63 6c69 656e 745f 6469  ...map_client_di
-00000620: 7363 6f76 6572 793a 0000 0073 1c00 0000  scovery:...s....
-00000630: 0003 0e01 0401 1401 0201 02fd 0605 0401  ................
-00000640: 0401 0401 1001 0201 0cfc 04ff 7236 0000  ............r6..
-00000650: 0029 1472 1a00 0000 721e 0000 0072 2000  .).r....r....r .
-00000660: 0000 7232 0000 00da 0674 7970 696e 6772  ..r2.....typingr
-00000670: 2400 0000 da1e 726f 7574 6572 5f6c 6f67  $.....router_log
-00000680: 5f70 7265 7072 6f63 6573 736f 722e 646f  _preprocessor.do
-00000690: 6d61 696e 7217 0000 00da 3372 6f75 7465  mainr.....3route
-000006a0: 725f 6c6f 675f 7072 6570 726f 6365 7373  r_log_preprocess
-000006b0: 6f72 2e68 6f6f 6b73 2e7a 6162 6269 782e  or.hooks.zabbix.
-000006c0: 5f6b 6e6f 776e 5f63 6c69 656e 7473 da05  _known_clients..
-000006d0: 686f 6f6b 73da 067a 6162 6269 78da 0e5f  hooks..zabbix.._
-000006e0: 6b6e 6f77 6e5f 636c 6965 6e74 73da 094c  known_clients..L
-000006f0: 6f67 5265 636f 7264 da07 4d65 7373 6167  ogRecord..Messag
-00000700: 65da 0947 656e 6572 6174 6f72 7225 0000  e..Generatorr%..
-00000710: 0072 2a00 0000 da0c 4b6e 6f77 6e43 6c69  .r*.....KnownCli
-00000720: 656e 7473 7235 0000 0072 3600 0000 7228  entsr5...r6...r(
-00000730: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
-00000740: 0000 da08 3c6d 6f64 756c 653e 0e00 0000  ....<module>....
-00000750: 731e 0000 0008 0108 0108 0108 0108 0208  s...............
-00000760: 020c 0118 0404 0004 0110 fe0c 2104 0004  ............!...
-00000770: 0104 fe                                  ...
+00000140: 467c 016a 096a 0a7d 0474 0ba0 0c7c 01a1  F|.j.j.}.t...|..
+00000150: 017d 057c 0544 005d 7a7d 067c 066a 0d64  .}.|.D.]z}.|.j.d
+00000160: 036b 0272 6471 5474 0e7c 017c 066a 0d83  .k.rdqTt.|.|.j..
+00000170: 027d 0774 067c 0774 0f6a 1083 0272 847c  .}.t.|.t.j...r.|
+00000180: 076a 0a7d 076e 1a74 067c 0774 116a 1274  .j.}.n.t.|.t.j.t
+00000190: 116a 1366 0283 0272 9e74 147c 0783 017d  .j.f...r.t.|...}
+000001a0: 0774 156a 167c 006a 1764 047c 029b 0064  .t.j.|.j.d.|...d
+000001b0: 057c 066a 0d9b 0064 067c 016a 189b 0064  .|.j...d.|.j...d
+000001c0: 079d 077c 077c 037c 0464 088d 0556 0001  ...|.|.|.d...V..
+000001d0: 0071 5464 0053 0029 094e fa01 2dda 015f  .qTd.S.).N..-.._
+000001e0: da0b 6d61 635f 6164 6472 6573 737a 0472  ..mac_addressz.r
+000001f0: 6c70 2efa 015b fa01 2cfa 015d 2905 da04  lp...[..,..])...
+00000200: 686f 7374 da03 6b65 79da 0576 616c 7565  host..key..value
+00000210: da05 636c 6f63 6bda 026e 7329 19da 0770  ..clock..ns)...p
+00000220: 726f 6365 7373 da0e 4173 7365 7274 696f  rocess..Assertio
+00000230: 6e45 7272 6f72 da05 6c6f 7765 72da 0772  nError..lower..r
+00000240: 6570 6c61 6365 da03 696e 74da 0974 696d  eplace..int..tim
+00000250: 6573 7461 6d70 da0a 6973 696e 7374 616e  estamp..isinstan
+00000260: 6365 da06 646f 6d61 696e da0d 576c 6345  ce..domain..WlcE
+00000270: 7665 6e74 4d6f 6465 6cda 0565 7665 6e74  ventModel..event
+00000280: 720d 0000 00da 0b64 6174 6163 6c61 7373  r......dataclass
+00000290: 6573 da06 6669 656c 6473 da04 6e61 6d65  es..fields..name
+000002a0: da07 6765 7461 7474 72da 0465 6e75 6dda  ..getattr..enum.
+000002b0: 0445 6e75 6dda 0969 7061 6464 7265 7373  .Enum..ipaddress
+000002c0: da0b 4950 7634 4164 6472 6573 73da 0b49  ..IPv4Address..I
+000002d0: 5076 3641 6464 7265 7373 da03 7374 72da  Pv6Address..str.
+000002e0: 1561 7379 6e63 696f 5f7a 6162 6269 785f  .asyncio_zabbix_
+000002f0: 7365 6e64 6572 da0b 4d65 6173 7572 656d  sender..Measurem
+00000300: 656e 74da 0868 6f73 746e 616d 6572 0700  ent..hostnamer..
+00000310: 0000 2908 7202 0000 0072 0300 0000 7210  ..).r....r....r.
+00000320: 0000 0072 0e00 0000 720f 0000 005a 0c6d  ...r....r....Z.m
+00000330: 6f64 656c 5f66 6965 6c64 73da 0566 6965  odel_fields..fie
+00000340: 6c64 720d 0000 00a9 0072 2800 0000 fa69  ldr......r(....i
+00000350: 2f68 6f6d 652f 6d79 732f 446f 6375 6d65  /home/mys/Docume
+00000360: 6e74 732f 4769 7448 7562 2f6d 6173 7464  nts/GitHub/mastd
+00000370: 692f 726f 7574 6572 2d6c 6f67 2d70 7265  i/router-log-pre
+00000380: 7072 6f63 6573 736f 722f 726f 7574 6572  processor/router
+00000390: 5f6c 6f67 5f70 7265 7072 6f63 6573 736f  _log_preprocesso
+000003a0: 722f 686f 6f6b 732f 7a61 6262 6978 2f5f  r/hooks/zabbix/_
+000003b0: 6d61 7070 6572 2e70 79da 126d 6170 5f63  mapper.py..map_c
+000003c0: 6c69 656e 745f 6d65 7373 6167 651a 0000  lient_message...
+000003d0: 0073 2c00 0000 0003 0e03 1202 0e01 0401  .s,.............
+000003e0: 0c01 0803 0a01 0801 0a01 0201 0c01 0c01  ................
+000003f0: 0801 1201 0801 0401 0401 1a01 0201 0201  ................
+00000400: 02fb 722a 0000 0029 0372 0200 0000 da0d  ..r*...).r......
+00000410: 6b6e 6f77 6e5f 636c 6965 6e74 7372 0400  known_clientsr..
+00000420: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+00000430: 0000 0009 0000 0043 0000 0073 6400 0000  .......C...sd...
+00000440: 7c00 6a00 6400 6b09 730e 7401 8201 7402  |.j.d.k.s.t...t.
+00000450: 6a03 6401 6402 8400 7c01 a004 7c00 6a00  j.d.d...|...|.j.
+00000460: a101 4400 8301 6400 6403 6404 8d03 7d02  ..D...d.d.d...}.
+00000470: 7405 a006 7405 6a07 7c00 6a08 6405 7c00  t...t.j.|.j.d.|.
+00000480: 6a00 a009 a100 9b00 6406 9d03 7c02 740a  j.......d...|.t.
+00000490: 7c00 6a0b a00b a100 8301 6407 8d04 6701  |.j.......d...g.
+000004a0: a101 5300 2908 4e63 0100 0000 0000 0000  ..S.).Nc........
+000004b0: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+000004c0: 7318 0000 0067 007c 005d 107d 0164 0074  s....g.|.].}.d.t
+000004d0: 007c 0183 0169 0191 0271 0453 0029 01da  .|...i...q.S.)..
+000004e0: 036d 6163 2901 7223 0000 0029 02da 022e  .mac).r#...)....
+000004f0: 3072 2c00 0000 7228 0000 0072 2800 0000  0r,...r(...r(...
+00000500: 7229 0000 00da 0a3c 6c69 7374 636f 6d70  r).....<listcomp
+00000510: 3e3f 0000 0073 0400 0000 0600 0200 7a28  >?...s........z(
+00000520: 6d61 705f 636c 6965 6e74 5f64 6973 636f  map_client_disco
+00000530: 7665 7279 2e3c 6c6f 6361 6c73 3e2e 3c6c  very.<locals>.<l
+00000540: 6973 7463 6f6d 703e 2902 7209 0000 00fa  istcomp>).r.....
+00000550: 013a 2902 da06 696e 6465 6e74 da0a 7365  .:)...indent..se
+00000560: 7061 7261 746f 7273 7a15 726c 702e 636c  paratorsz.rlp.cl
+00000570: 6965 6e74 5f64 6973 636f 7665 7279 5b72  ient_discovery[r
+00000580: 0a00 0000 2904 720b 0000 0072 0c00 0000  ....).r....r....
+00000590: 720d 0000 0072 0e00 0000 290c 7210 0000  r....r....).r...
+000005a0: 0072 1100 0000 da04 6a73 6f6e da05 6475  .r......json..du
+000005b0: 6d70 73da 0763 6c69 656e 7473 7224 0000  mps..clientsr$..
+000005c0: 00da 0c4d 6561 7375 7265 6d65 6e74 7372  ...Measurementsr
+000005d0: 2500 0000 7226 0000 0072 1200 0000 7214  %...r&...r....r.
+000005e0: 0000 0072 1500 0000 2903 7202 0000 0072  ...r....).r....r
+000005f0: 2b00 0000 720d 0000 0072 2800 0000 7228  +...r....r(...r(
+00000600: 0000 0072 2900 0000 da14 6d61 705f 636c  ...r).....map_cl
+00000610: 6965 6e74 5f64 6973 636f 7665 7279 3a00  ient_discovery:.
+00000620: 0000 731c 0000 0000 030e 0104 0114 0102  ..s.............
+00000630: 0102 fd06 0504 0104 0104 0110 0102 010c  ................
+00000640: fc04 ff72 3600 0000 2914 721a 0000 0072  ...r6...).r....r
+00000650: 1e00 0000 7220 0000 0072 3200 0000 da06  ....r ...r2.....
+00000660: 7479 7069 6e67 7224 0000 00da 1e72 6f75  typingr$.....rou
+00000670: 7465 725f 6c6f 675f 7072 6570 726f 6365  ter_log_preproce
+00000680: 7373 6f72 2e64 6f6d 6169 6e72 1700 0000  ssor.domainr....
+00000690: da33 726f 7574 6572 5f6c 6f67 5f70 7265  .3router_log_pre
+000006a0: 7072 6f63 6573 736f 722e 686f 6f6b 732e  processor.hooks.
+000006b0: 7a61 6262 6978 2e5f 6b6e 6f77 6e5f 636c  zabbix._known_cl
+000006c0: 6965 6e74 73da 0568 6f6f 6b73 da06 7a61  ients..hooks..za
+000006d0: 6262 6978 da0e 5f6b 6e6f 776e 5f63 6c69  bbix.._known_cli
+000006e0: 656e 7473 da09 4c6f 6752 6563 6f72 64da  ents..LogRecord.
+000006f0: 074d 6573 7361 6765 da09 4765 6e65 7261  .Message..Genera
+00000700: 746f 7272 2500 0000 722a 0000 00da 0c4b  torr%...r*.....K
+00000710: 6e6f 776e 436c 6965 6e74 7372 3500 0000  nownClientsr5...
+00000720: 7236 0000 0072 2800 0000 7228 0000 0072  r6...r(...r(...r
+00000730: 2800 0000 7229 0000 00da 083c 6d6f 6475  (...r).....<modu
+00000740: 6c65 3e0e 0000 0073 1e00 0000 0801 0801  le>....s........
+00000750: 0801 0801 0802 0802 0c01 1804 0400 0401  ................
+00000760: 10fe 0c21 0400 0401 04fe                 ...!......
```

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_known_clients.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_known_clients.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_mapper.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_mapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     # Ensure process is formatted according to Zabbix recommendations
     process = record.process.lower().replace("-", "_")
     # Convert record datetime to timestamp in full seconds
     clock = int(record.timestamp.timestamp())
     ns = None
     if isinstance(message, domain.WlcEventModel):
-        ns = message.event.value * 1000000
+        ns = message.event.value
 
     # Generate the measurements from the model
     model_fields = dataclasses.fields(message)
     for field in model_fields:
         if field.name == "mac_address":
             continue
         value = getattr(message, field.name)
```

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_trapper.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_trapper.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__init__.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/handler.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/handler.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/server.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/server.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__init__.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/typing.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/typing.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/wlc.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/wlc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/settings.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/settings.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/util/__init__.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/util/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc` & `router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/util/logging.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/util/logging.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/router_log_preprocessor/util/rfc3164_parser.py` & `router_log_preprocessor-0.1.4/router_log_preprocessor/util/rfc3164_parser.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.3/setup.py` & `router_log_preprocessor-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 entry_points = \
 {'console_scripts': ['router-log-preprocessor = '
                      'router_log_preprocessor.__main__:main']}
 
 setup_kwargs = {
     'name': 'router-log-preprocessor',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': '# Router Log Preprocessor\n![router-log-preprocessor](https://user-images.githubusercontent.com/105678820/228938795-66dbd955-813b-4fb3-a559-4f3a41f55bb9.png)\n\n> Garbage in, garbage out\n>\n> &mdash; <cite>George Fuechsel</cite>\n\nPreprocessors upcycle garbage input data into well-structured data to ensure reliable and accurate event handling in third-party systems such as Zabbix.\nBy parsing and filtering the input log data, the preprocessor helps to ensure that only high-quality data are sent for further analysis and alerting.\nThis helps to minimize false positives and ensure that network administrators receive reliable and actionable alerts about potential security threats or other issues.\n\n\nKey features:\n- **Wireless LAN Controller event** log entries are parsed to tangible enumerations\n- **DNSMASQ DHCP** log entries are parsed to catch which IP a given client is assigned to\n- **Zabbix** templates are included to ensure that the logs are can lead to actionable alerts\n- **Extendable** preprocessors and hooks to ensure future reliable information to network administrators\n\n## Installation\n```console\n$ pip install router-log-preprocessor\n```\n\nIf needed it can also be installed from sources.\nRequires [Poetry 1.3.2](https://python-poetry.org/).\n```console\n$ git pull https://github.com/mastdi/router-log-preprocessor.git\n$ cd router-log-preprocessor\n$ poetry install\n```\n\n## Usage\nInstalling the package using pip also creates the executable script named `router-log-preprocessor`.\nOn Linux systems the router log preprocessor can be run by\n\n```console\n./router-log-preprocessor\n```\n\nThe configuration solely happens through environment variables or a `.env` configuration file located in the current working directory.\nThe most important variables are documented below. \nA full sample can be found in [.env](https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env).\nThe application reads, in order of the least priority to the highest file:\n1. `.env`,\n2. `.env.dev`,\n3. `.env.test`,\n4. `.env.staging`,\n5. `.env.prod`,\n\nmeaning that values stored in `.env.prod` will overwrite any values from other dovenv files.\nParameters stored in environment variables will always take priority over values loaded from a dotenv file.\n\n```dotenv\n# Purpose: Specifies the IP address or hostname of the local interface to which the\n# logging system should bind.\n# Format: A string containing a valid IP address or hostname, such as "192.168.0.1" or\n# "example.com".\nLOG_SERVER_HOST="0.0.0.0"\n\n# Purpose: Specifies the port number of the server to which log data should be sent.\n# Format: An integer representing a valid port number, such as 514.\nLOG_SERVER_PORT=8514\n\n# Purpose: Specifies the hostname or IP address of the Zabbix server to which the\n# Zabbix Sender should send monitoring data.\n# Format: A string containing a valid hostname or IP address, such as "example.com" or\n# "192.168.0.1".\nZABBIX_HOST="example.com"\n\n# Purpose: Specifies the port number on which the Zabbix server is running and to\n# which the Zabbix Sender should send monitoring data.\n# Format: An integer representing a valid port number, such as 10051.\nZABBIX_PORT=10051\n```\n\n## As a service\n\nThis part will go through the steps to set up the Router Log Preprocessor as a service on Ubuntu.\nThe following steps will be explained in details below:\n\n- Create a service user\n- Create a virtual environment\n- Configure environment variables\n- Set up the logging directory\n- Create the service file\n- Start the service and check its status\n- Debugging the service using journalctl\n\n### Prerequisites\n\nTo install and set up the Router Log Preprocessor as a service on Ubuntu, you will need:\n\n- Python 3.8 installed or higher\n- `venv` package (can be installed via `apt-get install python3-venv` command)\n- `pip` package manager (should be included after activating the virtual environment)\n- Internet connection to download the Router Log Preprocessor package from PyPI and the `.env` file from the GitHub repository\n\nNote that some of these prerequisites may already be installed on your Ubuntu system.\nYou can check if Python and pip are installed by running the following commands:\n\n```console\npython3 --version\npip --version\n```\n\nIf both of these commands return the version number of Python and pip, respectively, you\'re good to go.\nOtherwise, you will need to install Python and pip on your Ubuntu system before proceeding.\n\n### Creating a service user\n\nFirst, we will create a service user to run the Router Log Preprocessor.\nThis is a good security practice as running the script as a root user is not needed.\n\nRun the following commands to create a new user called `rlp`:\n\n```console\nsudo adduser rlp --disabled-password --gecos ""\nsudo su rlp\ncd ~\n```\n\nThe first command creates a new user called `rlp` with a disabled password and no additional information. \nThe second command switches to the new user and moves to their home directory.\n\n### Creating a virtual environment\n\nNow that we have a service user set up, we can create a virtual environment to install the Router Log Preprocessor.\nThe following commands create a virtual environment using Python 3.8 and install the Router Log Preprocessor package:\n\n```console\npython3 -m venv venv\ncd venv\nsource bin/activate\npip install router-log-preprocessor\n```\n\nThese commands create a new virtual environment in the venv directory, activate the environment, and install the Router Log Preprocessor package.\n\n### Configuring the environment variables \nWe will create a .env file in the virtual environment directory to store these variables.\nYou can copy the default [.env](https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env) file from the Router Log Preprocessor repository and customize it according to your needs:\n```console\ncurl -o .env https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env\nnano .env\n```\nThis will download the .env file from the Router Log Preprocessor repository and open it in the Nano text editor. \nCustomize the file to set the environment variables you need.\n\nWe are done setting up the servie user:\n\n```console\nexit\n```\n\n### Setting up the logging directory\n\nIf you have set the `LOGGING_DIRECTORY` variable in the .env file to `/var/log/rlp`, you need to create the directory and set the ownership to the rlp user:\n\n```console\nsudo mkdir /var/log/rlp\nsudo chown rlp:rlp /var/log/rlp\n```\n\nThese commands will create the `/var/log/rlp` directory and set the ownership to the `rlp` user.\n\n### Creating the service file\n\nThe next step is to create a service file for the Router Log Preprocessor.\nThis file specifies how the service should be started and managed by the system.\nCreate a new file called rlp.service in the /etc/systemd/system/ directory using the following command:\n\n```console\nsudo nano /etc/systemd/system/rlp.service\n```\n\nThis will open the text editor with a new file.\nCopy the following text into the file:\n\n```ini\n[Unit]\nDescription=Router Log Preprocessor service\nAfter=network.target\n\n[Service]\nUser=rlp\nWorkingDirectory=/home/rlp/venv\nEnvironment="PATH=/home/rlp/venv/bin"\nEnvironmentFile=/home/rlp/venv/.env\nExecStart=/home/rlp/venv/bin/router-log-preprocessor\nRestart=on-failure\nRestartSec=5s\nStartLimitInterval=60s\nStartLimitBurst=3\n\n[Install]\nWantedBy=multi-user.target\n```\n\n\n### Starting the service\n\nThe service is now ready to be started.\nThe final step is to start the service, check if it is running, and ensuring that the service starts automatically on system boot.\nStart the service using the following command:\n```console\nsudo systemctl start rlp.service\n```\n\nThis starts the service based on the configuration we just provided.\nCheck that the service is started using the following command:\n\n```console\nsudo systemctl status rlp.service\n```\n\nThis should show `active (running)` in the console.\nTo make sure the service is started on system boot use the following command:\n\n```console\nsudo systemctl enable rlp.service \n```\n\n### Debugging the service creation\n\nTo debug any issues with the service, you can use the `journalctl` command.\nFor example, to view the logs of the `rlp` service, run the following command:\n\n```console\nsudo journalctl -u rlp.service -e\n```\n\nThis will show the logs of the `rlp` service and the `-e` flag will show the end of the logs.\nYou can use other flags like `-f` to follow the logs in real-time, `-n` to specify the number of lines to show, and `-r` to show the logs in reverse order (most recent first).\n\nIf the service crashes, you can also use the `--since` and `--until` flags to show the logs between a specific time range.\nFor example, to show the logs of the last 10 minutes, run the following command:\n\n```console\nsudo journalctl -u rlp.service --since "10 minutes ago"\n```\nThis will show the logs of the `rlp` service that were generated in the last 10 minutes.\nUse this command to debug any issues with the service.',
     'author': 'Martin Storgaard Dieu',
     'author_email': 'martin@storgaarddieu.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mastdi/router-log-preprocessor',
```

### Comparing `router_log_preprocessor-0.1.3/PKG-INFO` & `router_log_preprocessor-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: router-log-preprocessor
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/mastdi/router-log-preprocessor
 License: Apache-2.0
 Author: Martin Storgaard Dieu
 Author-email: martin@storgaarddieu.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

