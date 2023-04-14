# Comparing `tmp/botik-telebot-0.0.1.tar.gz` & `tmp/botik-telebot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botik-telebot-0.0.1.tar", last modified: Thu Apr 13 20:36:05 2023, max compression
+gzip compressed data, was "botik-telebot-0.0.2.tar", last modified: Fri Apr 14 13:46:45 2023, max compression
```

## Comparing `botik-telebot-0.0.1.tar` & `botik-telebot-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.393705 botik-telebot-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-02-12 17:52:21.000000 botik-telebot-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      863 2023-04-13 20:36:05.392706 botik-telebot-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-04-13 20:31:14.000000 botik-telebot-0.0.1/README.md
--rw-rw-rw-   0        0        0      879 2023-04-13 20:28:08.000000 botik-telebot-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 20:36:05.393705 botik-telebot-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.368706 botik-telebot-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-02-12 13:31:38.000000 botik-telebot-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.369705 botik-telebot-0.0.1/src/botik_telebot/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.1/src/botik_telebot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.382705 botik-telebot-0.0.1/src/botik_telebot/api/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.1/src/botik_telebot/api/__init__.py
--rw-rw-rw-   0        0        0      292 2023-03-20 14:25:30.000000 botik-telebot-0.0.1/src/botik_telebot/api/api.py
--rw-rw-rw-   0        0        0       81 2023-02-12 16:12:42.000000 botik-telebot-0.0.1/src/botik_telebot/api/api_type.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.383705 botik-telebot-0.0.1/src/botik_telebot/api/attachment_handlers/
--rw-rw-rw-   0        0        0        0 2023-02-24 21:54:25.000000 botik-telebot-0.0.1/src/botik_telebot/api/attachment_handlers/__init__.py
--rw-rw-rw-   0        0        0      603 2023-03-01 02:08:02.000000 botik-telebot-0.0.1/src/botik_telebot/api/attachment_handlers/photo_attachment_handler.py
--rw-rw-rw-   0        0        0      769 2023-02-24 23:19:46.000000 botik-telebot-0.0.1/src/botik_telebot/api/send_message.py
--rw-rw-rw-   0        0        0      934 2023-03-13 00:45:51.000000 botik-telebot-0.0.1/src/botik_telebot/app.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.384706 botik-telebot-0.0.1/src/botik_telebot/input/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.1/src/botik_telebot/input/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.386705 botik-telebot-0.0.1/src/botik_telebot/input/keyboard/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.1/src/botik_telebot/input/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.388705 botik-telebot-0.0.1/src/botik_telebot/input/keyboard/button/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.1/src/botik_telebot/input/keyboard/button/__init__.py
--rw-rw-rw-   0        0        0      928 2023-02-12 16:14:58.000000 botik-telebot-0.0.1/src/botik_telebot/input/keyboard/button/button.py
--rw-rw-rw-   0        0        0      206 2023-02-12 16:14:58.000000 botik-telebot-0.0.1/src/botik_telebot/input/keyboard/button/button_factory.py
--rw-rw-rw-   0        0        0      594 2023-02-12 16:14:58.000000 botik-telebot-0.0.1/src/botik_telebot/input/keyboard/keyboard_markup.py
--rw-rw-rw-   0        0        0      310 2023-02-12 16:14:58.000000 botik-telebot-0.0.1/src/botik_telebot/input/keyboard/markup_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.390706 botik-telebot-0.0.1/src/botik_telebot/input/message_handlers/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.1/src/botik_telebot/input/message_handlers/__init__.py
--rw-rw-rw-   0        0        0     2006 2023-03-01 02:08:02.000000 botik-telebot-0.0.1/src/botik_telebot/input/message_handlers/raw_message_handlers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.391706 botik-telebot-0.0.1/src/botik_telebot/page/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.1/src/botik_telebot/page/__init__.py
--rw-rw-rw-   0        0        0      479 2023-02-12 16:14:58.000000 botik-telebot-0.0.1/src/botik_telebot/page/page_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:36:05.379706 botik-telebot-0.0.1/src/botik_telebot.egg-info/
--rw-rw-rw-   0        0        0      863 2023-04-13 20:36:05.000000 botik-telebot-0.0.1/src/botik_telebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2023-04-13 20:36:05.000000 botik-telebot-0.0.1/src/botik_telebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:36:05.000000 botik-telebot-0.0.1/src/botik_telebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-13 20:36:05.000000 botik-telebot-0.0.1/src/botik_telebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-13 20:36:05.000000 botik-telebot-0.0.1/src/botik_telebot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.500778 botik-telebot-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 17:52:21.000000 botik-telebot-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      863 2023-04-14 13:46:45.499781 botik-telebot-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-04-13 20:31:14.000000 botik-telebot-0.0.2/README.md
+-rw-rw-rw-   0        0        0      895 2023-04-14 13:45:30.000000 botik-telebot-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:46:45.500778 botik-telebot-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.359780 botik-telebot-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-02-12 13:31:38.000000 botik-telebot-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.369778 botik-telebot-0.0.2/src/botik_telebot/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.2/src/botik_telebot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.424777 botik-telebot-0.0.2/src/botik_telebot/api/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.2/src/botik_telebot/api/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-03-20 14:25:30.000000 botik-telebot-0.0.2/src/botik_telebot/api/api.py
+-rw-rw-rw-   0        0        0       81 2023-02-12 16:12:42.000000 botik-telebot-0.0.2/src/botik_telebot/api/api_type.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.434778 botik-telebot-0.0.2/src/botik_telebot/api/attachment_handlers/
+-rw-rw-rw-   0        0        0        0 2023-02-24 21:54:25.000000 botik-telebot-0.0.2/src/botik_telebot/api/attachment_handlers/__init__.py
+-rw-rw-rw-   0        0        0      603 2023-03-01 02:08:02.000000 botik-telebot-0.0.2/src/botik_telebot/api/attachment_handlers/photo_attachment_handler.py
+-rw-rw-rw-   0        0        0      769 2023-02-24 23:19:46.000000 botik-telebot-0.0.2/src/botik_telebot/api/send_message.py
+-rw-rw-rw-   0        0        0      894 2023-04-13 21:09:25.000000 botik-telebot-0.0.2/src/botik_telebot/app.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.436782 botik-telebot-0.0.2/src/botik_telebot/input/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.2/src/botik_telebot/input/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.455777 botik-telebot-0.0.2/src/botik_telebot/input/keyboard/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.2/src/botik_telebot/input/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.475813 botik-telebot-0.0.2/src/botik_telebot/input/keyboard/button/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.2/src/botik_telebot/input/keyboard/button/__init__.py
+-rw-rw-rw-   0        0        0      928 2023-02-12 16:14:58.000000 botik-telebot-0.0.2/src/botik_telebot/input/keyboard/button/button.py
+-rw-rw-rw-   0        0        0      206 2023-02-12 16:14:58.000000 botik-telebot-0.0.2/src/botik_telebot/input/keyboard/button/button_factory.py
+-rw-rw-rw-   0        0        0      594 2023-02-12 16:14:58.000000 botik-telebot-0.0.2/src/botik_telebot/input/keyboard/keyboard_markup.py
+-rw-rw-rw-   0        0        0      310 2023-02-12 16:14:58.000000 botik-telebot-0.0.2/src/botik_telebot/input/keyboard/markup_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.487814 botik-telebot-0.0.2/src/botik_telebot/input/message_handlers/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.2/src/botik_telebot/input/message_handlers/__init__.py
+-rw-rw-rw-   0        0        0     2006 2023-03-01 02:08:02.000000 botik-telebot-0.0.2/src/botik_telebot/input/message_handlers/raw_message_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.497777 botik-telebot-0.0.2/src/botik_telebot/page/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:59:29.000000 botik-telebot-0.0.2/src/botik_telebot/page/__init__.py
+-rw-rw-rw-   0        0        0      479 2023-02-12 16:14:58.000000 botik-telebot-0.0.2/src/botik_telebot/page/page_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:46:45.397776 botik-telebot-0.0.2/src/botik_telebot.egg-info/
+-rw-rw-rw-   0        0        0      863 2023-04-14 13:46:45.000000 botik-telebot-0.0.2/src/botik_telebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2023-04-14 13:46:45.000000 botik-telebot-0.0.2/src/botik_telebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:46:45.000000 botik-telebot-0.0.2/src/botik_telebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-14 13:46:45.000000 botik-telebot-0.0.2/src/botik_telebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-14 13:46:45.000000 botik-telebot-0.0.2/src/botik_telebot.egg-info/top_level.txt
```

### Comparing `botik-telebot-0.0.1/LICENSE` & `botik-telebot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `botik-telebot-0.0.1/PKG-INFO` & `botik-telebot-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botik-telebot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extension for Botik to support pyTelegramBot
 Author-email: dasstyx <dasstyx@gmail.com>
 Project-URL: Documentation, https://botik.readthedocs.io
 Project-URL: Homepage, https://github.com/dasstyx/botik-telebot
 Project-URL: Bug Tracker, https://github.com/dasstyx/botik-telebot/issues
 Keywords: api,framework,bot,tg,messenger,async,botik
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botik-telebot-0.0.1/pyproject.toml` & `botik-telebot-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "botik-telebot"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "dasstyx", email = "dasstyx@gmail.com" },
 ]
 description = "Extension for Botik to support pyTelegramBot"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -20,14 +20,15 @@
     "messenger",
     "async",
     "botik",
 ]
 
 dependencies = [
     "botik",
+    "aiohttp",
     "pyTelegramBotAPI==4.7.0"
 ]
 
 [project.urls]
 "Documentation" = "https://botik.readthedocs.io"
 "Homepage" = "https://github.com/dasstyx/botik-telebot"
 "Bug Tracker" = "https://github.com/dasstyx/botik-telebot/issues"
```

### Comparing `botik-telebot-0.0.1/src/botik_telebot/api/attachment_handlers/photo_attachment_handler.py` & `botik-telebot-0.0.2/src/botik_telebot/api/attachment_handlers/photo_attachment_handler.py`

 * *Files identical despite different names*

### Comparing `botik-telebot-0.0.1/src/botik_telebot/api/send_message.py` & `botik-telebot-0.0.2/src/botik_telebot/api/send_message.py`

 * *Files identical despite different names*

### Comparing `botik-telebot-0.0.1/src/botik_telebot/app.py` & `botik-telebot-0.0.2/src/botik_telebot/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,15 @@
         self.initialize()
         loop = asyncio.get_event_loop()
         loop.create_task(self.bot.polling())
         loop.run_forever()
 
     def __init__(self, bot, start_callback=None):
         super().__init__(bot)
-        RawMessageHandlers(bot, start_callback,
-                           self.users, self.user_input)
+        RawMessageHandlers(bot, start_callback, self.user_input)
 
     def initialize(self):
         api = TgApi(self.bot)
         set_api(api)
 
         self._page_fac: PageFactory = TgPageFactory()
         navigator.initialize(self._page_fac, self.pages_data)
```

### Comparing `botik-telebot-0.0.1/src/botik_telebot/input/keyboard/button/button.py` & `botik-telebot-0.0.2/src/botik_telebot/input/keyboard/button/button.py`

 * *Files identical despite different names*

### Comparing `botik-telebot-0.0.1/src/botik_telebot/input/keyboard/keyboard_markup.py` & `botik-telebot-0.0.2/src/botik_telebot/input/keyboard/keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `botik-telebot-0.0.1/src/botik_telebot/input/message_handlers/raw_message_handlers.py` & `botik-telebot-0.0.2/src/botik_telebot/input/message_handlers/raw_message_handlers.py`

 * *Files identical despite different names*

### Comparing `botik-telebot-0.0.1/src/botik_telebot.egg-info/PKG-INFO` & `botik-telebot-0.0.2/src/botik_telebot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botik-telebot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extension for Botik to support pyTelegramBot
 Author-email: dasstyx <dasstyx@gmail.com>
 Project-URL: Documentation, https://botik.readthedocs.io
 Project-URL: Homepage, https://github.com/dasstyx/botik-telebot
 Project-URL: Bug Tracker, https://github.com/dasstyx/botik-telebot/issues
 Keywords: api,framework,bot,tg,messenger,async,botik
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botik-telebot-0.0.1/src/botik_telebot.egg-info/SOURCES.txt` & `botik-telebot-0.0.2/src/botik_telebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

