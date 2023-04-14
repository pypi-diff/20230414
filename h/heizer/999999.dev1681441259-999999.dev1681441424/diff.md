# Comparing `tmp/heizer-999999.dev1681441259.tar.gz` & `tmp/heizer-999999.dev1681441424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heizer-999999.dev1681441259.tar", last modified: Fri Apr 14 03:01:07 2023, max compression
+gzip compressed data, was "heizer-999999.dev1681441424.tar", last modified: Fri Apr 14 03:03:52 2023, max compression
```

## Comparing `heizer-999999.dev1681441259.tar` & `heizer-999999.dev1681441424.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.043470 heizer-999999.dev1681441259/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.github/workflows/deploy-latest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 03:00:56.000000 heizer-999999.dev1681441259/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/img1.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/source/_static/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_static/websocket/create-topic.png
--rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_static/websocket/message-in-browser.png
--rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_static/websocket/publish-kafka-msg.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.047470 heizer-999999.dev1681441259/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/heizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/tutorial/consumer.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/tutorial/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/docs/source/tutorial/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/heizer/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 03:00:59.000000 heizer-999999.dev1681441259/heizer/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/heizer/_source/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/_source/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/heizer/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/heizer/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/heizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 03:01:07.000000 heizer-999999.dev1681441259/heizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/samples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/samples/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/samples/websockets/client.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/samples/websockets/server.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:01:07.051471 heizer-999999.dev1681441259/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-14 03:00:57.000000 heizer-999999.dev1681441259/tests/test_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.040470 heizer-999999.dev1681441424/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.040470 heizer-999999.dev1681441424/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/.github/workflows/deploy-latest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.040470 heizer-999999.dev1681441424/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/img1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.040470 heizer-999999.dev1681441424/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.040470 heizer-999999.dev1681441424/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.040470 heizer-999999.dev1681441424/docs/source/_static/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/_static/websocket/create-topic.png
+-rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/_static/websocket/message-in-browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/_static/websocket/publish-kafka-msg.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/heizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/tutorial/consumer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/tutorial/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/docs/source/tutorial/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/heizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 03:03:44.000000 heizer-999999.dev1681441424/heizer/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/heizer/_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/_source/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/_source/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/_source/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/_source/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/_source/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/heizer/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/heizer/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/heizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-14 03:03:52.000000 heizer-999999.dev1681441424/heizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 03:03:52.000000 heizer-999999.dev1681441424/heizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:03:52.000000 heizer-999999.dev1681441424/heizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 03:03:52.000000 heizer-999999.dev1681441424/heizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 03:03:52.000000 heizer-999999.dev1681441424/heizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/samples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/samples/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/samples/websockets/client.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/samples/websockets/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:52.044470 heizer-999999.dev1681441424/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-14 03:03:42.000000 heizer-999999.dev1681441424/tests/test_consumer.py
```

### Comparing `heizer-999999.dev1681441259/.github/workflows/deploy-latest.yml` & `heizer-999999.dev1681441424/.github/workflows/deploy-latest.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/.github/workflows/main.yml` & `heizer-999999.dev1681441424/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/.github/workflows/release.yml` & `heizer-999999.dev1681441424/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/.gitignore` & `heizer-999999.dev1681441424/.gitignore`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/.pre-commit-config.yaml` & `heizer-999999.dev1681441424/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/LICENSE` & `heizer-999999.dev1681441424/LICENSE`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/PKG-INFO` & `heizer-999999.dev1681441424/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1681441259
+Version: 999999.dev1681441424
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `heizer-999999.dev1681441259/README.md` & `heizer-999999.dev1681441424/README.md`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docker-compose.yaml` & `heizer-999999.dev1681441424/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/Makefile` & `heizer-999999.dev1681441424/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/img1.png` & `heizer-999999.dev1681441424/docs/img1.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/make.bat` & `heizer-999999.dev1681441424/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/source/_static/websocket/create-topic.png` & `heizer-999999.dev1681441424/docs/source/_static/websocket/create-topic.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/source/_static/websocket/message-in-browser.png` & `heizer-999999.dev1681441424/docs/source/_static/websocket/message-in-browser.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/source/_static/websocket/publish-kafka-msg.png` & `heizer-999999.dev1681441424/docs/source/_static/websocket/publish-kafka-msg.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/source/_templates/versions.html` & `heizer-999999.dev1681441424/docs/source/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/source/conf.py` & `heizer-999999.dev1681441424/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/source/tutorial/consumer.rst` & `heizer-999999.dev1681441424/docs/source/tutorial/consumer.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/source/tutorial/prepare.rst` & `heizer-999999.dev1681441424/docs/source/tutorial/prepare.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/docs/source/tutorial/websockets.rst` & `heizer-999999.dev1681441424/docs/source/tutorial/websockets.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/heizer/_source/__init__.py` & `heizer-999999.dev1681441424/heizer/_source/__init__.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/heizer/_source/admin.py` & `heizer-999999.dev1681441424/heizer/_source/admin.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/heizer/_source/consumer.py` & `heizer-999999.dev1681441424/heizer/_source/consumer.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/heizer/_source/message.py` & `heizer-999999.dev1681441424/heizer/_source/message.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/heizer/_source/producer.py` & `heizer-999999.dev1681441424/heizer/_source/producer.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/heizer/_source/topic.py` & `heizer-999999.dev1681441424/heizer/_source/topic.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/heizer/config.py` & `heizer-999999.dev1681441424/heizer/config.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/heizer/types.py` & `heizer-999999.dev1681441424/heizer/types.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/heizer.egg-info/PKG-INFO` & `heizer-999999.dev1681441424/heizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1681441259
+Version: 999999.dev1681441424
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `heizer-999999.dev1681441259/heizer.egg-info/SOURCES.txt` & `heizer-999999.dev1681441424/heizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/pyproject.toml` & `heizer-999999.dev1681441424/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/samples/websockets/client.html` & `heizer-999999.dev1681441424/samples/websockets/client.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/samples/websockets/server.py` & `heizer-999999.dev1681441424/samples/websockets/server.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441259/tests/test_consumer.py` & `heizer-999999.dev1681441424/tests/test_consumer.py`

 * *Files identical despite different names*

