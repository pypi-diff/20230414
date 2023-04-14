# Comparing `tmp/freechatgpt-1.3.4.tar.gz` & `tmp/freechatgpt-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/freechatgpt-1.3.4.tar", last modified: Thu Apr 13 07:31:17 2023, max compression
+gzip compressed data, was "dist/freechatgpt-1.3.5.tar", last modified: Fri Apr 14 06:14:37 2023, max compression
```

## Comparing `freechatgpt-1.3.4.tar` & `freechatgpt-1.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/
--rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      461 2023-03-02 04:28:25.000000 freechatgpt-1.3.4/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/freechatgpt/
--rw-r--r--   0 admin      (501) staff       (20)      144 2023-03-02 03:57:41.000000 freechatgpt-1.3.4/freechatgpt/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     5103 2023-04-13 07:23:05.000000 freechatgpt-1.3.4/freechatgpt/free_chatgpt.py
--rw-r--r--   0 admin      (501) staff       (20)      435 2023-04-12 04:56:51.000000 freechatgpt-1.3.4/freechatgpt/ip_util.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/freechatgpt.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      267 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       33 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2023-04-13 07:31:16.000000 freechatgpt-1.3.4/freechatgpt.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-13 07:31:17.000000 freechatgpt-1.3.4/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1361 2023-04-13 07:30:52.000000 freechatgpt-1.3.4/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/
+-rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      461 2023-03-02 04:28:25.000000 freechatgpt-1.3.5/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/freechatgpt/
+-rw-r--r--   0 admin      (501) staff       (20)      144 2023-03-02 03:57:41.000000 freechatgpt-1.3.5/freechatgpt/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     5294 2023-04-14 06:14:32.000000 freechatgpt-1.3.5/freechatgpt/free_chatgpt.py
+-rw-r--r--   0 admin      (501) staff       (20)      435 2023-04-12 04:56:51.000000 freechatgpt-1.3.5/freechatgpt/ip_util.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/freechatgpt.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1590 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/freechatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      267 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/freechatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/freechatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       40 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/freechatgpt.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/freechatgpt.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-14 06:14:37.000000 freechatgpt-1.3.5/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1378 2023-04-14 06:03:56.000000 freechatgpt-1.3.5/setup.py
```

### Comparing `freechatgpt-1.3.4/PKG-INFO` & `freechatgpt-1.3.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freechatgpt
-Version: 1.3.4
+Version: 1.3.5
 Summary: free chatgpt api, not need token
 Home-page: https://github.com/abo123456789
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
```

### Comparing `freechatgpt-1.3.4/freechatgpt/free_chatgpt.py` & `freechatgpt-1.3.5/freechatgpt/free_chatgpt.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,95 +5,65 @@
 import json
 import urllib.parse
 from abc import ABCMeta
 from json import JSONDecodeError
 
 import requests
 import retrying
+from detool import timer_cost
 from requests import ReadTimeout
 
 from freechatgpt.ip_util import IpTool
 
 
 def retry_if_timeout_error(excep):
     return isinstance(excep, ReadTimeout)
 
 
 class FreeChatgpt(object):
 
     @staticmethod
-    def __ask(question: str) -> dict:
-        try:
-            @retrying.retry(stop_max_attempt_number=4, stop_max_delay=100000,
-                            wait_fixed=1500, retry_on_exception=retry_if_timeout_error)
-            def ask_q():
-                if not question or not question.strip():
-                    return {'code': 0, 'error': 'question is null!'}
-                # url = f'https://api.wqwlkj.cn/wqwlapi/chatgpt.php?msg={question.strip()}&type=json'
-                # url = f"http://www.emmapi.com/chatgpt?text={question.strip()}"
-                url = f"https://v1.apigpt.cn/?q={question.strip()}"
-                # url = f"https://api.caonm.net/api/ai/o.php?msg={question.strip()}"
-                # url = f"https://api.caonm.net/api/ai/o.php?msg={question.strip()}"
-                print('AI问题思考中=====')
-                res = requests.get(url, timeout=70)
-                answer_q = None
-                try:
-                    if not res.text:
-                        raise ReadTimeout()
-                    print(res.text)
-                    res_json = json.loads(res.text)
-
-                    answer_q = res_json.get("ChatGPT_Answer")
-                    print(f'AI问题回答:{answer_q}')
-                    # if res_json.get('info'):
-                    #     del res_json['info']
-                except JSONDecodeError:
-                    return {'code': 0, 'error': answer_q}
-                return {'code': 1, 'text': answer_q}
-
-            return ask_q()
-        except ReadTimeout:
-            return {'code': 0, 'error': 'ReadTimeout,please retry'}
-
-    @staticmethod
+    @timer_cost
     def ask(question: str):
         try:
-            @retrying.retry(stop_max_attempt_number=4, stop_max_delay=100000,
-                            wait_fixed=1500, retry_on_exception=retry_if_timeout_error)
+            @retrying.retry(stop_max_attempt_number=5, stop_max_delay=100*1000,
+                            wait_fixed=1000, retry_on_exception=retry_if_timeout_error)
             def ask_q():
                 if not question or not question.strip():
                     return {'code': 0, 'error': 'question is null!'}
                 print('AI问题思考中=====')
                 answer_q = None
                 try:
-                    answer_q = PlatformGptStore(question)._get_chat_res()
+                    answer_q = PlatformGptZxx(question)._get_chat_res()
                     print(f'AI问题回答:{answer_q}')
                     return answer_q
                 except JSONDecodeError:
                     return {'code': 0, 'error': answer_q}
 
             return ask_q()
         except ReadTimeout:
             return {'code': 0, 'error': 'ReadTimeout,please retry'}
 
 
 class BasePlatform(metaclass=ABCMeta):
     def __init__(self, question: str):
-        self.question = question
+        if question:
+            self.question = urllib.parse.quote(question)
+        else:
+            raise Exception('question is null')
 
     def _get_chat_res(self) -> str:
         pass
 
 
 class PlatformGptStore(BasePlatform):
     def _get_chat_res(self) -> str:
         url = "http://free-gpt.fun/chatgpt.php"
-        msg = urllib.parse.quote(self.question)
         ip = IpTool.get_host_ip() or '121.78.25.14'
-        payload = f'message={msg}&mychat_ip={ip}&user_uuid=CHAT-APIGPT-oj3uoj-gxhg-3u9ut-oj6q'
+        payload = f'message={self.question}&mychat_ip={ip}&user_uuid=CHAT-APIGPT-oj3uoj-gxhg-3u9ut-oj6q'
         headers = {
             'Accept': '*/*',
             'Accept-Encoding': 'gzip, deflate',
             'Accept-Language': 'en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7',
             'Connection': 'keep-alive',
             'Content-Length': '83',
             'Content-Type': 'application/x-www-form-urlencoded',
@@ -106,18 +76,61 @@
         }
 
         response = requests.request("POST", url, headers=headers, data=payload, timeout=60)
         rs = response.text.split('答：')[1].strip('<br />').strip('<br />')
         return rs
 
 
+class PlatformGptZxx(BasePlatform):
+
+    @retrying.retry(stop_max_attempt_number=3)
+    def _get_chat_res(self) -> str:
+        url = "https://chat.zhuleixx.top/api"
+
+        payload = "{\"messages\":[{\"role\":\"user\",\"content\":\"" + self.question + "\"}],\"temperature\":0.6,\"password\":\"\",\"model\":\"gpt-3.5-turbo\"}\n"
+        headers = {
+            'authority': 'chat.zhuleixx.top',
+            'method': 'POST',
+            'path': '/api',
+            'scheme': 'https',
+            'accept': '*/*',
+            'accept-encoding': 'gzip, deflate, br',
+            'accept-language': 'en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7',
+            'content-type': 'text/plain;charset=UTF-8',
+            'cookie': 'Hm_lvt_220930121be5ed42a5f54a30151d15ae=1681444427; Hm_lpvt_220930121be5ed42a5f54a30151d15ae=1681444427',
+            'origin': 'https://chat.zhuleixx.top',
+            'referer': 'https://chat.zhuleixx.top/',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'same-origin',
+            'user-agent': 'Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload, timeout=30)
+
+        return response.text
+
+
+class PlatformGptApi(BasePlatform):
+
+    def _get_chat_res(self) -> str:
+        url = f"https://v1.apigpt.cn/?q={self.question}"
+        res = requests.get(url, timeout=70)
+        if not res.text:
+            raise ReadTimeout()
+        res_json = json.loads(res.text)
+
+        answer_q = res_json.get("ChatGPT_Answer")
+        return answer_q
+
+
 if __name__ == '__main__':
     # r = FreeChatgpt.ask(question='帮我优化这段话:pandas快速替换所有字符中的特殊字符')
     # print(r)
     # t = FreeChatgpt.ask(question='中国文化的特点是什么？')
     # print(t)
-    # q = '根据我的预算6000元,风险偏好中等风险,预期收益率1.3%,请为我提供一种个人理财方案'
-    # s = FreeChatgpt.ask(question=q)
-    # print(s)
+    q = '根据我的预算9000元,风险偏好进取型,预期收益率10.3%,请为我提供一种个人理财方案'
+    s = FreeChatgpt.ask(question=q)
+    print(s)
 
-    r = FreeChatgpt.ask(question='帮我创作一个广告视频OPPO卖点？')
-    print(r)
+    # r = FreeChatgpt.ask(question='帮我创作一个广告视频OPPO卖点？')
+    # print(r)
```

### Comparing `freechatgpt-1.3.4/freechatgpt.egg-info/PKG-INFO` & `freechatgpt-1.3.5/freechatgpt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freechatgpt
-Version: 1.3.4
+Version: 1.3.5
 Summary: free chatgpt api, not need token
 Home-page: https://github.com/abo123456789
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
```

### Comparing `freechatgpt-1.3.4/setup.py` & `freechatgpt-1.3.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # @Author abo123456789
 # @TIME 2019/5/25 23:26
 
 from setuptools import setup, find_packages
 
 setup(
     name='freechatgpt',
-    version='1.3.4',
+    version='1.3.5',
     description=(
         'free chatgpt api, not need token'
     ),
     keywords=(
         "chatgpt,free"),
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding='utf-8').read(),
@@ -18,14 +18,15 @@
     author_email='abcdef123456chen@sohu.com',
     maintainer='abo123456789',
     maintainer_email='abcdef123456chen@sohu.com',
     license='MIT License',
     install_requires=[
         "requests>=2.12.3",
         "retrying>=1.3.3",
+        "detool"
     ],
     url='https://github.com/abo123456789',
     packages=find_packages(),
     platforms=["all"],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Operating System :: OS Independent',
```

