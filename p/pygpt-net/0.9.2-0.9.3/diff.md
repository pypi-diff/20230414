# Comparing `tmp/pygpt-net-0.9.2.tar.gz` & `tmp/pygpt-net-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt-net-0.9.2.tar", last modified: Thu Apr 13 23:00:00 2023, max compression
+gzip compressed data, was "pygpt-net-0.9.3.tar", last modified: Fri Apr 14 00:01:14 2023, max compression
```

## Comparing `pygpt-net-0.9.2.tar` & `pygpt-net-0.9.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.153746 pygpt-net-0.9.2/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1077 2023-04-10 01:01:37.000000 pygpt-net-0.9.2/LICENSE
--rw-rw-r--   0 marcin    (1000) marcin    (1000)    17088 2023-04-13 23:00:00.153746 pygpt-net-0.9.2/PKG-INFO
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    15001 2023-04-13 22:59:54.000000 pygpt-net-0.9.2/README.md
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     1146 2023-04-13 22:34:47.000000 pygpt-net-0.9.2/pyproject.toml
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       38 2023-04-13 23:00:00.153746 pygpt-net-0.9.2/setup.cfg
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     1470 2023-04-13 22:09:31.000000 pygpt-net-0.9.2/setup.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.145747 pygpt-net-0.9.2/src/
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.145747 pygpt-net-0.9.2/src/pygpt_net/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      197 2023-04-12 07:50:37.000000 pygpt-net-0.9.2/src/pygpt_net/CHANGELOG.txt
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      844 2023-04-13 21:43:30.000000 pygpt-net-0.9.2/src/pygpt_net/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      553 2023-04-13 21:40:18.000000 pygpt-net-0.9.2/src/pygpt_net/app.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.149747 pygpt-net-0.9.2/src/pygpt_net/core/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.2/src/pygpt_net/core/__init__.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     4245 2023-04-12 18:28:43.000000 pygpt-net-0.9.2/src/pygpt_net/core/app.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)    15100 2023-04-13 21:40:18.000000 pygpt-net-0.9.2/src/pygpt_net/core/config.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)    13292 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/context.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.149747 pygpt-net-0.9.2/src/pygpt_net/core/controller/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/__init__.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1662 2023-04-10 16:42:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/confirm.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     5161 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/context.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1516 2023-04-10 16:42:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/debug.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4793 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/image.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1806 2023-04-10 16:42:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/info.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4325 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/input.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    10565 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/lang.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1340 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/launcher.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1968 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/main.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)    12782 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/model.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3123 2023-04-10 16:42:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/output.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      657 2023-04-10 16:42:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/plugins.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    11561 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/presets.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13921 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/settings.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     7164 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/theme.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2601 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/controller/ui.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.149747 pygpt-net-0.9.2/src/pygpt_net/core/debug/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.2/src/pygpt_net/core/debug/__init__.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      988 2023-04-09 18:49:39.000000 pygpt-net-0.9.2/src/pygpt_net/core/debug/config.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2110 2023-04-10 16:42:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/debug/context.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1554 2023-04-09 18:49:39.000000 pygpt-net-0.9.2/src/pygpt_net/core/debug/models.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1954 2023-04-09 18:49:39.000000 pygpt-net-0.9.2/src/pygpt_net/core/debug/presets.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3699 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/debugger.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9122 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/gpt.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1737 2023-04-10 16:42:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/history.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2467 2023-04-11 05:25:57.000000 pygpt-net-0.9.2/src/pygpt_net/core/image.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      832 2023-04-09 18:49:39.000000 pygpt-net-0.9.2/src/pygpt_net/core/info.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1935 2023-04-13 21:06:16.000000 pygpt-net-0.9.2/src/pygpt_net/core/locale.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2431 2023-04-11 05:19:58.000000 pygpt-net-0.9.2/src/pygpt_net/core/settings.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4501 2023-04-10 16:42:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/tokens.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.149747 pygpt-net-0.9.2/src/pygpt_net/core/ui/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3043 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/chatbox.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3324 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/contexts.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.153746 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3194 2023-04-13 21:40:18.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/about.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1748 2023-04-13 21:40:18.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/changelog.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      966 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/ctx_rename.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1253 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/debug.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2334 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/editor.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1817 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/image.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6330 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/preset.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9119 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/settings.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2324 2023-04-13 21:40:18.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/start.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      822 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/update.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4169 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/dialogs.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3899 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/input.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2426 2023-04-12 19:39:35.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/main.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8459 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/menu.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1008 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/status.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8550 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/toolbox.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    24160 2023-04-13 21:40:18.000000 pygpt-net-0.9.2/src/pygpt_net/core/ui/widgets.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6275 2023-04-13 21:15:52.000000 pygpt-net-0.9.2/src/pygpt_net/core/updater.py
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1220 2023-04-13 18:51:32.000000 pygpt-net-0.9.2/src/pygpt_net/core/utils.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.153746 pygpt-net-0.9.2/src/pygpt_net/data/
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.153746 pygpt-net-0.9.2/src/pygpt_net/data/config/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1052 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/data/config/config.json
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      669 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/data/config/models.json
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.153746 pygpt-net-0.9.2/src/pygpt_net/data/config/presets/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      255 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/data/config/presets/batman_and_joker.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      287 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/data/config/presets/current.chat.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      276 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/data/config/presets/current.completion.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      259 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/data/config/presets/current.img.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      273 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/data/config/presets/dalle_covboy_tokio.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)      525 2023-04-13 21:09:42.000000 pygpt-net-0.9.2/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3461 2023-04-09 19:13:26.000000 pygpt-net-0.9.2/src/pygpt_net/data/icon.ico
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)    13970 2023-04-09 19:12:56.000000 pygpt-net-0.9.2/src/pygpt_net/data/icon.png
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.153746 pygpt-net-0.9.2/src/pygpt_net/data/locale/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5410 2023-04-12 07:50:37.000000 pygpt-net-0.9.2/src/pygpt_net/data/locale/locale.en.ini
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5935 2023-04-12 07:50:37.000000 pygpt-net-0.9.2/src/pygpt_net/data/locale/locale.pl.ini
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9703 2023-04-09 19:29:44.000000 pygpt-net-0.9.2/src/pygpt_net/data/logo.png
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-13 23:00:00.149747 pygpt-net-0.9.2/src/pygpt_net.egg-info/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)    17088 2023-04-13 23:00:00.000000 pygpt-net-0.9.2/src/pygpt_net.egg-info/PKG-INFO
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     2939 2023-04-13 23:00:00.000000 pygpt-net-0.9.2/src/pygpt_net.egg-info/SOURCES.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)        1 2023-04-13 23:00:00.000000 pygpt-net-0.9.2/src/pygpt_net.egg-info/dependency_links.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       49 2023-04-13 23:00:00.000000 pygpt-net-0.9.2/src/pygpt_net.egg-info/entry_points.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      138 2023-04-13 23:00:00.000000 pygpt-net-0.9.2/src/pygpt_net.egg-info/requires.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       10 2023-04-13 23:00:00.000000 pygpt-net-0.9.2/src/pygpt_net.egg-info/top_level.txt
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1077 2023-04-10 01:01:37.000000 pygpt-net-0.9.3/LICENSE
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)    17182 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/PKG-INFO
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    15095 2023-04-14 00:01:05.000000 pygpt-net-0.9.3/README.md
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     1146 2023-04-13 23:56:48.000000 pygpt-net-0.9.3/pyproject.toml
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       38 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/setup.cfg
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     1470 2023-04-13 23:56:48.000000 pygpt-net-0.9.3/setup.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.015881 pygpt-net-0.9.3/src/
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      245 2023-04-13 23:56:48.000000 pygpt-net-0.9.3/src/pygpt_net/CHANGELOG.txt
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      844 2023-04-13 23:56:48.000000 pygpt-net-0.9.3/src/pygpt_net/__init__.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      553 2023-04-13 21:40:18.000000 pygpt-net-0.9.3/src/pygpt_net/app.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net/core/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/__init__.py
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     4245 2023-04-12 18:28:43.000000 pygpt-net-0.9.3/src/pygpt_net/core/app.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    15134 2023-04-13 23:44:00.000000 pygpt-net-0.9.3/src/pygpt_net/core/config.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    13292 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/context.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net/core/controller/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1662 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/confirm.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     5161 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/context.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1516 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/debug.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4793 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/image.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1806 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/info.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4325 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/input.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    10565 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/lang.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1340 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/launcher.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1968 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/main.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    12782 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/model.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3123 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/output.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      657 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/plugins.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    11561 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/presets.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13921 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/settings.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     7164 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/theme.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2601 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/controller/ui.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net/core/debug/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      988 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/config.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2110 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/context.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1554 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/models.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1954 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/debug/presets.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3699 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/debugger.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9122 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/gpt.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1737 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/history.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2467 2023-04-11 05:25:57.000000 pygpt-net-0.9.3/src/pygpt_net/core/image.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      832 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/info.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1926 2023-04-13 23:39:46.000000 pygpt-net-0.9.3/src/pygpt_net/core/locale.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2431 2023-04-11 05:19:58.000000 pygpt-net-0.9.3/src/pygpt_net/core/settings.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4501 2023-04-10 16:42:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/tokens.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/core/ui/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/__init__.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3043 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/chatbox.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3324 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/contexts.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-09 18:49:39.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/__init__.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3170 2023-04-13 23:41:43.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/about.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1724 2023-04-13 23:40:57.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/changelog.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      966 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/ctx_rename.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1253 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/debug.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2334 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/editor.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1817 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/image.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6330 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/preset.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9119 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/settings.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2300 2023-04-13 23:40:50.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/start.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      822 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/update.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4169 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/dialogs.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3899 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/input.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2426 2023-04-12 19:39:35.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/main.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8459 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/menu.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1008 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/status.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8550 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/toolbox.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    24147 2023-04-13 23:40:34.000000 pygpt-net-0.9.3/src/pygpt_net/core/ui/widgets.py
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6275 2023-04-13 21:15:52.000000 pygpt-net-0.9.3/src/pygpt_net/core/updater.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1220 2023-04-13 18:51:32.000000 pygpt-net-0.9.3/src/pygpt_net/core/utils.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/data/
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/data/config/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1052 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/config.json
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)      669 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/models.json
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      255 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      287 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/current.chat.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      276 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/current.completion.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      259 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/current.img.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      273 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/dalle_covboy_tokio.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      525 2023-04-13 21:09:42.000000 pygpt-net-0.9.3/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3461 2023-04-09 19:13:26.000000 pygpt-net-0.9.3/src/pygpt_net/data/icon.ico
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    13970 2023-04-09 19:12:56.000000 pygpt-net-0.9.3/src/pygpt_net/data/icon.png
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.023881 pygpt-net-0.9.3/src/pygpt_net/data/locale/
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5410 2023-04-12 07:50:37.000000 pygpt-net-0.9.3/src/pygpt_net/data/locale/locale.en.ini
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5935 2023-04-12 07:50:37.000000 pygpt-net-0.9.3/src/pygpt_net/data/locale/locale.pl.ini
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9703 2023-04-09 19:29:44.000000 pygpt-net-0.9.3/src/pygpt_net/data/logo.png
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-14 00:01:14.019881 pygpt-net-0.9.3/src/pygpt_net.egg-info/
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)    17182 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/PKG-INFO
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     2939 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)        1 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       49 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/entry_points.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)      138 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/requires.txt
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       10 2023-04-14 00:01:14.000000 pygpt-net-0.9.3/src/pygpt_net.egg-info/top_level.txt
```

### Comparing `pygpt-net-0.9.2/LICENSE` & `pygpt-net-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/PKG-INFO` & `pygpt-net-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 0.9.2
+Version: 0.9.3
 Summary: A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation
 Home-page: https://github.com/szczyglis-dev/py-gpt
 Author: Marcin Szczygliński
 Author-email: Marcin Szczygliński <info@pygpt.net>
 Maintainer: Marcin Szczygliński
 Maintainer-email: info@pygpt.net
 License: MIT License
@@ -34,20 +34,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Current release: **0.9.2** (build: **2023.04.12**)
+Current release: **0.9.3** (build: **2023.04.14**)
 
 Official website: https://pygpt.net
 
 Documentation: https://pygpt.readthedocs.io
 
+PyPi: https://pypi.org/project/pygpt-net
+
 ### **Compiled binary versions for Windows 10, 11 and Linux are available to download on project's page**: https://pygpt.net (in "Download" section)
 
 # PYGPT
 
 ## What is PYGPT?
 
 **PYGPT** is a desktop application that allows you to talk to OpenAI\'s
@@ -488,14 +490,18 @@
 
 Support for plug-ins and voice recognition and synthesis will be added
 in future versions of the application.
 
 
 # CHANGELOG
 
+## v0.9.3 (2023.04.13)
+
+- packed into PyPI package
+
 ## v0.9.2 (2023.04.12)
 
 - added theme color settings
 - small UI fixes
 
 ## v0.9.1 (2023.04.11)
```

### Comparing `pygpt-net-0.9.2/README.md` & `pygpt-net-0.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-Current release: **0.9.2** (build: **2023.04.12**)
+Current release: **0.9.3** (build: **2023.04.14**)
 
 Official website: https://pygpt.net
 
 Documentation: https://pygpt.readthedocs.io
 
+PyPi: https://pypi.org/project/pygpt-net
+
 ### **Compiled binary versions for Windows 10, 11 and Linux are available to download on project's page**: https://pygpt.net (in "Download" section)
 
 # PYGPT
 
 ## What is PYGPT?
 
 **PYGPT** is a desktop application that allows you to talk to OpenAI\'s
@@ -448,14 +450,18 @@
 
 Support for plug-ins and voice recognition and synthesis will be added
 in future versions of the application.
 
 
 # CHANGELOG
 
+## v0.9.3 (2023.04.13)
+
+- packed into PyPI package
+
 ## v0.9.2 (2023.04.12)
 
 - added theme color settings
 - small UI fixes
 
 ## v0.9.1 (2023.04.11)
```

### Comparing `pygpt-net-0.9.2/pyproject.toml` & `pygpt-net-0.9.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygpt-net"
-version = "0.9.2"
+version = "0.9.3"
 description = "A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation"
 readme = "README.md"
 authors = [{ name = "Marcin Szczygliński", email = "info@pygpt.net" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pygpt-net-0.9.2/setup.py` & `pygpt-net-0.9.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.9.2'
+VERSION = '0.9.3'
 DESCRIPTION = 'A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation'
 LONG_DESCRIPTION = 'A package containing a GPT4, GPT3, ChatGPT and DALL-E 2 desktop chatbot, ' \
                    'text completion and image generation app, using OpenAI API and your own API Key. ' \
                    'It includes context memory and history, editable presets, customizable UI and more.'
 
 setup(
     name='pygpt-net',
```

### Comparing `pygpt-net-0.9.2/src/pygpt_net/__init__.py` & `pygpt-net-0.9.3/src/pygpt_net/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 # Updated Date: 2023.04.12 09:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2023, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "0.9.2"
-__build__ = "2023.04.12"
+__version__ = "0.9.3"
+__build__ = "2023.04.14"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __email__ = "info@pygpt.net"
```

### Comparing `pygpt-net-0.9.2/src/pygpt_net/app.py` & `pygpt-net-0.9.3/src/pygpt_net/app.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/app.py` & `pygpt-net-0.9.3/src/pygpt_net/core/app.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/config.py` & `pygpt-net-0.9.3/src/pygpt_net/core/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,30 +29,33 @@
         self.path = str(Path(os.path.join(Path.home(), '.config', self.CONFIG_DIR)))
         self.initialized = False
         self.models = {}
         self.data = {}
         self.presets = {}
         self.version = self.get_version()
 
-    def get_local_data_path(self):
+    def get_root_path(self):
         """
         Returns local data path
 
         :return: local data path
         """
-        return os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, 'data'))
+        if __file__.endswith('.pyc'):  # if compiled with pyinstaller
+            return os.path.abspath('.')
+        else:
+            return os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir))
 
     def get_available_langs(self):
         """
         Returns list with available languages
 
         :return: list with available languages
         """
         langs = []
-        path = os.path.join(os.path.dirname(__file__), os.pardir, 'data', 'locale')
+        path = os.path.join(self.get_root_path(), 'data', 'locale')
         if not os.path.exists(path):
             return langs
 
         for file in os.listdir(path):
             if file.endswith(".ini"):
                 langs.append(file.replace('locale.', '').replace('.ini', ''))
 
@@ -75,15 +78,15 @@
 
     def get_version(self):
         """
         Returns version
 
         :return: version string
         """
-        path = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, '__init__.py'))
+        path = os.path.abspath(os.path.join(self.get_root_path(), '__init__.py'))
         result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format("__version__"),
                            open(path).read())
         return result.group(1)
 
     def load(self, all=True):
         """
         Loads config
@@ -475,27 +478,27 @@
             # create user config directory
             path = Path(self.path)
             path.mkdir(parents=True, exist_ok=True)
 
             # install config file
             dst = os.path.join(self.path, 'config.json')
             if not os.path.exists(dst):
-                src = os.path.join(os.path.dirname(__file__), os.pardir, 'data', 'config', 'config.json')
+                src = os.path.join(self.get_root_path(), 'data', 'config', 'config.json')
                 shutil.copyfile(src, dst)
 
             # install models file
             dst = os.path.join(self.path, 'models.json')
             if not os.path.exists(dst):
-                src = os.path.join(os.path.dirname(__file__), os.pardir, 'data', 'config', 'models.json')
+                src = os.path.join(self.get_root_path(), 'data', 'config', 'models.json')
                 shutil.copyfile(src, dst)
 
             # install prompt presets
             presets_dir = os.path.join(self.path, 'presets')
             if not os.path.exists(presets_dir):
-                src = os.path.join(os.path.dirname(__file__), os.pardir, 'data', 'config', 'presets')
+                src = os.path.join(self.get_root_path(), 'data', 'config', 'presets')
                 shutil.copytree(src, presets_dir)
 
             # create history directory
             history_dir = os.path.join(self.path, 'history')
             if not os.path.exists(history_dir):
                 os.mkdir(history_dir)
```

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/context.py` & `pygpt-net-0.9.3/src/pygpt_net/core/context.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/confirm.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/context.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/context.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/debug.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/image.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/image.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/info.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/info.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/input.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/input.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/lang.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/lang.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/launcher.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/main.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/main.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/model.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/model.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/output.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/output.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/plugins.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/presets.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/settings.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/theme.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/theme.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/controller/ui.py` & `pygpt-net-0.9.3/src/pygpt_net/core/controller/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/debug/config.py` & `pygpt-net-0.9.3/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/debug/context.py` & `pygpt-net-0.9.3/src/pygpt_net/core/debug/context.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/debug/models.py` & `pygpt-net-0.9.3/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/debug/presets.py` & `pygpt-net-0.9.3/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/debugger.py` & `pygpt-net-0.9.3/src/pygpt_net/core/debugger.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/gpt.py` & `pygpt-net-0.9.3/src/pygpt_net/core/gpt.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/history.py` & `pygpt-net-0.9.3/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/image.py` & `pygpt-net-0.9.3/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/info.py` & `pygpt-net-0.9.3/src/pygpt_net/core/info.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/locale.py` & `pygpt-net-0.9.3/src/pygpt_net/core/locale.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """
         Loads translation ini file
 
         :param lang: language code
         """
         if type(lang) is not str:
             lang = 'en'
-        path = os.path.join(os.path.dirname(__file__), os.pardir, 'data', 'locale', 'locale.' + lang + '.ini')
+        path = os.path.join(self.config.get_root_path(), 'data', 'locale', 'locale.' + lang + '.ini')
         if not os.path.exists(path):
             print("FATAL ERROR: {} not found!".format(path))
             return None
         try:
             ini = configparser.ConfigParser()
             data = io.open(path, mode="r", encoding="utf-8")
             ini.read_string(data.read())
```

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/settings.py` & `pygpt-net-0.9.3/src/pygpt_net/core/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/tokens.py` & `pygpt-net-0.9.3/src/pygpt_net/core/tokens.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/chatbox.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/chatbox.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/contexts.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/contexts.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/about.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/about.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.window = window
 
     def setup(self):
         """Setups about dialog"""
         id = 'about'
 
         logo_label = QLabel()
-        path = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, os.pardir, os.pardir, 'data', 'logo.png'))
+        path = os.path.abspath(os.path.join(self.window.config.get_root_path(), 'data', 'logo.png'))
         pixmap = QPixmap(path)
         logo_label.setPixmap(pixmap)
 
         btn_www = QPushButton('WWW')
         btn_www.clicked.connect(lambda: self.window.controller.info.goto_website())
 
         btn_github = QPushButton('GitHub')
```

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/changelog.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/changelog.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def setup(self):
         """Setups change log dialog"""
         id = 'changelog'
 
         txt = ''
         try:
-            with open(os.path.join(os.path.dirname(__file__), os.pardir, os.pardir, os.pardir,
+            with open(os.path.join(self.window.config.get_root_path(),
                                    "CHANGELOG.txt"), "r") as f:
                 txt = f.read()
                 f.close()
         except Exception as e:
             print(e)
 
         textarea = QPlainTextEdit()
```

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/ctx_rename.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/ctx_rename.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/debug.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/editor.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/image.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/preset.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/settings.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/start.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/start.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         id = 'start'
 
         self.window.data['start.btn'] = QPushButton(trans('dialog.start.btn'))
         self.window.data['start.btn'].clicked.connect(lambda: self.window.controller.settings.start_settings())
 
         logo_label = QLabel()
         path = os.path.abspath(
-            os.path.join(os.path.dirname(__file__), os.pardir, os.pardir, os.pardir, 'data', 'logo.png'))
+            os.path.join(self.window.config.get_root_path(), 'data', 'logo.png'))
         pixmap = QPixmap(path)
         logo_label.setPixmap(pixmap)
 
         self.window.data['start.title'] = QLabel(trans('dialog.start.title.text'))
         link = QLabel(trans('dialog.start.link'))
         self.window.data['start.settings'] = QLabel(trans('dialog.start.settings.text'))
         self.window.data['start.settings'].setAlignment(Qt.AlignCenter)
```

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialog/update.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/dialogs.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/input.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/input.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/main.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/main.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/menu.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/menu.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/status.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/status.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/toolbox.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/toolbox.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/ui/widgets.py` & `pygpt-net-0.9.3/src/pygpt_net/core/ui/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,15 +641,15 @@
         self.changelog = QPlainTextEdit()
         self.changelog.setReadOnly(True)
         self.changelog.setMaximumWidth(400)
         self.changelog.setMaximumHeight(200)
 
         logo_label = QLabel()
         path = os.path.abspath(
-            os.path.join(os.path.dirname(__file__), os.pardir, os.pardir, 'data', 'logo.png'))
+            os.path.join(self.window.config.get_root_path(), 'data', 'logo.png'))
         pixmap = QPixmap(path)
         logo_label.setPixmap(pixmap)
 
         self.layout = QVBoxLayout()
         self.message = QLabel("")
         info = QLabel(trans("update.info"))
         info.setWordWrap(True)
```

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/updater.py` & `pygpt-net-0.9.3/src/pygpt_net/core/updater.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/core/utils.py` & `pygpt-net-0.9.3/src/pygpt_net/core/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/data/config/config.json` & `pygpt-net-0.9.3/src/pygpt_net/data/config/config.json`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/data/config/models.json` & `pygpt-net-0.9.3/src/pygpt_net/data/config/models.json`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json` & `pygpt-net-0.9.3/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/data/icon.ico` & `pygpt-net-0.9.3/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/data/icon.png` & `pygpt-net-0.9.3/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/data/locale/locale.en.ini` & `pygpt-net-0.9.3/src/pygpt_net/data/locale/locale.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt-net-0.9.3/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net/data/logo.png` & `pygpt-net-0.9.3/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.2/src/pygpt_net.egg-info/PKG-INFO` & `pygpt-net-0.9.3/src/pygpt_net.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 0.9.2
+Version: 0.9.3
 Summary: A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation
 Home-page: https://github.com/szczyglis-dev/py-gpt
 Author: Marcin Szczygliński
 Author-email: Marcin Szczygliński <info@pygpt.net>
 Maintainer: Marcin Szczygliński
 Maintainer-email: info@pygpt.net
 License: MIT License
@@ -34,20 +34,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Current release: **0.9.2** (build: **2023.04.12**)
+Current release: **0.9.3** (build: **2023.04.14**)
 
 Official website: https://pygpt.net
 
 Documentation: https://pygpt.readthedocs.io
 
+PyPi: https://pypi.org/project/pygpt-net
+
 ### **Compiled binary versions for Windows 10, 11 and Linux are available to download on project's page**: https://pygpt.net (in "Download" section)
 
 # PYGPT
 
 ## What is PYGPT?
 
 **PYGPT** is a desktop application that allows you to talk to OpenAI\'s
@@ -488,14 +490,18 @@
 
 Support for plug-ins and voice recognition and synthesis will be added
 in future versions of the application.
 
 
 # CHANGELOG
 
+## v0.9.3 (2023.04.13)
+
+- packed into PyPI package
+
 ## v0.9.2 (2023.04.12)
 
 - added theme color settings
 - small UI fixes
 
 ## v0.9.1 (2023.04.11)
```

### Comparing `pygpt-net-0.9.2/src/pygpt_net.egg-info/SOURCES.txt` & `pygpt-net-0.9.3/src/pygpt_net.egg-info/SOURCES.txt`

 * *Files identical despite different names*

