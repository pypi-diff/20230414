# Comparing `tmp/heizer-999999.dev1681435064.tar.gz` & `tmp/heizer-999999.dev1681441259.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heizer-999999.dev1681435064.tar", last modified: Fri Apr 14 01:17:51 2023, max compression
+gzip compressed data, was "heizer-999999.dev1681441259.tar", last modified: Fri Apr 14 03:01:07 2023, max compression
```

## Comparing `heizer-999999.dev1681435064.tar` & `heizer-999999.dev1681441259.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.859037 heizer-999999.dev1681435064/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.github/workflows/deploy-latest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/img1.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/_static/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_static/websocket/create-topic.png
--rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_static/websocket/message-in-browser.png
--rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_static/websocket/publish-kafka-msg.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/heizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/tutorial/consumer.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/tutorial/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/tutorial/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/heizer/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 01:17:44.000000 heizer-999999.dev1681435064/heizer/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/heizer/_source/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/heizer/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/heizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/samples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/samples/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/samples/websockets/client.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/samples/websockets/server.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/tests/test_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.043470 heizer-999999.dev1681441259/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.github/workflows/deploy-latest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/img1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/source/_static/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_static/websocket/create-topic.png
+-rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_static/websocket/message-in-browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_static/websocket/publish-kafka-msg.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/heizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/tutorial/consumer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/tutorial/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/tutorial/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/heizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 03:00:59.000000 heizer-999999.dev1681441259/heizer/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/heizer/_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/heizer/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/heizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/samples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/samples/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/samples/websockets/client.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/samples/websockets/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/tests/test_consumer.py
```

### Comparing `heizer-999999.dev1681435064/.github/workflows/deploy-latest.yml` & `heizer-999999.dev1681441259/.github/workflows/deploy-latest.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/.github/workflows/main.yml` & `heizer-999999.dev1681441259/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/.github/workflows/release.yml` & `heizer-999999.dev1681441259/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/.gitignore` & `heizer-999999.dev1681441259/.gitignore`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/.pre-commit-config.yaml` & `heizer-999999.dev1681441259/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/LICENSE` & `heizer-999999.dev1681441259/LICENSE`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/PKG-INFO` & `heizer-999999.dev1681441259/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1681435064
+Version: 999999.dev1681441259
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,16 +53,14 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat)](https://pycqa.github.io/isort/)
 
 
 A python library to easily create kafka producer and consumer
 
 ## Install
 
-> Note: Heizer is still in development, so you need to install it with `--pre` flag
-
 ```shell
 pip install heizer
 ```
 
 ## Setup
 Use `docker-compose.yaml` file to start kafka service
```

### Comparing `heizer-999999.dev1681435064/docker-compose.yaml` & `heizer-999999.dev1681441259/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/Makefile` & `heizer-999999.dev1681441259/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/img1.png` & `heizer-999999.dev1681441259/docs/img1.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/make.bat` & `heizer-999999.dev1681441259/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/source/_static/websocket/create-topic.png` & `heizer-999999.dev1681441259/docs/source/_static/websocket/create-topic.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/source/_static/websocket/message-in-browser.png` & `heizer-999999.dev1681441259/docs/source/_static/websocket/message-in-browser.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/source/_static/websocket/publish-kafka-msg.png` & `heizer-999999.dev1681441259/docs/source/_static/websocket/publish-kafka-msg.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/source/_templates/versions.html` & `heizer-999999.dev1681441259/docs/source/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/source/conf.py` & `heizer-999999.dev1681441259/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/source/tutorial/consumer.rst` & `heizer-999999.dev1681441259/docs/source/tutorial/consumer.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/source/tutorial/prepare.rst` & `heizer-999999.dev1681441259/docs/source/tutorial/prepare.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/docs/source/tutorial/websockets.rst` & `heizer-999999.dev1681441259/docs/source/tutorial/websockets.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/heizer/_source/__init__.py` & `heizer-999999.dev1681441259/heizer/_source/__init__.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/heizer/_source/consumer.py` & `heizer-999999.dev1681441259/heizer/_source/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 from uuid import uuid4
 
 from confluent_kafka import Consumer
 from pydantic import BaseModel
 
 from heizer._source import get_logger
+from heizer._source.admin import create_new_topic, get_admin_client
 from heizer._source.message import HeizerMessage
 from heizer._source.topic import HeizerTopic
 from heizer.config import HeizerConfig
 from heizer.types import (
     Any,
     Awaitable,
     Callable,
@@ -44,46 +45,55 @@
     call_once: bool = False
     stopper: Optional[Stopper] = None
     deserializer: Optional[Type[BaseModel]] = None
 
     is_async: bool = False
     poll_timeout: int = 1
 
+    init_topics: bool = True
+
     def __init__(
         self,
         *,
         topics: List[HeizerTopic],
         config: HeizerConfig = HeizerConfig(),
         call_once: bool = False,
         stopper: Optional[Stopper] = None,
         deserializer: Optional[Type[BaseModel]] = None,
         is_async: bool = False,
         name: Optional[str] = None,
         poll_timeout: Optional[int] = None,
+        init_topics: bool = True,
     ):
         self.topics = topics
         self.config = config
         self.call_once = call_once
         self.stopper = stopper
         self.deserializer = deserializer
         self.__id__ = str(uuid4())
         self.name = name or self.__id__
         self.is_async = is_async
         self.poll_timeout = poll_timeout or 1
+        self.init_topics = init_topics
 
     async def __run__(
         self,
         func: Callable[Concatenate[HeizerMessage, P], Union[T, Awaitable[T]]],
         c: Consumer,
         is_async: bool,
         *args: P.args,
         **kwargs: P.kwargs,
     ) -> Union[Optional[T]]:  # ignore type
         """Run the consumer"""
 
+        if self.init_topics:
+            logger.debug("Initializing topics")
+            admin_client = get_admin_client(self.config)
+            create_new_topic(admin_client, self.topics)
+
         while True:
             msg = c.poll(self.poll_timeout)
 
             if msg is None:
                 continue
 
             if msg.error():
```

### Comparing `heizer-999999.dev1681435064/heizer/_source/message.py` & `heizer-999999.dev1681441259/heizer/_source/message.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/heizer/_source/producer.py` & `heizer-999999.dev1681441259/heizer/_source/producer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 import json
 from uuid import uuid4
 
 from confluent_kafka import Message, Producer
 
 from heizer._source import get_logger
+from heizer._source.admin import create_new_topic, get_admin_client
 from heizer._source.topic import HeizerTopic
 from heizer.config import HeizerConfig
 from heizer.types import Any, Callable, Dict, List, Optional, TypeVar, Union, cast
 
 logger = get_logger(__name__)
 
 R = TypeVar("R")
@@ -50,28 +51,31 @@
 
     default_key: Optional[str] = None
     default_headers: Optional[Dict[str, str]] = None
 
     key_alias: str = "key"
     headers_alias: str = "headers"
 
+    init_topics: bool = True
+
     # private properties
     _producer_instance: Optional[Producer] = None
 
     def __init__(
         self,
         topics: List[HeizerTopic],
         config: HeizerConfig = HeizerConfig(),
         serializer: Callable[..., bytes] = _default_serializer,
         call_back: Optional[Callable[..., Any]] = None,
         default_key: Optional[str] = None,
         default_headers: Optional[Dict[str, str]] = None,
         key_alias: Optional[str] = None,
         headers_alias: Optional[str] = None,
         name: Optional[str] = None,
+        init_topics: bool = True,
     ):
         self.topics = topics
         self.config = config
         self.serializer = serializer
         self.call_back = call_back
         self.default_key = default_key
         self.default_headers = default_headers
@@ -79,37 +83,43 @@
         if key_alias:
             self.key_alias = key_alias
         if headers_alias:
             self.headers_alias = headers_alias
 
         self.__id__ = str(uuid4())
         self.name = name or self.__id__
+        self.init_topics = init_topics
 
     @property
     def _producer(self) -> Producer:
         if not self._producer_instance:
             self._producer_instance = Producer(self.config.value)
         return self._producer_instance
 
     def __call__(self, func: F) -> F:
         @functools.wraps(func)
         def decorator(*args: Any, **kwargs: Any) -> Any:
+            if self.init_topics:
+                logger.debug("Initializing topics")
+                admin_client = get_admin_client(self.config)
+                create_new_topic(admin_client, self.topics)
+
             try:
                 result = func(*args, **kwargs)
             except Exception as e:
                 raise e
 
             try:
-                key = result.get(self.key_alias, self.default_key)
+                key = result.pop(self.key_alias, self.default_key)
             except Exception as e:
                 logger.debug(f"Failed to get key from result. {str(e)}")
                 key = self.default_key
 
             try:
-                headers = result.get(self.headers_alias, self.default_headers)
+                headers = result.pop(self.headers_alias, self.default_headers)
             except Exception as e:
                 logger.debug(
                     f"Failed to get headers from result. {str(e)}",
                 )
                 headers = self.default_headers
 
             headers = cast(Dict[str, str], headers)
```

### Comparing `heizer-999999.dev1681435064/heizer/_source/topic.py` & `heizer-999999.dev1681441259/heizer/_source/topic.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,26 @@
 
 from confluent_kafka import TopicPartition
 
 
 class HeizerTopic(TopicPartition):
     name: str
     _partitions: List[int]
+    _replication_factor: int
     _topic_partitions: List[TopicPartition]
 
-    def __init__(self, name: str, partitions: Optional[List[int]] = None):
+    def __init__(
+        self,
+        name: str,
+        partitions: Optional[List[int]] = None,
+        replication_factor: int = 1,
+    ):
         self._partitions = partitions or [-1]
         self._topic_partitions = []
+        self._replication_factor = replication_factor
         self.name = name
 
         for partition in self._partitions:
             self._topic_partitions.append(TopicPartition(topic=name, partition=partition))
 
     @property
     def partitions(self) -> List[int]:
```

### Comparing `heizer-999999.dev1681435064/heizer/config.py` & `heizer-999999.dev1681441259/heizer/config.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/heizer/types.py` & `heizer-999999.dev1681441259/heizer/types.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/heizer.egg-info/PKG-INFO` & `heizer-999999.dev1681441259/heizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1681435064
+Version: 999999.dev1681441259
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,16 +53,14 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat)](https://pycqa.github.io/isort/)
 
 
 A python library to easily create kafka producer and consumer
 
 ## Install
 
-> Note: Heizer is still in development, so you need to install it with `--pre` flag
-
 ```shell
 pip install heizer
 ```
 
 ## Setup
 Use `docker-compose.yaml` file to start kafka service
```

### Comparing `heizer-999999.dev1681435064/heizer.egg-info/SOURCES.txt` & `heizer-999999.dev1681441259/heizer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 heizer/types.py
 heizer.egg-info/PKG-INFO
 heizer.egg-info/SOURCES.txt
 heizer.egg-info/dependency_links.txt
 heizer.egg-info/requires.txt
 heizer.egg-info/top_level.txt
 heizer/_source/__init__.py
+heizer/_source/admin.py
 heizer/_source/consumer.py
 heizer/_source/message.py
 heizer/_source/producer.py
 heizer/_source/topic.py
 heizer/bin/__init__.py
 samples/requirements.txt
 samples/websockets/client.html
```

### Comparing `heizer-999999.dev1681435064/pyproject.toml` & `heizer-999999.dev1681441259/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/samples/websockets/client.html` & `heizer-999999.dev1681441259/samples/websockets/client.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/samples/websockets/server.py` & `heizer-999999.dev1681441259/samples/websockets/server.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681435064/tests/test_consumer.py` & `heizer-999999.dev1681441259/tests/test_consumer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import json
 import logging
 import os
 from typing import Any, Dict, cast
 
+import pytest
 from pydantic import BaseModel
 
 from heizer import HeizerConfig, HeizerMessage, HeizerTopic, consumer, producer
 
 Producer_Config = HeizerConfig(
     {
         "bootstrap.servers": os.environ.get("KAFKA_SERVER", "localhost:9092"),
     }
 )
 
-Consumer_Config = HeizerConfig(
-    {
-        "bootstrap.servers": os.environ.get("KAFKA_SERVER", "localhost:9092"),
-        "group.id": "default",
-        "auto.offset.reset": "earliest",
-    }
-)
+
+@pytest.fixture
+def group_id():
+    return "test_group"
 
 
-def test_consumer_stopper() -> None:
+@pytest.fixture
+def consumer_config(group_id):
+    return HeizerConfig(
+        {
+            "bootstrap.servers": os.environ.get("KAFKA_SERVER", "localhost:9092"),
+            "group.id": group_id,
+            "auto.offset.reset": "earliest",
+        }
+    )
+
+
+@pytest.mark.parametrize("group_id", ["test_consumer_stopper"])
+def test_consumer_stopper(group_id, consumer_config) -> None:
     @producer(
-        topics=[HeizerTopic(name="heizer.test.result")],
+        topics=[HeizerTopic(name="heizer.test.result", partitions=[0, 1, 2], replication_factor=2)],
         config=Producer_Config,
         key_alias="myKey",
         headers_alias="myHeaders",
     )
     def produce_data(status: str, result_value: str) -> Dict[str, Any]:
         return {
             "key1": 1,
@@ -44,54 +54,60 @@
         data = json.loads(msg.value)
         if data["status"] == "success":
             return True
         return False
 
     @consumer(
         topics=[HeizerTopic(name="heizer.test.result")],
-        config=Consumer_Config,
+        config=consumer_config,
         stopper=stopper,
     )
     def consume_data(msg, *args, **kwargs) -> str:
         data = json.loads(msg.value)
 
         assert msg.key == "id1"
         assert msg.headers == {"header1": "value1", "header2": "value2"}
 
+        assert "myKey" not in data
+        assert "myHeaders" not in data
+
         return cast(str, data["result"])
 
     produce_data("start", "waiting")
     produce_data("loading", "waiting")
     produce_data("success", "finished")
     produce_data("postprocess", "postprocess")
 
     result = consume_data()  # type: ignore
 
     assert result == "finished"
 
 
-def test_consumer_call_once() -> None:
+@pytest.mark.parametrize("group_id", ["test_consumer_call_once"])
+def test_consumer_call_once(consumer_config) -> None:
     topic_name = "heizer.test.test_consumer_call_once"
 
     @producer(
         topics=[HeizerTopic(name=topic_name)],
         config=Producer_Config,
+        key_alias="non_existing_key",
+        headers_alias="non_existing_headers",
     )
     def produce_data(status: str, result: str) -> Dict[str, Any]:
         return {
             "key1": 1,
             "key2": "2",
             "key3": True,
             "status": status,
             "result": result,
         }
 
     @consumer(
         topics=[HeizerTopic(name=topic_name)],
-        config=Consumer_Config,
+        config=consumer_config,
         call_once=True,
     )
     def consume_data(msg, *args, **kwargs) -> str:
         data = json.loads(msg.value)
         return cast(str, data["result"])
 
     produce_data("start", "waiting")
@@ -99,15 +115,16 @@
     produce_data("success", "finished")
 
     result = consume_data()
 
     assert result == "waiting"
 
 
-def test_consumer_deserializer(caplog) -> None:
+@pytest.mark.parametrize("group_id", ["test_consumer_deserializer"])
+def test_consumer_deserializer(caplog, consumer_config) -> None:
     caplog.set_level(logging.DEBUG)
     topic_name = "heizer.test.test_consumer_deserializer"
 
     class TestModel(BaseModel):
         name: str
         age: int
 
@@ -121,15 +138,15 @@
         return {
             "name": "mike",
             "age": 20,
         }
 
     @consumer(
         topics=[HeizerTopic(name=topic_name)],
-        config=Consumer_Config,
+        config=consumer_config,
         call_once=True,
         deserializer=deserializer,
     )
     def consume_data(message: HeizerMessage, *args, **kwargs):
         return message.formatted_value
 
     produce_data()
```

