# Comparing `tmp/router_log_preprocessor-0.1.2.tar.gz` & `tmp/router_log_preprocessor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "router_log_preprocessor-0.1.2.tar", max compression
+gzip compressed data, was "router_log_preprocessor-0.1.3.tar", max compression
```

## Comparing `router_log_preprocessor-0.1.2.tar` & `router_log_preprocessor-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.2/LICENSE
--rw-r--r--   0        0        0     8920 2023-04-13 12:24:43.831463 router_log_preprocessor-0.1.2/README.md
--rw-r--r--   0        0        0      794 2023-04-13 13:07:15.158555 router_log_preprocessor-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.2/router_log_preprocessor/__init__.py
--rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.2/router_log_preprocessor/__main__.py
--rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__init__.py
--rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
--rw-r--r--   0        0        0     1317 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
--rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_dnsmasq_dhcp.py
--rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_message.py
--rw-r--r--   0        0        0     1536 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_wlc.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__init__.py
--rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
--rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/abc.py
--rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__init__.py
--rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
--rw-r--r--   0        0        0     1907 2023-04-13 12:48:57.905739 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
--rw-r--r--   0        0        0     4217 2023-04-13 12:50:18.950272 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
--rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_known_clients.py
--rw-r--r--   0        0        0     2654 2023-04-13 12:48:56.785731 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_mapper.py
--rw-r--r--   0        0        0     5820 2023-04-13 12:50:17.498262 router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_trapper.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__init__.py
--rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
--rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
--rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/handler.py
--rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/server.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__init__.py
--rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
--rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
--rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
--rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/typing.py
--rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/wlc.py
--rw-r--r--   0        0        0     2327 2023-04-05 19:10:32.809547 router_log_preprocessor-0.1.2/router_log_preprocessor/settings.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/util/__init__.py
--rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
--rw-r--r--   0        0        0     3026 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
--rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/util/logging.py
--rw-r--r--   0        0        0     3588 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.2/router_log_preprocessor/util/rfc3164_parser.py
--rw-r--r--   0        0        0    10333 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.2/setup.py
--rw-r--r--   0        0        0     9790 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.3/LICENSE
+-rw-r--r--   0        0        0     8920 2023-04-13 12:24:43.831463 router_log_preprocessor-0.1.3/README.md
+-rw-r--r--   0        0        0      794 2023-04-14 08:30:46.328283 router_log_preprocessor-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.3/router_log_preprocessor/__init__.py
+-rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.3/router_log_preprocessor/__main__.py
+-rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
+-rw-r--r--   0        0        0     1317 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
+-rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_dnsmasq_dhcp.py
+-rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_message.py
+-rw-r--r--   0        0        0     1536 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_wlc.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
+-rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/abc.py
+-rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
+-rw-r--r--   0        0        0     1907 2023-04-13 12:48:57.905739 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
+-rw-r--r--   0        0        0     4217 2023-04-13 12:50:18.950272 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
+-rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_known_clients.py
+-rw-r--r--   0        0        0     2654 2023-04-13 12:48:56.785731 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_mapper.py
+-rw-r--r--   0        0        0     5820 2023-04-13 12:50:17.498262 router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_trapper.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
+-rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
+-rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/handler.py
+-rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/server.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
+-rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
+-rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
+-rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/typing.py
+-rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/wlc.py
+-rw-r--r--   0        0        0     2327 2023-04-05 19:10:32.809547 router_log_preprocessor-0.1.3/router_log_preprocessor/settings.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/util/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
+-rw-r--r--   0        0        0     3026 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
+-rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/util/logging.py
+-rw-r--r--   0        0        0     3588 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.3/router_log_preprocessor/util/rfc3164_parser.py
+-rw-r--r--   0        0        0    10333 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.3/setup.py
+-rw-r--r--   0        0        0     9790 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.3/PKG-INFO
```

### Comparing `router_log_preprocessor-0.1.2/LICENSE` & `router_log_preprocessor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/README.md` & `router_log_preprocessor-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/pyproject.toml` & `router_log_preprocessor-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "router-log-preprocessor"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 repository = "https://github.com/mastdi/router-log-preprocessor"
 authors = ["Martin Storgaard Dieu <martin@storgaarddieu.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "router_log_preprocessor"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = {extras = ["dotenv"], version = "^1.10.4"}
 anyio = "^3.6.2"
 macaddress = "^2.0.2"
-asyncio-zabbix-sender = "^0.1.1"
+asyncio-zabbix-sender = "^0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [tool.mypy]
```

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/__init__.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/__main__.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/__main__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__init__.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_message.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_message.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/domain/_wlc.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/domain/_wlc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__init__.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/abc.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/abc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__init__.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_known_clients.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_known_clients.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_mapper.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_mapper.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/hooks/zabbix/_trapper.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/hooks/zabbix/_trapper.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__init__.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/handler.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/handler.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/log_server/server.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/log_server/server.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__init__.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/typing.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/typing.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/preprocessors/wlc.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/preprocessors/wlc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/settings.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/settings.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/util/__init__.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/util/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc` & `router_log_preprocessor-0.1.3/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/util/logging.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/util/logging.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/router_log_preprocessor/util/rfc3164_parser.py` & `router_log_preprocessor-0.1.3/router_log_preprocessor/util/rfc3164_parser.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.2/setup.py` & `router_log_preprocessor-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,25 +11,25 @@
  'router_log_preprocessor.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['anyio>=3.6.2,<4.0.0',
- 'asyncio-zabbix-sender>=0.1.1,<0.2.0',
+ 'asyncio-zabbix-sender>=0.1.2,<0.2.0',
  'macaddress>=2.0.2,<3.0.0',
  'pydantic[dotenv]>=1.10.4,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['router-log-preprocessor = '
                      'router_log_preprocessor.__main__:main']}
 
 setup_kwargs = {
     'name': 'router-log-preprocessor',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '# Router Log Preprocessor\n![router-log-preprocessor](https://user-images.githubusercontent.com/105678820/228938795-66dbd955-813b-4fb3-a559-4f3a41f55bb9.png)\n\n> Garbage in, garbage out\n>\n> &mdash; <cite>George Fuechsel</cite>\n\nPreprocessors upcycle garbage input data into well-structured data to ensure reliable and accurate event handling in third-party systems such as Zabbix.\nBy parsing and filtering the input log data, the preprocessor helps to ensure that only high-quality data are sent for further analysis and alerting.\nThis helps to minimize false positives and ensure that network administrators receive reliable and actionable alerts about potential security threats or other issues.\n\n\nKey features:\n- **Wireless LAN Controller event** log entries are parsed to tangible enumerations\n- **DNSMASQ DHCP** log entries are parsed to catch which IP a given client is assigned to\n- **Zabbix** templates are included to ensure that the logs are can lead to actionable alerts\n- **Extendable** preprocessors and hooks to ensure future reliable information to network administrators\n\n## Installation\n```console\n$ pip install router-log-preprocessor\n```\n\nIf needed it can also be installed from sources.\nRequires [Poetry 1.3.2](https://python-poetry.org/).\n```console\n$ git pull https://github.com/mastdi/router-log-preprocessor.git\n$ cd router-log-preprocessor\n$ poetry install\n```\n\n## Usage\nInstalling the package using pip also creates the executable script named `router-log-preprocessor`.\nOn Linux systems the router log preprocessor can be run by\n\n```console\n./router-log-preprocessor\n```\n\nThe configuration solely happens through environment variables or a `.env` configuration file located in the current working directory.\nThe most important variables are documented below. \nA full sample can be found in [.env](https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env).\nThe application reads, in order of the least priority to the highest file:\n1. `.env`,\n2. `.env.dev`,\n3. `.env.test`,\n4. `.env.staging`,\n5. `.env.prod`,\n\nmeaning that values stored in `.env.prod` will overwrite any values from other dovenv files.\nParameters stored in environment variables will always take priority over values loaded from a dotenv file.\n\n```dotenv\n# Purpose: Specifies the IP address or hostname of the local interface to which the\n# logging system should bind.\n# Format: A string containing a valid IP address or hostname, such as "192.168.0.1" or\n# "example.com".\nLOG_SERVER_HOST="0.0.0.0"\n\n# Purpose: Specifies the port number of the server to which log data should be sent.\n# Format: An integer representing a valid port number, such as 514.\nLOG_SERVER_PORT=8514\n\n# Purpose: Specifies the hostname or IP address of the Zabbix server to which the\n# Zabbix Sender should send monitoring data.\n# Format: A string containing a valid hostname or IP address, such as "example.com" or\n# "192.168.0.1".\nZABBIX_HOST="example.com"\n\n# Purpose: Specifies the port number on which the Zabbix server is running and to\n# which the Zabbix Sender should send monitoring data.\n# Format: An integer representing a valid port number, such as 10051.\nZABBIX_PORT=10051\n```\n\n## As a service\n\nThis part will go through the steps to set up the Router Log Preprocessor as a service on Ubuntu.\nThe following steps will be explained in details below:\n\n- Create a service user\n- Create a virtual environment\n- Configure environment variables\n- Set up the logging directory\n- Create the service file\n- Start the service and check its status\n- Debugging the service using journalctl\n\n### Prerequisites\n\nTo install and set up the Router Log Preprocessor as a service on Ubuntu, you will need:\n\n- Python 3.8 installed or higher\n- `venv` package (can be installed via `apt-get install python3-venv` command)\n- `pip` package manager (should be included after activating the virtual environment)\n- Internet connection to download the Router Log Preprocessor package from PyPI and the `.env` file from the GitHub repository\n\nNote that some of these prerequisites may already be installed on your Ubuntu system.\nYou can check if Python and pip are installed by running the following commands:\n\n```console\npython3 --version\npip --version\n```\n\nIf both of these commands return the version number of Python and pip, respectively, you\'re good to go.\nOtherwise, you will need to install Python and pip on your Ubuntu system before proceeding.\n\n### Creating a service user\n\nFirst, we will create a service user to run the Router Log Preprocessor.\nThis is a good security practice as running the script as a root user is not needed.\n\nRun the following commands to create a new user called `rlp`:\n\n```console\nsudo adduser rlp --disabled-password --gecos ""\nsudo su rlp\ncd ~\n```\n\nThe first command creates a new user called `rlp` with a disabled password and no additional information. \nThe second command switches to the new user and moves to their home directory.\n\n### Creating a virtual environment\n\nNow that we have a service user set up, we can create a virtual environment to install the Router Log Preprocessor.\nThe following commands create a virtual environment using Python 3.8 and install the Router Log Preprocessor package:\n\n```console\npython3 -m venv venv\ncd venv\nsource bin/activate\npip install router-log-preprocessor\n```\n\nThese commands create a new virtual environment in the venv directory, activate the environment, and install the Router Log Preprocessor package.\n\n### Configuring the environment variables \nWe will create a .env file in the virtual environment directory to store these variables.\nYou can copy the default [.env](https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env) file from the Router Log Preprocessor repository and customize it according to your needs:\n```console\ncurl -o .env https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env\nnano .env\n```\nThis will download the .env file from the Router Log Preprocessor repository and open it in the Nano text editor. \nCustomize the file to set the environment variables you need.\n\nWe are done setting up the servie user:\n\n```console\nexit\n```\n\n### Setting up the logging directory\n\nIf you have set the `LOGGING_DIRECTORY` variable in the .env file to `/var/log/rlp`, you need to create the directory and set the ownership to the rlp user:\n\n```console\nsudo mkdir /var/log/rlp\nsudo chown rlp:rlp /var/log/rlp\n```\n\nThese commands will create the `/var/log/rlp` directory and set the ownership to the `rlp` user.\n\n### Creating the service file\n\nThe next step is to create a service file for the Router Log Preprocessor.\nThis file specifies how the service should be started and managed by the system.\nCreate a new file called rlp.service in the /etc/systemd/system/ directory using the following command:\n\n```console\nsudo nano /etc/systemd/system/rlp.service\n```\n\nThis will open the text editor with a new file.\nCopy the following text into the file:\n\n```ini\n[Unit]\nDescription=Router Log Preprocessor service\nAfter=network.target\n\n[Service]\nUser=rlp\nWorkingDirectory=/home/rlp/venv\nEnvironment="PATH=/home/rlp/venv/bin"\nEnvironmentFile=/home/rlp/venv/.env\nExecStart=/home/rlp/venv/bin/router-log-preprocessor\nRestart=on-failure\nRestartSec=5s\nStartLimitInterval=60s\nStartLimitBurst=3\n\n[Install]\nWantedBy=multi-user.target\n```\n\n\n### Starting the service\n\nThe service is now ready to be started.\nThe final step is to start the service, check if it is running, and ensuring that the service starts automatically on system boot.\nStart the service using the following command:\n```console\nsudo systemctl start rlp.service\n```\n\nThis starts the service based on the configuration we just provided.\nCheck that the service is started using the following command:\n\n```console\nsudo systemctl status rlp.service\n```\n\nThis should show `active (running)` in the console.\nTo make sure the service is started on system boot use the following command:\n\n```console\nsudo systemctl enable rlp.service \n```\n\n### Debugging the service creation\n\nTo debug any issues with the service, you can use the `journalctl` command.\nFor example, to view the logs of the `rlp` service, run the following command:\n\n```console\nsudo journalctl -u rlp.service -e\n```\n\nThis will show the logs of the `rlp` service and the `-e` flag will show the end of the logs.\nYou can use other flags like `-f` to follow the logs in real-time, `-n` to specify the number of lines to show, and `-r` to show the logs in reverse order (most recent first).\n\nIf the service crashes, you can also use the `--since` and `--until` flags to show the logs between a specific time range.\nFor example, to show the logs of the last 10 minutes, run the following command:\n\n```console\nsudo journalctl -u rlp.service --since "10 minutes ago"\n```\nThis will show the logs of the `rlp` service that were generated in the last 10 minutes.\nUse this command to debug any issues with the service.',
     'author': 'Martin Storgaard Dieu',
     'author_email': 'martin@storgaarddieu.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mastdi/router-log-preprocessor',
```

### Comparing `router_log_preprocessor-0.1.2/PKG-INFO` & `router_log_preprocessor-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: router-log-preprocessor
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/mastdi/router-log-preprocessor
 License: Apache-2.0
 Author: Martin Storgaard Dieu
 Author-email: martin@storgaarddieu.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.6.2,<4.0.0)
-Requires-Dist: asyncio-zabbix-sender (>=0.1.1,<0.2.0)
+Requires-Dist: asyncio-zabbix-sender (>=0.1.2,<0.2.0)
 Requires-Dist: macaddress (>=2.0.2,<3.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.4,<2.0.0)
 Project-URL: Repository, https://github.com/mastdi/router-log-preprocessor
 Description-Content-Type: text/markdown
 
 # Router Log Preprocessor
 ![router-log-preprocessor](https://user-images.githubusercontent.com/105678820/228938795-66dbd955-813b-4fb3-a559-4f3a41f55bb9.png)
```

