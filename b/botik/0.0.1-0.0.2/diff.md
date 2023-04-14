# Comparing `tmp/botik-0.0.1.tar.gz` & `tmp/botik-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botik-0.0.1.tar", last modified: Thu Apr 13 20:35:28 2023, max compression
+gzip compressed data, was "botik-0.0.2.tar", last modified: Fri Apr 14 13:46:45 2023, max compression
```

## Comparing `botik-0.0.1.tar` & `botik-0.0.2.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:28.147273 botik-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-02-12 17:52:21.000000 botik-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3965 2023-04-13 20:35:28.146274 botik-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-04-12 13:33:01.000000 botik-0.0.1/README.md
--rw-rw-rw-   0        0        0      750 2023-04-13 20:28:08.000000 botik-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 20:35:28.147273 botik-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:27.940274 botik-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-02-12 13:30:44.000000 botik-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:27.946273 botik-0.0.1/src/botik/
--rw-rw-rw-   0        0        0        0 2023-02-16 14:55:57.000000 botik-0.0.1/src/botik/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:27.978310 botik-0.0.1/src/botik/api/
--rw-rw-rw-   0        0        0      189 2023-02-24 20:48:51.000000 botik-0.0.1/src/botik/api/__init__.py
--rw-rw-rw-   0        0        0      214 2023-04-03 13:25:58.000000 botik-0.0.1/src/botik/api/api.py
--rw-rw-rw-   0        0        0      119 2023-02-16 14:55:57.000000 botik-0.0.1/src/botik/api/api_type.py
--rw-rw-rw-   0        0        0      314 2023-02-24 23:04:33.000000 botik-0.0.1/src/botik/api/send_message.py
--rw-rw-rw-   0        0        0      784 2023-04-03 13:25:58.000000 botik-0.0.1/src/botik/app.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:27.983310 botik-0.0.1/src/botik/input/
--rw-rw-rw-   0        0        0        0 2022-11-04 03:04:56.000000 botik-0.0.1/src/botik/input/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:27.996273 botik-0.0.1/src/botik/input/keyboard/
--rw-rw-rw-   0        0        0        0 2022-11-04 03:04:56.000000 botik-0.0.1/src/botik/input/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:28.023274 botik-0.0.1/src/botik/input/keyboard/button/
--rw-rw-rw-   0        0        0        0 2023-02-16 14:55:57.000000 botik-0.0.1/src/botik/input/keyboard/button/__init__.py
--rw-rw-rw-   0        0        0      835 2023-02-24 20:48:51.000000 botik-0.0.1/src/botik/input/keyboard/button/button.py
--rw-rw-rw-   0        0        0     1192 2023-02-24 20:48:51.000000 botik-0.0.1/src/botik/input/keyboard/button/button_data.py
--rw-rw-rw-   0        0        0      466 2023-02-24 20:48:51.000000 botik-0.0.1/src/botik/input/keyboard/button/button_factory.py
--rw-rw-rw-   0        0        0      117 2023-02-16 14:55:57.000000 botik-0.0.1/src/botik/input/keyboard/button/button_function.py
--rw-rw-rw-   0        0        0     1347 2023-02-24 20:48:51.000000 botik-0.0.1/src/botik/input/keyboard/keyboard_markup.py
--rw-rw-rw-   0        0        0      366 2023-02-16 14:55:57.000000 botik-0.0.1/src/botik/input/keyboard/markup_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:28.031273 botik-0.0.1/src/botik/input/message_handlers/
--rw-rw-rw-   0        0        0        0 2022-11-04 03:04:56.000000 botik-0.0.1/src/botik/input/message_handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:28.059274 botik-0.0.1/src/botik/input/message_handlers/events/
--rw-rw-rw-   0        0        0      116 2023-02-18 01:28:04.000000 botik-0.0.1/src/botik/input/message_handlers/events/__init__.py
--rw-rw-rw-   0        0        0      728 2023-02-18 01:26:04.000000 botik-0.0.1/src/botik/input/message_handlers/events/bot_event.py
--rw-rw-rw-   0        0        0      482 2023-02-25 15:02:41.000000 botik-0.0.1/src/botik/input/message_handlers/events/bot_events.py
--rw-rw-rw-   0        0        0      118 2023-02-18 01:26:04.000000 botik-0.0.1/src/botik/input/message_handlers/events/contact_share_event.py
--rw-rw-rw-   0        0        0      114 2023-02-18 01:26:04.000000 botik-0.0.1/src/botik/input/message_handlers/events/geo_share_event.py
--rw-rw-rw-   0        0        0      119 2023-02-25 00:36:05.000000 botik-0.0.1/src/botik/input/message_handlers/events/got_attachment_event.py
--rw-rw-rw-   0        0        0     1419 2023-04-03 13:25:58.000000 botik-0.0.1/src/botik/input/message_handlers/raw_message_handlers.py
--rw-rw-rw-   0        0        0      360 2023-04-03 13:25:58.000000 botik-0.0.1/src/botik/input/user_input.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:28.076274 botik-0.0.1/src/botik/navigation/
--rw-rw-rw-   0        0        0      105 2023-02-18 01:26:04.000000 botik-0.0.1/src/botik/navigation/__init__.py
--rw-rw-rw-   0        0        0     2558 2023-03-12 21:15:00.000000 botik-0.0.1/src/botik/navigation/navigation.py
--rw-rw-rw-   0        0        0      685 2023-02-20 17:41:14.000000 botik-0.0.1/src/botik/navigation/routing.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:28.100276 botik-0.0.1/src/botik/page/
--rw-rw-rw-   0        0        0        0 2023-02-16 14:55:57.000000 botik-0.0.1/src/botik/page/__init__.py
--rw-rw-rw-   0        0        0      546 2023-03-07 14:51:37.000000 botik-0.0.1/src/botik/page/input_page.py
--rw-rw-rw-   0        0        0     2753 2023-03-20 12:02:28.000000 botik-0.0.1/src/botik/page/page.py
--rw-rw-rw-   0        0        0     1389 2023-03-12 21:15:00.000000 botik-0.0.1/src/botik/page/page_data.py
--rw-rw-rw-   0        0        0      353 2023-03-12 21:15:00.000000 botik-0.0.1/src/botik/page/page_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:28.122274 botik-0.0.1/src/botik/user/
--rw-rw-rw-   0        0        0       87 2023-04-03 13:25:58.000000 botik-0.0.1/src/botik/user/__init__.py
--rw-rw-rw-   0        0        0      285 2023-02-27 16:52:46.000000 botik-0.0.1/src/botik/user/storage.py
--rw-rw-rw-   0        0        0      325 2023-03-12 21:15:00.000000 botik-0.0.1/src/botik/user/user.py
--rw-rw-rw-   0        0        0      497 2023-02-18 01:26:04.000000 botik-0.0.1/src/botik/user/user_base.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:27.957274 botik-0.0.1/src/botik.egg-info/
--rw-rw-rw-   0        0        0     3965 2023-04-13 20:35:27.000000 botik-0.0.1/src/botik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1631 2023-04-13 20:35:27.000000 botik-0.0.1/src/botik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:35:27.000000 botik-0.0.1/src/botik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 20:35:27.000000 botik-0.0.1/src/botik.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:28.145273 botik-0.0.1/tests/
--rw-rw-rw-   0        0        0     1382 2023-02-18 01:26:04.000000 botik-0.0.1/tests/test_bot_event.py
--rw-rw-rw-   0        0        0     1126 2023-02-18 01:26:04.000000 botik-0.0.1/tests/test_button_templates.py
--rw-rw-rw-   0        0        0      686 2023-02-18 01:26:04.000000 botik-0.0.1/tests/test_navigation.py
--rw-rw-rw-   0        0        0      882 2023-02-18 01:26:04.000000 botik-0.0.1/tests/test_user_base.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.712778 botik-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 17:52:21.000000 botik-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3965 2023-04-14 13:46:45.711778 botik-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-04-12 13:33:01.000000 botik-0.0.2/README.md
+-rw-rw-rw-   0        0        0      787 2023-04-14 13:45:30.000000 botik-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:46:45.712778 botik-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.359780 botik-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-02-12 13:30:44.000000 botik-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.369778 botik-0.0.2/src/botik/
+-rw-rw-rw-   0        0        0        0 2023-02-16 14:55:57.000000 botik-0.0.2/src/botik/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.433813 botik-0.0.2/src/botik/api/
+-rw-rw-rw-   0        0        0      189 2023-02-24 20:48:51.000000 botik-0.0.2/src/botik/api/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-04-03 13:25:58.000000 botik-0.0.2/src/botik/api/api.py
+-rw-rw-rw-   0        0        0      119 2023-02-16 14:55:57.000000 botik-0.0.2/src/botik/api/api_type.py
+-rw-rw-rw-   0        0        0      314 2023-02-24 23:04:33.000000 botik-0.0.2/src/botik/api/send_message.py
+-rw-rw-rw-   0        0        0      784 2023-04-03 13:25:58.000000 botik-0.0.2/src/botik/app.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.438780 botik-0.0.2/src/botik/input/
+-rw-rw-rw-   0        0        0        0 2022-11-04 03:04:56.000000 botik-0.0.2/src/botik/input/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.458814 botik-0.0.2/src/botik/input/keyboard/
+-rw-rw-rw-   0        0        0        0 2022-11-04 03:04:56.000000 botik-0.0.2/src/botik/input/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.499781 botik-0.0.2/src/botik/input/keyboard/button/
+-rw-rw-rw-   0        0        0        0 2023-02-16 14:55:57.000000 botik-0.0.2/src/botik/input/keyboard/button/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-02-24 20:48:51.000000 botik-0.0.2/src/botik/input/keyboard/button/button.py
+-rw-rw-rw-   0        0        0     1192 2023-02-24 20:48:51.000000 botik-0.0.2/src/botik/input/keyboard/button/button_data.py
+-rw-rw-rw-   0        0        0      466 2023-02-24 20:48:51.000000 botik-0.0.2/src/botik/input/keyboard/button/button_factory.py
+-rw-rw-rw-   0        0        0      117 2023-02-16 14:55:57.000000 botik-0.0.2/src/botik/input/keyboard/button/button_function.py
+-rw-rw-rw-   0        0        0     1347 2023-02-24 20:48:51.000000 botik-0.0.2/src/botik/input/keyboard/keyboard_markup.py
+-rw-rw-rw-   0        0        0      366 2023-02-16 14:55:57.000000 botik-0.0.2/src/botik/input/keyboard/markup_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.512780 botik-0.0.2/src/botik/input/message_handlers/
+-rw-rw-rw-   0        0        0        0 2022-11-04 03:04:56.000000 botik-0.0.2/src/botik/input/message_handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.568784 botik-0.0.2/src/botik/input/message_handlers/events/
+-rw-rw-rw-   0        0        0      116 2023-02-18 01:28:04.000000 botik-0.0.2/src/botik/input/message_handlers/events/__init__.py
+-rw-rw-rw-   0        0        0      728 2023-02-18 01:26:04.000000 botik-0.0.2/src/botik/input/message_handlers/events/bot_event.py
+-rw-rw-rw-   0        0        0      482 2023-02-25 15:02:41.000000 botik-0.0.2/src/botik/input/message_handlers/events/bot_events.py
+-rw-rw-rw-   0        0        0      118 2023-02-18 01:26:04.000000 botik-0.0.2/src/botik/input/message_handlers/events/contact_share_event.py
+-rw-rw-rw-   0        0        0      114 2023-02-18 01:26:04.000000 botik-0.0.2/src/botik/input/message_handlers/events/geo_share_event.py
+-rw-rw-rw-   0        0        0      119 2023-02-25 00:36:05.000000 botik-0.0.2/src/botik/input/message_handlers/events/got_attachment_event.py
+-rw-rw-rw-   0        0        0     1419 2023-04-03 13:25:58.000000 botik-0.0.2/src/botik/input/message_handlers/raw_message_handlers.py
+-rw-rw-rw-   0        0        0      360 2023-04-03 13:25:58.000000 botik-0.0.2/src/botik/input/user_input.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.598814 botik-0.0.2/src/botik/navigation/
+-rw-rw-rw-   0        0        0      105 2023-02-18 01:26:04.000000 botik-0.0.2/src/botik/navigation/__init__.py
+-rw-rw-rw-   0        0        0     2558 2023-03-12 21:15:00.000000 botik-0.0.2/src/botik/navigation/navigation.py
+-rw-rw-rw-   0        0        0      685 2023-02-20 17:41:14.000000 botik-0.0.2/src/botik/navigation/routing.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.638783 botik-0.0.2/src/botik/page/
+-rw-rw-rw-   0        0        0        0 2023-02-16 14:55:57.000000 botik-0.0.2/src/botik/page/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-03-07 14:51:37.000000 botik-0.0.2/src/botik/page/input_page.py
+-rw-rw-rw-   0        0        0     2753 2023-03-20 12:02:28.000000 botik-0.0.2/src/botik/page/page.py
+-rw-rw-rw-   0        0        0     1389 2023-03-12 21:15:00.000000 botik-0.0.2/src/botik/page/page_data.py
+-rw-rw-rw-   0        0        0      353 2023-03-12 21:15:00.000000 botik-0.0.2/src/botik/page/page_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.673778 botik-0.0.2/src/botik/user/
+-rw-rw-rw-   0        0        0       87 2023-04-03 13:25:58.000000 botik-0.0.2/src/botik/user/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-02-27 16:52:46.000000 botik-0.0.2/src/botik/user/storage.py
+-rw-rw-rw-   0        0        0      325 2023-03-12 21:15:00.000000 botik-0.0.2/src/botik/user/user.py
+-rw-rw-rw-   0        0        0      497 2023-02-18 01:26:04.000000 botik-0.0.2/src/botik/user/user_base.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.397776 botik-0.0.2/src/botik.egg-info/
+-rw-rw-rw-   0        0        0     3965 2023-04-14 13:46:45.000000 botik-0.0.2/src/botik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2023-04-14 13:46:45.000000 botik-0.0.2/src/botik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:46:45.000000 botik-0.0.2/src/botik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 13:46:45.000000 botik-0.0.2/src/botik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 13:46:45.000000 botik-0.0.2/src/botik.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.709777 botik-0.0.2/tests/
+-rw-rw-rw-   0        0        0     1382 2023-02-18 01:26:04.000000 botik-0.0.2/tests/test_bot_event.py
+-rw-rw-rw-   0        0        0     1126 2023-02-18 01:26:04.000000 botik-0.0.2/tests/test_button_templates.py
+-rw-rw-rw-   0        0        0      686 2023-02-18 01:26:04.000000 botik-0.0.2/tests/test_navigation.py
+-rw-rw-rw-   0        0        0      882 2023-02-18 01:26:04.000000 botik-0.0.2/tests/test_user_base.py
```

### Comparing `botik-0.0.1/LICENSE` & `botik-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/PKG-INFO` & `botik-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botik
-Version: 0.0.1
+Version: 0.0.2
 Summary: Botik core package
 Author-email: dasstyx <dasstyx@gmail.com>
 Project-URL: Documentation, https://botik.readthedocs.io
 Project-URL: Homepage, https://github.com/dasstyx/botik
 Project-URL: Bug Tracker, https://github.com/dasstyx/botik/issues
 Keywords: api,framework,bot,messenger,async,botik
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botik-0.0.1/README.md` & `botik-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/pyproject.toml` & `botik-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "botik"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "dasstyx", email = "dasstyx@gmail.com" },
 ]
 description = "Botik core package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,14 +17,18 @@
     "framework",
     "bot",
     "messenger",
     "async",
     "botik",
 ]
 
+dependencies = [
+    "pillow"
+]
+
 [project.urls]
 "Documentation" = "https://botik.readthedocs.io"
 "Homepage" = "https://github.com/dasstyx/botik"
 "Bug Tracker" = "https://github.com/dasstyx/botik/issues"
 
 [build-system]
 requires = [
```

### Comparing `botik-0.0.1/src/botik/app.py` & `botik-0.0.2/src/botik/app.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/input/keyboard/button/button.py` & `botik-0.0.2/src/botik/input/keyboard/button/button.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/input/keyboard/button/button_data.py` & `botik-0.0.2/src/botik/input/keyboard/button/button_data.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/input/keyboard/keyboard_markup.py` & `botik-0.0.2/src/botik/input/keyboard/keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/input/message_handlers/events/bot_event.py` & `botik-0.0.2/src/botik/input/message_handlers/events/bot_event.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/input/message_handlers/raw_message_handlers.py` & `botik-0.0.2/src/botik/input/message_handlers/raw_message_handlers.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/navigation/navigation.py` & `botik-0.0.2/src/botik/navigation/navigation.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/navigation/routing.py` & `botik-0.0.2/src/botik/navigation/routing.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/page/input_page.py` & `botik-0.0.2/src/botik/page/input_page.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/page/page.py` & `botik-0.0.2/src/botik/page/page.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik/page/page_data.py` & `botik-0.0.2/src/botik/page/page_data.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/src/botik.egg-info/PKG-INFO` & `botik-0.0.2/src/botik.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botik
-Version: 0.0.1
+Version: 0.0.2
 Summary: Botik core package
 Author-email: dasstyx <dasstyx@gmail.com>
 Project-URL: Documentation, https://botik.readthedocs.io
 Project-URL: Homepage, https://github.com/dasstyx/botik
 Project-URL: Bug Tracker, https://github.com/dasstyx/botik/issues
 Keywords: api,framework,bot,messenger,async,botik
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botik-0.0.1/src/botik.egg-info/SOURCES.txt` & `botik-0.0.2/src/botik.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 src/__init__.py
 src/botik/__init__.py
 src/botik/app.py
 src/botik.egg-info/PKG-INFO
 src/botik.egg-info/SOURCES.txt
 src/botik.egg-info/dependency_links.txt
+src/botik.egg-info/requires.txt
 src/botik.egg-info/top_level.txt
 src/botik/api/__init__.py
 src/botik/api/api.py
 src/botik/api/api_type.py
 src/botik/api/send_message.py
 src/botik/input/__init__.py
 src/botik/input/user_input.py
```

### Comparing `botik-0.0.1/tests/test_bot_event.py` & `botik-0.0.2/tests/test_bot_event.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/tests/test_button_templates.py` & `botik-0.0.2/tests/test_button_templates.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/tests/test_navigation.py` & `botik-0.0.2/tests/test_navigation.py`

 * *Files identical despite different names*

### Comparing `botik-0.0.1/tests/test_user_base.py` & `botik-0.0.2/tests/test_user_base.py`

 * *Files identical despite different names*

