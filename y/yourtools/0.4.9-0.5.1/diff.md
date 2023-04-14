# Comparing `tmp/yourtools-0.4.9.tar.gz` & `tmp/yourtools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yourtools-0.4.9.tar", last modified: Fri Apr 14 10:09:33 2023, max compression
+gzip compressed data, was "dist/yourtools-0.5.1.tar", last modified: Fri Apr 14 10:39:04 2023, max compression
```

## Comparing `yourtools-0.4.9.tar` & `yourtools-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:09:33.000000 yourtools-0.4.9/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:09:33.000000 yourtools-0.4.9/yourtools/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:09:33.000000 yourtools-0.4.9/yourtools/db/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.4.9/yourtools/db/__init__.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.4.9/yourtools/db/dbutils.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.4.9/yourtools/db/hive.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.4.9/yourtools/db/mysql.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.4.9/yourtools/Azkaban.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      723 2023-04-14 09:47:09.000000 yourtools-0.4.9/yourtools/Time.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     4629 2023-04-14 10:08:39.000000 yourtools-0.4.9/yourtools/WeChat.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      469 2023-04-13 08:48:52.000000 yourtools-0.4.9/yourtools/__init__.py
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:09:33.000000 yourtools-0.4.9/yourtools.egg-info/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 10:09:33.000000 yourtools-0.4.9/yourtools.egg-info/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-14 10:09:33.000000 yourtools-0.4.9/yourtools.egg-info/SOURCES.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-14 10:09:33.000000 yourtools-0.4.9/yourtools.egg-info/dependency_links.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-14 10:09:33.000000 yourtools-0.4.9/yourtools.egg-info/requires.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-14 10:09:33.000000 yourtools-0.4.9/yourtools.egg-info/top_level.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.4.9/README.md
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.4.9/requirements.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-07 10:28:09.000000 yourtools-0.4.9/setup.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 10:09:33.000000 yourtools-0.4.9/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-14 10:09:33.000000 yourtools-0.4.9/setup.cfg
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:39:04.000000 yourtools-0.5.1/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools/db/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.5.1/yourtools/db/__init__.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.5.1/yourtools/db/dbutils.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.5.1/yourtools/db/hive.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.5.1/yourtools/db/mysql.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.5.1/yourtools/Azkaban.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      723 2023-04-14 09:47:09.000000 yourtools-0.5.1/yourtools/Time.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     5929 2023-04-14 10:23:17.000000 yourtools-0.5.1/yourtools/WeChat.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      469 2023-04-13 08:48:52.000000 yourtools-0.5.1/yourtools/__init__.py
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/requires.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/top_level.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.5.1/README.md
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.5.1/requirements.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-07 10:28:09.000000 yourtools-0.5.1/setup.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 10:39:04.000000 yourtools-0.5.1/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-14 10:39:04.000000 yourtools-0.5.1/setup.cfg
```

### Comparing `yourtools-0.4.9/yourtools/db/dbutils.py` & `yourtools-0.5.1/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.9/yourtools/db/hive.py` & `yourtools-0.5.1/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.9/yourtools/db/mysql.py` & `yourtools-0.5.1/yourtools/db/mysql.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.9/yourtools/Azkaban.py` & `yourtools-0.5.1/yourtools/Azkaban.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.9/yourtools/Time.py` & `yourtools-0.5.1/yourtools/Time.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.9/yourtools/WeChat.py` & `yourtools-0.5.1/yourtools/WeChat.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,35 +8,66 @@
 @filename   : WeChat.py
 @create time: 2022/9/27 2:54 PM
 @modify time: 2022/9/27 2:54 PM
 @describe   : 
 -------------------------------------------------
 """
 import json
+import os
 import requests
 from requests_toolbelt import MultipartEncoder
 
 
-def send_chat_msg(key, data):
-    """
-    发送机器人消息到企微群
-    :param key: 机器人地址key
-    :return:
-    """
-    try:
-        url = f"https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key={key}"
-        header = {
-            "Content-Type": "application/json"
-        }
-        response = requests.post(url, headers=header, data=json.dumps(data))
-        if response.status_code == 200:
-            result = json.loads(response.text)
-            return result
-    except Exception as err:
-        raise Exception("Send Chat Message error", err)
+class Chat:
+    def __init__(self, key):
+        self.url = f"https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key={key}"
+
+    def upload_media(self, filepath):
+        """
+        发送机器人消息到企微群
+        :param key: 机器人地址key
+        :return:
+        """
+        try:
+            headers = {
+                'Content-Type': 'multipart/form-data',
+            }
+            with open(filepath, 'rb') as f:
+                files = {
+                    'media': (os.path.basename(filepath), f.read())
+                }
+                response = requests.post(self.url, headers=headers, files=files)
+                if response.status_code == 200:
+                    result = json.loads(response.text)
+                    return result
+                else:
+                    print("HTTP Error:", response.status_code)
+                    return None
+        except Exception as err:
+            raise Exception("upload_media error", err)
+
+    def send_chat_msg(self, data):
+        """
+        发送机器人消息到企微群
+        :param key: 机器人地址key
+        :return:
+        """
+        try:
+            header = {
+                "Content-Type": "application/json"
+            }
+            response = requests.post(self.url, headers=header, data=json.dumps(data))
+            if response.status_code == 200:
+                result = json.loads(response.text)
+                return result
+            else:
+                print("HTTP Error:", response.status_code)
+                return None
+        except Exception as err:
+            raise Exception("Send Chat Message error", err)
 
 
 class WeChat:
     def __init__(self, corpid, corpsecret, agentid):
         self.corpid = corpid
         self.corpsecret = corpsecret
         self.agentid = agentid
@@ -47,26 +78,32 @@
             if all([self.corpid, self.corpsecret]):
                 url = "https://qyapi.weixin.qq.com/cgi-bin/gettoken?corpid={corpid}&corpsecret={corpsecret}".format(
                     corpid=self.corpid, corpsecret=self.corpsecret)
                 response = requests.get(url)
                 if response.status_code == 200:
                     result = json.loads(response.text)
                     return result['access_token']
+                else:
+                    print("HTTP Error:", response.status_code)
+                    return None
         except Exception as err:
             raise Exception("get WeChat access Token error", err)
 
     def _send_msg(self, data):
         self._check_token()
         try:
             send_url = "https://qyapi.weixin.qq.com/cgi-bin/message/send?access_token={access_token}".format(
                 access_token=self.access_token)
             response = requests.post(send_url, json.dumps(data))
             if response.status_code == 200:
                 result = json.loads(response.text)
                 return result
+            else:
+                print("HTTP Error:", response.status_code)
+                return None
         except Exception as err:
             raise Exception("send WeChat Message error", err)
 
     def _check_token(self):
         if self.access_token is None:
             self._getToken()
```

### Comparing `yourtools-0.4.9/yourtools.egg-info/PKG-INFO` & `yourtools-0.5.1/yourtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.4.9
+Version: 0.5.1
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.4.9/README.md` & `yourtools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.9/setup.py` & `yourtools-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.4.9/PKG-INFO` & `yourtools-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.4.9
+Version: 0.5.1
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

