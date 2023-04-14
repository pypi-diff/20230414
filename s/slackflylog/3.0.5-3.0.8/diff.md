# Comparing `tmp/slackflylog-3.0.5.tar.gz` & `tmp/slackflylog-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-3.0.5.tar", last modified: Thu Apr 13 09:27:17 2023, max compression
+gzip compressed data, was "dist/slackflylog-3.0.8.tar", last modified: Fri Apr 14 09:42:41 2023, max compression
```

## Comparing `slackflylog-3.0.5.tar` & `slackflylog-3.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.766273 slackflylog-3.0.5/
--rw-r--r--   0 user_xh   (1000) users      (100)     1063 2023-04-13 09:26:46.000000 slackflylog-3.0.5/LICENSE
--rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-13 09:27:17.766273 slackflylog-3.0.5/PKG-INFO
--rw-r--r--   0 user_xh   (1000) users      (100)       13 2023-04-13 09:26:46.000000 slackflylog-3.0.5/README.md
--rw-r--r--   0 user_xh   (1000) users      (100)       38 2023-04-13 09:27:17.766273 slackflylog-3.0.5/setup.cfg
--rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-13 09:27:05.000000 slackflylog-3.0.5/setup.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.763273 slackflylog-3.0.5/slackflylog/
--rw-r--r--   0 user_xh   (1000) users      (100)      281 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/__init__.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.765273 slackflylog-3.0.5/slackflylog/agent/
--rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/__init__.py
--rw-r--r--   0 user_xh   (1000) users      (100)     3686 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/agent.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.765273 slackflylog-3.0.5/slackflylog/agent/backends/
--rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/backends/__init__.py
--rw-r--r--   0 user_xh   (1000) users      (100)     2114 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/backends/send_slack.py
--rw-r--r--   0 user_xh   (1000) users      (100)      123 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/log.py
--rw-r--r--   0 user_xh   (1000) users      (100)     1795 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/agent/utils.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.765273 slackflylog-3.0.5/slackflylog/api/
--rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/api/__init__.py
--rw-r--r--   0 user_xh   (1000) users      (100)     1174 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/api/client.py
--rw-r--r--   0 user_xh   (1000) users      (100)     1599 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/api/log_handler.py
--rw-r--r--   0 user_xh   (1000) users      (100)      182 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/constants.py
--rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-13 09:26:46.000000 slackflylog-3.0.5/slackflylog/setup.py
-drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-13 09:27:17.764273 slackflylog-3.0.5/slackflylog.egg-info/
--rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 user_xh   (1000) users      (100)      544 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 user_xh   (1000) users      (100)        1 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 user_xh   (1000) users      (100)       25 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/requires.txt
--rw-r--r--   0 user_xh   (1000) users      (100)       12 2023-04-13 09:27:17.000000 slackflylog-3.0.5/slackflylog.egg-info/top_level.txt
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-14 09:42:41.677322 slackflylog-3.0.8/
+-rw-r--r--   0 user_xh   (1000) users      (100)     1063 2023-04-13 09:26:46.000000 slackflylog-3.0.8/LICENSE
+-rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-14 09:42:41.677322 slackflylog-3.0.8/PKG-INFO
+-rw-r--r--   0 user_xh   (1000) users      (100)       13 2023-04-13 09:26:46.000000 slackflylog-3.0.8/README.md
+-rw-r--r--   0 user_xh   (1000) users      (100)       38 2023-04-14 09:42:41.677322 slackflylog-3.0.8/setup.cfg
+-rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-14 09:42:29.000000 slackflylog-3.0.8/setup.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-14 09:42:41.675322 slackflylog-3.0.8/slackflylog/
+-rw-r--r--   0 user_xh   (1000) users      (100)      281 2023-04-13 09:26:46.000000 slackflylog-3.0.8/slackflylog/__init__.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-14 09:42:41.676322 slackflylog-3.0.8/slackflylog/agent/
+-rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 09:26:46.000000 slackflylog-3.0.8/slackflylog/agent/__init__.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     3686 2023-04-13 09:26:46.000000 slackflylog-3.0.8/slackflylog/agent/agent.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-14 09:42:41.676322 slackflylog-3.0.8/slackflylog/agent/backends/
+-rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 09:26:46.000000 slackflylog-3.0.8/slackflylog/agent/backends/__init__.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     2189 2023-04-14 09:41:48.000000 slackflylog-3.0.8/slackflylog/agent/backends/send_slack.py
+-rw-r--r--   0 user_xh   (1000) users      (100)      123 2023-04-13 09:26:46.000000 slackflylog-3.0.8/slackflylog/agent/log.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     1083 2023-04-14 09:41:48.000000 slackflylog-3.0.8/slackflylog/agent/utils.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-14 09:42:41.676322 slackflylog-3.0.8/slackflylog/api/
+-rw-r--r--   0 user_xh   (1000) users      (100)       23 2023-04-13 09:26:46.000000 slackflylog-3.0.8/slackflylog/api/__init__.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     1174 2023-04-13 09:26:46.000000 slackflylog-3.0.8/slackflylog/api/client.py
+-rw-r--r--   0 user_xh   (1000) users      (100)     1599 2023-04-13 09:26:46.000000 slackflylog-3.0.8/slackflylog/api/log_handler.py
+-rw-r--r--   0 user_xh   (1000) users      (100)      182 2023-04-13 09:26:46.000000 slackflylog-3.0.8/slackflylog/constants.py
+-rw-r--r--   0 user_xh   (1000) users      (100)      639 2023-04-14 09:41:48.000000 slackflylog-3.0.8/slackflylog/setup.py
+drwxr-xr-x   0 user_xh   (1000) users      (100)        0 2023-04-14 09:42:41.675322 slackflylog-3.0.8/slackflylog.egg-info/
+-rw-r--r--   0 user_xh   (1000) users      (100)      229 2023-04-14 09:42:41.000000 slackflylog-3.0.8/slackflylog.egg-info/PKG-INFO
+-rw-r--r--   0 user_xh   (1000) users      (100)      544 2023-04-14 09:42:41.000000 slackflylog-3.0.8/slackflylog.egg-info/SOURCES.txt
+-rw-r--r--   0 user_xh   (1000) users      (100)        1 2023-04-14 09:42:41.000000 slackflylog-3.0.8/slackflylog.egg-info/dependency_links.txt
+-rw-r--r--   0 user_xh   (1000) users      (100)       25 2023-04-14 09:42:41.000000 slackflylog-3.0.8/slackflylog.egg-info/requires.txt
+-rw-r--r--   0 user_xh   (1000) users      (100)       12 2023-04-14 09:42:41.000000 slackflylog-3.0.8/slackflylog.egg-info/top_level.txt
```

### Comparing `slackflylog-3.0.5/LICENSE` & `slackflylog-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.5/setup.py` & `slackflylog-3.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.5"
+    __version__ = "1.0.8"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
-    __version__ = "3.0.5"
+    __version__ = "3.0.8"
 
 
 
 
 setup(
     name='slackflylog',
     version=__version__,
```

### Comparing `slackflylog-3.0.5/slackflylog/agent/agent.py` & `slackflylog-3.0.8/slackflylog/agent/agent.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.5/slackflylog/agent/backends/send_slack.py` & `slackflylog-3.0.8/slackflylog/agent/backends/send_slack.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,23 +62,27 @@
         if not send_msg and not title:
             return False
 
         msg = '\n\n'.join([title, send_msg])
         if '%0a' in msg:
             msg = msg.replace('%0a', '\n')
 
+        # 增加@功能
+        msg = '{msg}\n<!channel>'.format(msg=msg)
+
+
         if PY2:
             sc = SendClient(slack_token)
             # 发送消息
             sc.api_call(
                 "chat.postMessage",
                 channel=channel_id,
                 text=msg
             )
 
         else:
             # Python3 发送
             sc = SendClient(token=slack_token)
 
-            sc.chat_postMessage(channel=channel_id, text=text)
+            sc.chat_postMessage(channel=channel_id, text=msg)
 
         return True
```

### Comparing `slackflylog-3.0.5/slackflylog/api/client.py` & `slackflylog-3.0.8/slackflylog/api/client.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.5/slackflylog/api/log_handler.py` & `slackflylog-3.0.8/slackflylog/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `slackflylog-3.0.5/slackflylog/setup.py` & `slackflylog-3.0.8/slackflylog/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 # 基於flylog, slack-client處理
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['flylog','slackclient>=1.3.2']
-    __version__ = "1.0.5"
+    __version__ = "1.0.8"
 
 else:
     REQUIRE_PACK = ['flylog','slack_sdk>=3.19.5']
-    __version__ = "3.0.5"
+    __version__ = "3.0.8"
 
 
 
 
 setup(
     name='slackflylog',
     version=__version__,
```

### Comparing `slackflylog-3.0.5/slackflylog.egg-info/SOURCES.txt` & `slackflylog-3.0.8/slackflylog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

