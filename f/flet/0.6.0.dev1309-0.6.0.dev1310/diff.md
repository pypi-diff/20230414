# Comparing `tmp/flet-0.6.0.dev1309.tar.gz` & `tmp/flet-0.6.0.dev1310.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-0.6.0.dev1309.tar", max compression
+gzip compressed data, was "flet-0.6.0.dev1310.tar", max compression
```

## Comparing `flet-0.6.0.dev1309.tar` & `flet-0.6.0.dev1310.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     2145 2023-04-14 16:39:07.411338 flet-0.6.0.dev1309/README.md
--rw-r--r--   0        0        0     1066 2023-04-14 16:39:41.086890 flet-0.6.0.dev1309/pyproject.toml
--rw-r--r--   0        0        0      155 2023-04-14 16:39:07.411338 flet-0.6.0.dev1309/src/flet/__init__.py
--rw-r--r--   0        0        0       72 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/__pyinstaller/__init__.py
--rw-r--r--   0        0        0       20 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/__pyinstaller/config.py
--rw-r--r--   0        0        0      378 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/__pyinstaller/hook-flet.py
--rw-r--r--   0        0        0     2985 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/__pyinstaller/macos_utils.py
--rw-r--r--   0        0        0      187 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
--rw-r--r--   0        0        0       61 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/__pyinstaller/rthooks.dat
--rw-r--r--   0        0        0      562 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/__pyinstaller/utils.py
--rw-r--r--   0        0        0     3636 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/__pyinstaller/win_utils.py
--rw-r--r--   0        0        0     6192 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/async_local_socket_connection.py
--rw-r--r--   0        0        0     7183 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/async_websocket_connection.py
--rw-r--r--   0        0        0     9083 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/auth/authorization.py
--rw-r--r--   0        0        0      128 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/auth/group.py
--rw-r--r--   0        0        0     1499 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/auth/oauth_token.py
--rw-r--r--   0        0        0      735 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      840 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3669 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      799 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      182 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/auth/user.py
--rw-r--r--   0        0        0     2958 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/cli/cli.py
--rw-r--r--   0        0        0     1953 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/cli/commands/base.py
--rw-r--r--   0        0        0      673 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/cli/commands/options.py
--rw-r--r--   0        0        0     8449 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/cli/commands/pack.py
--rw-r--r--   0        0        0     8885 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/cli/commands/publish.py
--rw-r--r--   0        0        0     6711 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/cli/commands/run.py
--rw-r--r--   0        0        0       52 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/constants.py
--rw-r--r--   0        0        0    21493 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/plotly_chart.py
--rw-r--r--   0        0        0    10239 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/pubsub.py
--rw-r--r--   0        0        0     3046 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/reconnecting_websocket.py
--rw-r--r--   0        0        0     1272 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/security.py
--rw-r--r--   0        0        0     6843 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/sync_local_socket_connection.py
--rw-r--r--   0        0        0     5396 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/sync_websocket_connection.py
--rw-r--r--   0        0        0     6955 2023-04-14 16:39:07.415338 flet-0.6.0.dev1309/src/flet/utils.py
--rw-r--r--   0        0        0     1431 2023-04-14 16:39:40.874890 flet-0.6.0.dev1309/src/flet/version.py
--rw-r--r--   0        0        0       32 2023-04-14 16:29:35.000000 flet-0.6.0.dev1309/src/flet/web/.last_build_id
--rw-r--r--   0        0        0      455 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/assets/AssetManifest.json
--rw-r--r--   0        0        0       82 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/assets/FontManifest.json
--rw-r--r--   0        0        0   916508 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/assets/NOTICES
--rw-r--r--   0        0        0  1645184 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
--rw-r--r--   0        0        0      298 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
--rw-r--r--   0        0        0      271 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
--rw-r--r--   0        0        0      166 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
--rw-r--r--   0        0        0      366 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
--rw-r--r--   0        0        0     1028 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/favicon.png
--rw-r--r--   0        0        0    13910 2023-04-14 16:28:17.000000 flet-0.6.0.dev1309/src/flet/web/flutter.js
--rw-r--r--   0        0        0     7836 2023-04-14 16:29:35.000000 flet-0.6.0.dev1309/src/flet/web/flutter_service_worker.js
--rw-r--r--   0        0        0     4699 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/icons/apple-touch-icon-192.png
--rw-r--r--   0        0        0     6622 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/icons/icon-192.png
--rw-r--r--   0        0        0    18666 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/icons/icon-512.png
--rw-r--r--   0        0        0     4128 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    11906 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    17040 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/icons/loading-animation.png
--rw-r--r--   0        0        0     2972 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/index.html
--rw-r--r--   0        0        0  5302239 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/main.dart.js
--rw-r--r--   0        0        0      789 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/manifest.json
--rw-r--r--   0        0        0     1573 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/python-worker.js
--rw-r--r--   0        0        0      744 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/python.js
--rw-r--r--   0        0        0       92 2023-04-14 16:29:34.000000 flet-0.6.0.dev1309/src/flet/web/version.json
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.6.0.dev1309/PKG-INFO
+-rw-r--r--   0        0        0     2145 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/README.md
+-rw-r--r--   0        0        0     1066 2023-04-14 17:13:00.351077 flet-0.6.0.dev1310/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/__init__.py
+-rw-r--r--   0        0        0       72 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0       20 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/__pyinstaller/config.py
+-rw-r--r--   0        0        0      378 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/__pyinstaller/hook-flet.py
+-rw-r--r--   0        0        0     2985 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/__pyinstaller/macos_utils.py
+-rw-r--r--   0        0        0      187 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
+-rw-r--r--   0        0        0       61 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/__pyinstaller/rthooks.dat
+-rw-r--r--   0        0        0      562 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/__pyinstaller/utils.py
+-rw-r--r--   0        0        0     3636 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/__pyinstaller/win_utils.py
+-rw-r--r--   0        0        0     6192 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/async_local_socket_connection.py
+-rw-r--r--   0        0        0     7183 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/async_websocket_connection.py
+-rw-r--r--   0        0        0     9083 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/auth/group.py
+-rw-r--r--   0        0        0     1499 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/auth/oauth_token.py
+-rw-r--r--   0        0        0      735 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      840 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3669 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      799 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      182 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/auth/user.py
+-rw-r--r--   0        0        0     2958 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/cli/cli.py
+-rw-r--r--   0        0        0     1953 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/cli/commands/base.py
+-rw-r--r--   0        0        0      673 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/cli/commands/options.py
+-rw-r--r--   0        0        0     8449 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/cli/commands/pack.py
+-rw-r--r--   0        0        0     8885 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/cli/commands/publish.py
+-rw-r--r--   0        0        0     6711 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/cli/commands/run.py
+-rw-r--r--   0        0        0       52 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/constants.py
+-rw-r--r--   0        0        0    21493 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0    10239 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/pubsub.py
+-rw-r--r--   0        0        0     3046 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/reconnecting_websocket.py
+-rw-r--r--   0        0        0     1272 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/security.py
+-rw-r--r--   0        0        0     6843 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     5396 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/sync_websocket_connection.py
+-rw-r--r--   0        0        0     6955 2023-04-14 17:12:25.302516 flet-0.6.0.dev1310/src/flet/utils.py
+-rw-r--r--   0        0        0     1431 2023-04-14 17:13:00.123074 flet-0.6.0.dev1310/src/flet/version.py
+-rw-r--r--   0        0        0       32 2023-04-14 17:04:47.000000 flet-0.6.0.dev1310/src/flet/web/.last_build_id
+-rw-r--r--   0        0        0      455 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/assets/AssetManifest.json
+-rw-r--r--   0        0        0       82 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/assets/FontManifest.json
+-rw-r--r--   0        0        0   916508 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/assets/NOTICES
+-rw-r--r--   0        0        0  1645184 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
+-rw-r--r--   0        0        0      298 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
+-rw-r--r--   0        0        0      271 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
+-rw-r--r--   0        0        0      166 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
+-rw-r--r--   0        0        0      366 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
+-rw-r--r--   0        0        0     1028 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/favicon.png
+-rw-r--r--   0        0        0    13910 2023-04-14 17:03:34.000000 flet-0.6.0.dev1310/src/flet/web/flutter.js
+-rw-r--r--   0        0        0     7836 2023-04-14 17:04:47.000000 flet-0.6.0.dev1310/src/flet/web/flutter_service_worker.js
+-rw-r--r--   0        0        0     4699 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/icons/apple-touch-icon-192.png
+-rw-r--r--   0        0        0     6622 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/icons/icon-192.png
+-rw-r--r--   0        0        0    18666 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/icons/icon-512.png
+-rw-r--r--   0        0        0     4128 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    11906 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    17040 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/icons/loading-animation.png
+-rw-r--r--   0        0        0     2972 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/index.html
+-rw-r--r--   0        0        0  5302323 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/main.dart.js
+-rw-r--r--   0        0        0      789 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/manifest.json
+-rw-r--r--   0        0        0     1573 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/python-worker.js
+-rw-r--r--   0        0        0      744 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/python.js
+-rw-r--r--   0        0        0       92 2023-04-14 17:04:46.000000 flet-0.6.0.dev1310/src/flet/web/version.json
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.6.0.dev1310/PKG-INFO
```

### Comparing `flet-0.6.0.dev1309/README.md` & `flet-0.6.0.dev1310/README.md`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/pyproject.toml` & `flet-0.6.0.dev1310/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet"
-version = "0.6.0.dev1309"
+version = "0.6.0.dev1310"
 description = "Flet for Python - easily build interactive multi-platform apps in Python"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.6.0.dev1309"
+flet-core = "0.6.0.dev1310"
 python = "^3.7"
 typing-extensions = { version = "^4.4.0", python = "<3.8" }
 websocket-client = "^1.4.2"
 watchdog = "^2.2.1"
 oauthlib = "^3.2.2"
 websockets = "^10.4"
 httpx = "^0.23.3"
```

### Comparing `flet-0.6.0.dev1309/src/flet/__pyinstaller/macos_utils.py` & `flet-0.6.0.dev1310/src/flet/__pyinstaller/macos_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/__pyinstaller/utils.py` & `flet-0.6.0.dev1310/src/flet/__pyinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/__pyinstaller/win_utils.py` & `flet-0.6.0.dev1310/src/flet/__pyinstaller/win_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/async_local_socket_connection.py` & `flet-0.6.0.dev1310/src/flet/async_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/async_websocket_connection.py` & `flet-0.6.0.dev1310/src/flet/async_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/auth/authorization.py` & `flet-0.6.0.dev1310/src/flet/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/auth/oauth_provider.py` & `flet-0.6.0.dev1310/src/flet/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/auth/oauth_token.py` & `flet-0.6.0.dev1310/src/flet/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/auth/providers/auth0_oauth_provider.py` & `flet-0.6.0.dev1310/src/flet/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/auth/providers/azure_oauth_provider.py` & `flet-0.6.0.dev1310/src/flet/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/auth/providers/github_oauth_provider.py` & `flet-0.6.0.dev1310/src/flet/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/auth/providers/google_oauth_provider.py` & `flet-0.6.0.dev1310/src/flet/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/cli/cli.py` & `flet-0.6.0.dev1310/src/flet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/cli/commands/base.py` & `flet-0.6.0.dev1310/src/flet/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/cli/commands/options.py` & `flet-0.6.0.dev1310/src/flet/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/cli/commands/pack.py` & `flet-0.6.0.dev1310/src/flet/cli/commands/pack.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/cli/commands/publish.py` & `flet-0.6.0.dev1310/src/flet/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/cli/commands/run.py` & `flet-0.6.0.dev1310/src/flet/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/flet.py` & `flet-0.6.0.dev1310/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/pubsub.py` & `flet-0.6.0.dev1310/src/flet/pubsub.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/reconnecting_websocket.py` & `flet-0.6.0.dev1310/src/flet/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/security.py` & `flet-0.6.0.dev1310/src/flet/security.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/sync_local_socket_connection.py` & `flet-0.6.0.dev1310/src/flet/sync_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/sync_websocket_connection.py` & `flet-0.6.0.dev1310/src/flet/sync_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/utils.py` & `flet-0.6.0.dev1310/src/flet/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/version.py` & `flet-0.6.0.dev1310/src/flet/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess as sp
 from pathlib import Path
 
 import flet
 from flet.utils import is_windows, which
 
 # this value will be replaced by CI
-version = "0.6.0.dev1309"
+version = "0.6.0.dev1310"
 
 
 def update_version():
     """Return the current version or default."""
     working = Path().absolute()
     os.chdir(Path(flet.__file__).absolute().parent)
     in_repo = which("git.exe" if is_windows() else "git") and sp.run(
```

### Comparing `flet-0.6.0.dev1309/src/flet/web/assets/NOTICES` & `flet-0.6.0.dev1310/src/flet/web/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/assets/fonts/MaterialIcons-Regular.otf` & `flet-0.6.0.dev1310/src/flet/web/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/favicon.png` & `flet-0.6.0.dev1310/src/flet/web/favicon.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/flutter.js` & `flet-0.6.0.dev1310/src/flet/web/flutter.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/flutter_service_worker.js` & `flet-0.6.0.dev1310/src/flet/web/flutter_service_worker.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -10,30 +10,30 @@
     "assets/packages/window_manager/images/ic_chrome_close.png": "75f4b8ab3608a05461a31fc18d6b47c2",
     "assets/packages/window_manager/images/ic_chrome_unmaximize.png": "4a90c1909cb74e8f0d35794e2f61d8bf",
     "assets/FontManifest.json": "7b2a36307916a9721811788013e65289",
     "assets/fonts/MaterialIcons-Regular.otf": "e7069dfd19b331be16bed984668fe080",
     "favicon.png": "302ac04c14db027d016d1fe74c6a80a0",
     "manifest.json": "7909dae66a9203092dc86b5a6162e79c",
     "flutter.js": "a85fcf6324d3c4d3ae3be1ae4931e9c5",
-    "main.dart.js": "b969d8b0ae8e04c82fad058f06e4443c",
+    "main.dart.js": "bfb2bbc79c4bbed42642a9284ba312ba",
     "version.json": "3fea9d9c7b4ca6955aa03e762e0d2e13",
     "icons/apple-touch-icon-192.png": "8cf0d5162941f467a77f023c414a1812",
     "icons/icon-maskable-512.png": "aa798e6d780ff109da17c3a98d5f2619",
     "icons/loading-animation.png": "41a96047dbd2463a50c46ad3bf6ff158",
     "icons/icon-192.png": "81c4311263d0cad60c1f0496b4fa7c8f",
     "icons/icon-maskable-192.png": "c1c2210feeb444cf800a5ce0d06eff16",
     "icons/icon-512.png": "06b219f171b5a1af6dd8299ea1e116f2",
     "python.js": "9eee2c1773af78bc45ee89ca2ac5724f",
     "canvaskit/canvaskit.wasm": "3de12d898ec208a5f31362cc00f09b9e",
     "canvaskit/canvaskit.js": "97937cb4c2c2073c968525a3e08c86a3",
     "canvaskit/profiling/canvaskit.wasm": "371bc4e204443b0d5e774d64a046eb99",
     "canvaskit/profiling/canvaskit.js": "c21852696bc1cc82e8894d851c01921a",
     "python-worker.js": "b961f261b9ad85e06369e83fd2e33bb7",
-    "index.html": "43d859f416d37fa175677f7c3ac3d417",
-    "/": "43d859f416d37fa175677f7c3ac3d417"
+    "index.html": "f02902d82cf20e6436f75b1673574349",
+    "/": "f02902d82cf20e6436f75b1673574349"
 };
 
 // The application shell files that are downloaded before a service worker can
 // start.
 const CORE = [
     "main.dart.js",
     "index.html",
```

### Comparing `flet-0.6.0.dev1309/src/flet/web/icons/apple-touch-icon-192.png` & `flet-0.6.0.dev1310/src/flet/web/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/icons/icon-192.png` & `flet-0.6.0.dev1310/src/flet/web/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/icons/icon-512.png` & `flet-0.6.0.dev1310/src/flet/web/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/icons/icon-maskable-192.png` & `flet-0.6.0.dev1310/src/flet/web/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/icons/icon-maskable-512.png` & `flet-0.6.0.dev1310/src/flet/web/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/icons/loading-animation.png` & `flet-0.6.0.dev1310/src/flet/web/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/index.html` & `flet-0.6.0.dev1310/src/flet/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
   <!-- flutterWebRenderer -->
 
   <!-- pyodideCode -->
 
   <script>
     // The value below is injected by flutter build, do not touch.
-    var serviceWorkerVersion = '4268081007';
+    var serviceWorkerVersion = '3717999858';
   </script>
   <!-- This script adds the flutter initialization JS code -->
   <script src="flutter.js" defer></script>
 </head>
 
 <body>
   <div id="loading">
```

### Comparing `flet-0.6.0.dev1309/src/flet/web/main.dart.js` & `flet-0.6.0.dev1310/src/flet/web/main.dart.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -97917,24 +97917,27 @@
         $1(a) {
             return a.a.c === "c"
         },
         $S: 127
     }
     A.aJe.prototype = {
         $1(a) {
-            var s, r, q, p = a.b,
-                o = new A.V(p, new A.aJ8(), A.G(p).h("V<1>"))
-            p = a.a
-            s = p.H("numeric", !1)
+            var s, r, q, p, o, n = a.b,
+                m = new A.V(n, new A.aJ8(), A.G(n).h("V<1>"))
+            n = a.a
+            s = n.H("numeric", !1)
             s.toString
-            r = p.c1("tooltip")
-            q = p.H("onSort", !1)
+            r = n.c1("tooltip")
+            q = n.H("onSort", !1)
             q.toString
             q = q ? new A.aJ9(this.a, a) : null
-            return new A.xZ(A.bj(p, o.gJ(o).a, this.b), r, s, q)
+            p = m.gJ(m).a
+            o = n.H("disabled", !1)
+            o.toString
+            return new A.xZ(A.bj(n, p, o || this.b), r, s, q)
         },
         $S: 681
     }
     A.aJ8.prototype = {
         $1(a) {
             return a.d === "l"
         },
@@ -97982,36 +97985,40 @@
         $0() {
             this.a.aQ("", "long_press", this.b.a.a)
         },
         $S: 0
     }
     A.aJ7.prototype = {
         $1(a) {
-            var s, r, q, p, o, n, m = this,
-                l = null,
-                k = A.bj(m.a.a, B.b.gJ(a.e), m.b),
-                j = a.H("placeholder", !1)
+            var s, r, q, p, o, n = this,
+                m = null,
+                l = n.a.a,
+                k = B.b.gJ(a.e),
+                j = l.H("disabled", !1)
             j.toString
+            l = A.bj(l, k, j || n.b)
+            k = a.H("placeholder", !1)
+            k.toString
             s = a.H("showEditIcon", !1)
             s.toString
-            r = a.H("onDoubleTap", !1)
+            j = a.H("onDoubleTap", !1)
+            j.toString
+            j = j ? new A.aJ0(n.c, a) : m
+            r = a.H("onLongPress", !1)
             r.toString
-            r = r ? new A.aJ0(m.c, a) : l
-            q = a.H("onLongPress", !1)
+            r = r ? new A.aJ1(n.c, a) : m
+            q = a.H("onTap", !1)
             q.toString
-            q = q ? new A.aJ1(m.c, a) : l
-            p = a.H("onTap", !1)
+            q = q ? new A.aJ2(n.c, a) : m
+            p = a.H("onTapCancel", !1)
             p.toString
-            p = p ? new A.aJ2(m.c, a) : l
-            o = a.H("onTapCancel", !1)
+            p = p ? new A.aJ3(n.c, a) : m
+            o = a.H("onTapDown", !1)
             o.toString
-            o = o ? new A.aJ3(m.c, a) : l
-            n = a.H("onTapDown", !1)
-            n.toString
-            return new A.xY(k, j, s, p, r, q, n ? new A.aJ4(m.c, a) : l, o)
+            return new A.xY(l, k, s, q, j, r, o ? new A.aJ4(n.c, a) : m, p)
         },
         $S: 684
     }
     A.aJ0.prototype = {
         $0() {
             this.a.aQ("", "double_tap", this.b.a)
         },
```

### Comparing `flet-0.6.0.dev1309/src/flet/web/manifest.json` & `flet-0.6.0.dev1310/src/flet/web/manifest.json`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/python-worker.js` & `flet-0.6.0.dev1310/src/flet/web/python-worker.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/src/flet/web/python.js` & `flet-0.6.0.dev1310/src/flet/web/python.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1309/PKG-INFO` & `flet-0.6.0.dev1310/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet
-Version: 0.6.0.dev1309
+Version: 0.6.0.dev1310
 Summary: Flet for Python - easily build interactive multi-platform apps in Python
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.6.0.dev1309)
+Requires-Dist: flet-core (==0.6.0.dev1310)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: watchdog (>=2.2.1,<3.0.0)
 Requires-Dist: websocket-client (>=1.4.2,<2.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
```

