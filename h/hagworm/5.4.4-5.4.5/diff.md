# Comparing `tmp/hagworm-5.4.4.tar.gz` & `tmp/hagworm-5.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.4.4.tar", last modified: Thu Apr 13 09:18:36 2023, max compression
+gzip compressed data, was "hagworm-5.4.5.tar", last modified: Fri Apr 14 03:16:22 2023, max compression
```

## Comparing `hagworm-5.4.4.tar` & `hagworm-5.4.5.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.453160 hagworm-5.4.4/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.4.4/LICENSE
--rw-rw-rw-   0        0        0     7509 2023-04-13 09:18:36.452159 hagworm-5.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.339657 hagworm-5.4.4/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.4.4/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.342657 hagworm-5.4.4/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.349719 hagworm-5.4.4/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.352717 hagworm-5.4.4/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      840 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1417 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.354718 hagworm-5.4.4/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.356160 hagworm-5.4.4/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      788 2023-03-01 02:07:14.000000 hagworm-5.4.4/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.357159 hagworm-5.4.4/hagworm/
--rw-rw-rw-   0        0        0      510 2023-04-13 09:17:44.000000 hagworm-5.4.4/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.395160 hagworm-5.4.4/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.422159 hagworm-5.4.4/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16082 2023-04-11 09:03:03.000000 hagworm-5.4.4/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4773 2023-04-11 08:20:16.000000 hagworm-5.4.4/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2008 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     3073 2023-04-12 08:05:02.000000 hagworm-5.4.4/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1308 2023-04-11 09:00:40.000000 hagworm-5.4.4/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    14412 2023-04-12 08:15:17.000000 hagworm-5.4.4/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1490 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    10611 2023-04-11 07:37:23.000000 hagworm-5.4.4/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     3787 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.4.4/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22551 2023-04-12 08:21:47.000000 hagworm-5.4.4/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1759 2023-04-12 08:23:58.000000 hagworm-5.4.4/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1699 2023-04-12 08:24:47.000000 hagworm-5.4.4/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4375 2023-04-13 02:37:21.000000 hagworm-5.4.4/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2208 2023-04-12 08:06:38.000000 hagworm-5.4.4/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14859 2023-04-13 09:17:30.000000 hagworm-5.4.4/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-04-08 01:06:26.000000 hagworm-5.4.4/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     3555 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     6909 2023-04-12 08:32:50.000000 hagworm-5.4.4/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3620 2023-04-12 08:40:57.000000 hagworm-5.4.4/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.426159 hagworm-5.4.4/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.433159 hagworm-5.4.4/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     7849 2023-04-12 08:55:19.000000 hagworm-5.4.4/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3822 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.436159 hagworm-5.4.4/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.438159 hagworm-5.4.4/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.442159 hagworm-5.4.4/hagworm/third/aliyun/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/aliyun/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/aliyun/logging.py
--rw-rw-rw-   0        0        0    10141 2023-04-12 08:57:49.000000 hagworm-5.4.4/hagworm/third/aliyun/rocketmq.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.445161 hagworm-5.4.4/hagworm/third/consul/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/consul/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/consul/config.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.451159 hagworm-5.4.4/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3437 2023-04-12 09:00:41.000000 hagworm-5.4.4/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.4.4/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.4.4/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:18:36.364160 hagworm-5.4.4/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7509 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2262 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      707 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 09:18:36.000000 hagworm-5.4.4/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 09:18:36.453160 hagworm-5.4.4/setup.cfg
--rw-rw-rw-   0        0        0     2291 2023-03-01 02:07:14.000000 hagworm-5.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.139502 hagworm-5.4.5/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.4.5/LICENSE
+-rw-rw-rw-   0        0        0     7509 2023-04-14 03:16:22.138501 hagworm-5.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.022531 hagworm-5.4.5/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.4.5/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.025501 hagworm-5.4.5/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.031502 hagworm-5.4.5/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.034502 hagworm-5.4.5/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      840 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1417 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.035536 hagworm-5.4.5/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.036531 hagworm-5.4.5/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      788 2023-03-01 02:07:14.000000 hagworm-5.4.5/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.038503 hagworm-5.4.5/hagworm/
+-rw-rw-rw-   0        0        0      510 2023-04-14 01:21:17.000000 hagworm-5.4.5/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.076501 hagworm-5.4.5/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.104501 hagworm-5.4.5/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16082 2023-04-11 09:03:03.000000 hagworm-5.4.5/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4773 2023-04-11 08:20:16.000000 hagworm-5.4.5/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2008 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     3073 2023-04-12 08:05:02.000000 hagworm-5.4.5/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1308 2023-04-11 09:00:40.000000 hagworm-5.4.5/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    14412 2023-04-12 08:15:17.000000 hagworm-5.4.5/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1490 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    12069 2023-04-14 02:51:40.000000 hagworm-5.4.5/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     3787 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.4.5/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/asyncio/zmq.py
+-rw-rw-rw-   0        0        0    22551 2023-04-12 08:21:47.000000 hagworm-5.4.5/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1759 2023-04-12 08:23:58.000000 hagworm-5.4.5/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1699 2023-04-12 08:24:47.000000 hagworm-5.4.5/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4375 2023-04-13 02:37:21.000000 hagworm-5.4.5/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2208 2023-04-12 08:06:38.000000 hagworm-5.4.5/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    14859 2023-04-13 09:17:30.000000 hagworm-5.4.5/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-04-08 01:06:26.000000 hagworm-5.4.5/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     3555 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     6909 2023-04-12 08:32:50.000000 hagworm-5.4.5/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3620 2023-04-12 08:40:57.000000 hagworm-5.4.5/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.109501 hagworm-5.4.5/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.116501 hagworm-5.4.5/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     7849 2023-04-12 08:55:19.000000 hagworm-5.4.5/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3822 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.119501 hagworm-5.4.5/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.122502 hagworm-5.4.5/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.127501 hagworm-5.4.5/hagworm/third/aliyun/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/third/aliyun/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/third/aliyun/logging.py
+-rw-rw-rw-   0        0        0    10141 2023-04-12 08:57:49.000000 hagworm-5.4.5/hagworm/third/aliyun/rocketmq.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.130501 hagworm-5.4.5/hagworm/third/consul/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/third/consul/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/third/consul/config.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.136501 hagworm-5.4.5/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3437 2023-04-12 09:00:41.000000 hagworm-5.4.5/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.4.5/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.4.5/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:16:22.046501 hagworm-5.4.5/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7509 2023-04-14 03:16:21.000000 hagworm-5.4.5/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2262 2023-04-14 03:16:21.000000 hagworm-5.4.5/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 03:16:21.000000 hagworm-5.4.5/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      707 2023-04-14 03:16:21.000000 hagworm-5.4.5/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 03:16:21.000000 hagworm-5.4.5/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 03:16:22.139502 hagworm-5.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     2291 2023-03-01 02:07:14.000000 hagworm-5.4.5/setup.py
```

### Comparing `hagworm-5.4.4/LICENSE` & `hagworm-5.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/PKG-INFO` & `hagworm-5.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.4.4
+Version: 5.4.5
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.4.4/README.md` & `hagworm-5.4.5/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/c_extend/math.c` & `hagworm-5.4.5/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.4.5/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/example/fastapi_demo/main.py` & `hagworm-5.4.5/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/example/fastapi_demo/service/__init__.py` & `hagworm-5.4.5/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/example/fastapi_demo/setting.py` & `hagworm-5.4.5/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/example/main_test.py` & `hagworm-5.4.5/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/base.py` & `hagworm-5.4.5/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/buffer.py` & `hagworm-5.4.5/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/command.py` & `hagworm-5.4.5/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/event.py` & `hagworm-5.4.5/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/file.py` & `hagworm-5.4.5/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/future.py` & `hagworm-5.4.5/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/mail.py` & `hagworm-5.4.5/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/mongo.py` & `hagworm-5.4.5/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/mysql.py` & `hagworm-5.4.5/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/net.py` & `hagworm-5.4.5/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/ntp.py` & `hagworm-5.4.5/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/pool.py` & `hagworm-5.4.5/hagworm/extend/asyncio/pool.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/redis.py` & `hagworm-5.4.5/hagworm/extend/asyncio/redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,34 +2,66 @@
 
 __author__ = r'wsb310@gmail.com'
 
 from aredis import lock, StrictRedis, StrictRedisCluster
 
 from .base import Utils
 
-from ..error import catch_error
+from ..error import catch_error, catch_warning
 from ..interface import AsyncContextManager
 from .ntp import AsyncNTPClient
 from .transaction import Transaction
 
 
 REDIS_ERROR_RETRY_COUNT = 0x10
 REDIS_POOL_WATER_LEVEL_WARNING_LINE = 0x10
 
 
 class LuaLock(AsyncContextManager, lock.LuaLock):
 
+    def __init__(
+            self, redis, name, timeout=None, sleep=0.1,
+            blocking=False, blocking_timeout=None, thread_local=True
+    ):
+        super().__init__(
+            redis, name, timeout=timeout, sleep=sleep,
+            blocking=blocking, blocking_timeout=blocking_timeout, thread_local=thread_local
+        )
+
     async def _context_release(self):
-        await self.release()
+        with catch_warning():
+            await super().release()
+
+    async def acquire(self, blocking=None, blocking_timeout=None):
+        if self.local.get() is None:
+            return await super().acquire(blocking, blocking_timeout)
+        else:
+            return await super().extend(self.timeout)
 
 
 class ClusterLock(AsyncContextManager, lock.ClusterLock):
 
+    def __init__(
+            self, redis, name, timeout=None, sleep=0.1,
+            blocking=False, blocking_timeout=None, thread_local=True
+    ):
+        super().__init__(
+            redis, name, timeout=timeout, sleep=sleep,
+            blocking=blocking, blocking_timeout=blocking_timeout, thread_local=thread_local
+        )
+
     async def _context_release(self):
-        await self.release()
+        with catch_warning():
+            await super().release()
+
+    async def acquire(self, blocking=None, blocking_timeout=None):
+        if self.local.get() is None:
+            return await super().acquire(blocking, blocking_timeout)
+        else:
+            return await super().extend(self.timeout)
 
 
 class _PoolMixin(AsyncContextManager):
 
     def __init__(self, min_connections=0):
 
         self._name = Utils.uuid1()[:8]
@@ -142,17 +174,20 @@
 
         return self
 
     def get_created_connections(self):
 
         return self.connection_pool._created_connections
 
-    def allocate_lock(self, name, *, timeout=600, blocking_timeout=0):
+    def allocate_lock(self, name, *, timeout=None, sleep=0.1, blocking_timeout=None, thread_local=True):
 
-        return self.lock(name, timeout=timeout, blocking_timeout=blocking_timeout, lock_class=LuaLock)
+        return self.lock(
+            name, timeout=timeout, sleep=sleep, blocking_timeout=blocking_timeout,
+            lock_class=LuaLock, thread_local=thread_local
+        )
 
 
 class StrictRedisClusterPool(_PoolMixin, StrictRedisCluster):
     """StrictRedisCluster连接管理
     """
 
     def __init__(
@@ -202,17 +237,20 @@
 
         return self
 
     def get_created_connections(self):
 
         return sum(self.connection_pool._created_connections_per_node.values())
 
-    def allocate_lock(self, name, *, timeout=60, blocking_timeout=0):
+    def allocate_lock(self, name, *, timeout=None, sleep=0.1, blocking_timeout=None, thread_local=True):
 
-        return self.lock(name, timeout=timeout, blocking_timeout=blocking_timeout, lock_class=ClusterLock)
+        return self.lock(
+            name, timeout=timeout, sleep=sleep, blocking_timeout=blocking_timeout,
+            lock_class=ClusterLock, thread_local=thread_local
+        )
 
 
 class RedisDelegate:
     """Redis功能组件
     """
 
     def __init__(self):
```

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/socket.py` & `hagworm-5.4.5/hagworm/extend/asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/task.py` & `hagworm-5.4.5/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/transaction.py` & `hagworm-5.4.5/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/asyncio/zmq.py` & `hagworm-5.4.5/hagworm/extend/asyncio/zmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/base.py` & `hagworm-5.4.5/hagworm/extend/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/cache.py` & `hagworm-5.4.5/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/compile.py` & `hagworm-5.4.5/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/config.py` & `hagworm-5.4.5/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/crypto.py` & `hagworm-5.4.5/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/error.py` & `hagworm-5.4.5/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/event.py` & `hagworm-5.4.5/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/igraph.py` & `hagworm-5.4.5/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/interface.py` & `hagworm-5.4.5/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/logging.py` & `hagworm-5.4.5/hagworm/extend/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/media.py` & `hagworm-5.4.5/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/metaclass.py` & `hagworm-5.4.5/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/process.py` & `hagworm-5.4.5/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/qrcode.py` & `hagworm-5.4.5/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/struct.py` & `hagworm-5.4.5/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/text.py` & `hagworm-5.4.5/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/trace.py` & `hagworm-5.4.5/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/transaction.py` & `hagworm-5.4.5/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/extend/validator.py` & `hagworm-5.4.5/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/frame/fastapi/base.py` & `hagworm-5.4.5/hagworm/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/frame/fastapi/field.py` & `hagworm-5.4.5/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/frame/fastapi/model.py` & `hagworm-5.4.5/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/frame/fastapi/response.py` & `hagworm-5.4.5/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/frame/gunicorn.py` & `hagworm-5.4.5/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/frame/stress_tests.py` & `hagworm-5.4.5/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/static/cacert.pem` & `hagworm-5.4.5/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/third/aliyun/logging.py` & `hagworm-5.4.5/hagworm/third/aliyun/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/third/aliyun/rocketmq.py` & `hagworm-5.4.5/hagworm/third/aliyun/rocketmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/third/consul/config.py` & `hagworm-5.4.5/hagworm/third/consul/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/third/rabbitmq/consume.py` & `hagworm-5.4.5/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/third/rabbitmq/publish.py` & `hagworm-5.4.5/hagworm/third/rabbitmq/publish.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.4.5/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm.egg-info/PKG-INFO` & `hagworm-5.4.5/hagworm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.4.4
+Version: 5.4.5
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.4.4/hagworm.egg-info/SOURCES.txt` & `hagworm-5.4.5/hagworm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/hagworm.egg-info/requires.txt` & `hagworm-5.4.5/hagworm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.4/setup.py` & `hagworm-5.4.5/setup.py`

 * *Files identical despite different names*

