# Comparing `tmp/tonconnect-0.0.1.tar.gz` & `tmp/tonconnect-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonconnect-0.0.1.tar", last modified: Fri Apr 14 20:15:53 2023, max compression
+gzip compressed data, was "tonconnect-0.0.2.tar", last modified: Fri Apr 14 20:28:01 2023, max compression
```

## Comparing `tonconnect-0.0.1.tar` & `tonconnect-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.0.1/.gitignore
--rw-r--r--   0        0        0    11350 2023-04-14 20:08:17.432870 tonconnect-0.0.1/LICENSE.md
--rw-r--r--   0        0        0     1182 2023-04-12 09:12:00.350752 tonconnect-0.0.1/README.md
--rw-r--r--   0        0        0      288 2023-04-12 09:33:18.589470 tonconnect-0.0.1/examples/address.py
--rw-r--r--   0        0        0      552 2023-04-12 09:16:57.911646 tonconnect-0.0.1/examples/transactions.py
--rw-r--r--   0        0        0      304 2023-04-12 07:29:10.042607 tonconnect-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.0.1/tonconnect/__init__.py
--rw-r--r--   0        0        0      195 2023-04-12 07:18:49.859990 tonconnect-0.0.1/tonconnect/apps.py
--rw-r--r--   0        0        0     3709 2023-04-12 19:38:49.272910 tonconnect-0.0.1/tonconnect/bridge.py
--rw-r--r--   0        0        0     1368 2023-04-12 20:58:05.396250 tonconnect-0.0.1/tonconnect/connector.py
--rw-r--r--   0        0        0     1202 2023-04-12 07:19:51.920373 tonconnect-0.0.1/tonconnect/crypto.py
--rw-r--r--   0        0        0     3442 2023-04-12 07:39:01.886103 tonconnect-0.0.1/tonconnect/events.py
--rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.0.1/tonconnect/exceptions.py
--rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.0.1/tonconnect/options.py
--rw-r--r--   0        0        0     1745 2023-04-11 19:09:18.328616 tonconnect-0.0.1/tonconnect/requests.py
--rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.0.1/tonconnect/static.py
--rw-r--r--   0        0        0      299 2023-04-12 07:37:03.212040 tonconnect-0.0.1/tonconnect/url.py
--rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.0.1/tonconnect/utils.py
--rw-r--r--   0        0        0      361 2023-04-12 07:36:46.419499 tonconnect-0.0.1/tonconnect/wallet.py
--rw-r--r--   0        0        0      201 1970-01-01 00:00:00.000000 tonconnect-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11350 2023-04-14 20:08:17.432870 tonconnect-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1182 2023-04-12 09:12:00.350752 tonconnect-0.0.2/README.md
+-rw-r--r--   0        0        0      288 2023-04-12 09:33:18.589470 tonconnect-0.0.2/examples/address.py
+-rw-r--r--   0        0        0      552 2023-04-12 09:16:57.911646 tonconnect-0.0.2/examples/transactions.py
+-rw-r--r--   0        0        0      520 2023-04-14 20:27:48.458383 tonconnect-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.0.2/tonconnect/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-12 07:18:49.859990 tonconnect-0.0.2/tonconnect/apps.py
+-rw-r--r--   0        0        0     3709 2023-04-12 19:38:49.272910 tonconnect-0.0.2/tonconnect/bridge.py
+-rw-r--r--   0        0        0     1368 2023-04-12 20:58:05.396250 tonconnect-0.0.2/tonconnect/connector.py
+-rw-r--r--   0        0        0     1202 2023-04-12 07:19:51.920373 tonconnect-0.0.2/tonconnect/crypto.py
+-rw-r--r--   0        0        0     3442 2023-04-12 07:39:01.886103 tonconnect-0.0.2/tonconnect/events.py
+-rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.0.2/tonconnect/exceptions.py
+-rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.0.2/tonconnect/options.py
+-rw-r--r--   0        0        0     1745 2023-04-11 19:09:18.328616 tonconnect-0.0.2/tonconnect/requests.py
+-rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.0.2/tonconnect/static.py
+-rw-r--r--   0        0        0      299 2023-04-12 07:37:03.212040 tonconnect-0.0.2/tonconnect/url.py
+-rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.0.2/tonconnect/utils.py
+-rw-r--r--   0        0        0      361 2023-04-12 07:36:46.419499 tonconnect-0.0.2/tonconnect/wallet.py
+-rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 tonconnect-0.0.2/PKG-INFO
```

### Comparing `tonconnect-0.0.1/LICENSE.md` & `tonconnect-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.1/README.md` & `tonconnect-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.1/examples/transactions.py` & `tonconnect-0.0.2/examples/transactions.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.1/tonconnect/bridge.py` & `tonconnect-0.0.2/tonconnect/bridge.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.1/tonconnect/connector.py` & `tonconnect-0.0.2/tonconnect/connector.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.1/tonconnect/crypto.py` & `tonconnect-0.0.2/tonconnect/crypto.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.1/tonconnect/events.py` & `tonconnect-0.0.2/tonconnect/events.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.1/tonconnect/requests.py` & `tonconnect-0.0.2/tonconnect/requests.py`

 * *Files identical despite different names*

