# Comparing `tmp/heizer-999999.dev1681352876.tar.gz` & `tmp/heizer-999999.dev1681435064.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heizer-999999.dev1681352876.tar", last modified: Thu Apr 13 02:28:04 2023, max compression
+gzip compressed data, was "heizer-999999.dev1681435064.tar", last modified: Fri Apr 14 01:17:51 2023, max compression
```

## Comparing `heizer-999999.dev1681352876.tar` & `heizer-999999.dev1681435064.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.005730 heizer-999999.dev1681352876/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.005730 heizer-999999.dev1681352876/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/.github/workflows/deploy-latest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.005730 heizer-999999.dev1681352876/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/img1.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.005730 heizer-999999.dev1681352876/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.005730 heizer-999999.dev1681352876/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.005730 heizer-999999.dev1681352876/docs/source/_static/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/_static/websocket/create-topic.png
--rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/_static/websocket/message-in-browser.png
--rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/_static/websocket/publish-kafka-msg.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/heizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/tutorial/consumer.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/tutorial/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/docs/source/tutorial/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/heizer/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 02:27:56.000000 heizer-999999.dev1681352876/heizer/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/heizer/_source/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/_source/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/_source/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/_source/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/_source/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/heizer/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/heizer/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/heizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-13 02:28:03.000000 heizer-999999.dev1681352876/heizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-13 02:28:04.000000 heizer-999999.dev1681352876/heizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 02:28:03.000000 heizer-999999.dev1681352876/heizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 02:28:03.000000 heizer-999999.dev1681352876/heizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 02:28:03.000000 heizer-999999.dev1681352876/heizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/samples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/samples/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/samples/websockets/client.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/samples/websockets/server.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:28:04.009730 heizer-999999.dev1681352876/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-13 02:27:54.000000 heizer-999999.dev1681352876/tests/test_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.859037 heizer-999999.dev1681435064/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.github/workflows/deploy-latest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/img1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/_static/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_static/websocket/create-topic.png
+-rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_static/websocket/message-in-browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_static/websocket/publish-kafka-msg.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/heizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/tutorial/consumer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/tutorial/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/docs/source/tutorial/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.863036 heizer-999999.dev1681435064/heizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 01:17:44.000000 heizer-999999.dev1681435064/heizer/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/heizer/_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/_source/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/heizer/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/heizer/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/heizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 01:17:51.000000 heizer-999999.dev1681435064/heizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/samples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/samples/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/samples/websockets/client.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/samples/websockets/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:51.867036 heizer-999999.dev1681435064/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-14 01:17:41.000000 heizer-999999.dev1681435064/tests/test_consumer.py
```

### Comparing `heizer-999999.dev1681352876/.github/workflows/deploy-latest.yml` & `heizer-999999.dev1681435064/.github/workflows/deploy-latest.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/.github/workflows/main.yml` & `heizer-999999.dev1681435064/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/.github/workflows/release.yml` & `heizer-999999.dev1681435064/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/.gitignore` & `heizer-999999.dev1681435064/.gitignore`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/.pre-commit-config.yaml` & `heizer-999999.dev1681435064/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/LICENSE` & `heizer-999999.dev1681435064/LICENSE`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/PKG-INFO` & `heizer-999999.dev1681435064/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1681352876
+Version: 999999.dev1681435064
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,15 +56,15 @@
 A python library to easily create kafka producer and consumer
 
 ## Install
 
 > Note: Heizer is still in development, so you need to install it with `--pre` flag
 
 ```shell
-pip install --pre heizer
+pip install heizer
 ```
 
 ## Setup
 Use `docker-compose.yaml` file to start kafka service
 
 ```shell
 docker-compose up -d
```

### Comparing `heizer-999999.dev1681352876/README.md` & `heizer-999999.dev1681435064/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 A python library to easily create kafka producer and consumer
 
 ## Install
 
 > Note: Heizer is still in development, so you need to install it with `--pre` flag
 
 ```shell
-pip install --pre heizer
+pip install heizer
 ```
 
 ## Setup
 Use `docker-compose.yaml` file to start kafka service
 
 ```shell
 docker-compose up -d
```

### Comparing `heizer-999999.dev1681352876/docker-compose.yaml` & `heizer-999999.dev1681435064/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/Makefile` & `heizer-999999.dev1681435064/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/img1.png` & `heizer-999999.dev1681435064/docs/img1.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/make.bat` & `heizer-999999.dev1681435064/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/source/_static/websocket/create-topic.png` & `heizer-999999.dev1681435064/docs/source/_static/websocket/create-topic.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/source/_static/websocket/message-in-browser.png` & `heizer-999999.dev1681435064/docs/source/_static/websocket/message-in-browser.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/source/_static/websocket/publish-kafka-msg.png` & `heizer-999999.dev1681435064/docs/source/_static/websocket/publish-kafka-msg.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/source/_templates/versions.html` & `heizer-999999.dev1681435064/docs/source/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/source/conf.py` & `heizer-999999.dev1681435064/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/source/tutorial/consumer.rst` & `heizer-999999.dev1681435064/docs/source/tutorial/consumer.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/source/tutorial/prepare.rst` & `heizer-999999.dev1681435064/docs/source/tutorial/prepare.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/docs/source/tutorial/websockets.rst` & `heizer-999999.dev1681435064/docs/source/tutorial/websockets.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/heizer/_source/__init__.py` & `heizer-999999.dev1681435064/heizer/_source/__init__.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/heizer/_source/consumer.py` & `heizer-999999.dev1681435064/heizer/_source/consumer.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/heizer/_source/message.py` & `heizer-999999.dev1681435064/heizer/_source/message.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/heizer/_source/producer.py` & `heizer-999999.dev1681435064/heizer/_source/producer.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/heizer/_source/topic.py` & `heizer-999999.dev1681435064/heizer/_source/topic.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/heizer/config.py` & `heizer-999999.dev1681435064/heizer/config.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/heizer/types.py` & `heizer-999999.dev1681435064/heizer/types.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/heizer.egg-info/PKG-INFO` & `heizer-999999.dev1681435064/heizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1681352876
+Version: 999999.dev1681435064
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,15 +56,15 @@
 A python library to easily create kafka producer and consumer
 
 ## Install
 
 > Note: Heizer is still in development, so you need to install it with `--pre` flag
 
 ```shell
-pip install --pre heizer
+pip install heizer
 ```
 
 ## Setup
 Use `docker-compose.yaml` file to start kafka service
 
 ```shell
 docker-compose up -d
```

### Comparing `heizer-999999.dev1681352876/heizer.egg-info/SOURCES.txt` & `heizer-999999.dev1681435064/heizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/pyproject.toml` & `heizer-999999.dev1681435064/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/samples/websockets/client.html` & `heizer-999999.dev1681435064/samples/websockets/client.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/samples/websockets/server.py` & `heizer-999999.dev1681435064/samples/websockets/server.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681352876/tests/test_consumer.py` & `heizer-999999.dev1681435064/tests/test_consumer.py`

 * *Files identical despite different names*

