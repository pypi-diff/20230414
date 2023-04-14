# Comparing `tmp/nonebot_plugin_BitTorrent-0.0.6.tar.gz` & `tmp/nonebot_plugin_BitTorrent-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_BitTorrent-0.0.6.tar", last modified: Sun Mar 26 14:05:33 2023, max compression
+gzip compressed data, was "nonebot_plugin_BitTorrent-0.0.7.tar", last modified: Fri Apr 14 13:42:13 2023, max compression
```

## Comparing `nonebot_plugin_BitTorrent-0.0.6.tar` & `nonebot_plugin_BitTorrent-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 14:05:33.966301 nonebot_plugin_BitTorrent-0.0.6/
--rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_BitTorrent-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      305 2023-03-26 14:05:33.966301 nonebot_plugin_BitTorrent-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2022-06-23 16:37:02.000000 nonebot_plugin_BitTorrent-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-26 14:05:33.954739 nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent/
--rw-rw-rw-   0        0        0      217 2023-03-26 13:48:38.000000 nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent/__init__.py
--rw-rw-rw-   0        0        0     5342 2023-03-26 13:50:34.000000 nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-26 14:05:33.964301 nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent.egg-info/
--rw-rw-rw-   0        0        0      305 2023-03-26 14:05:33.000000 nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-03-26 14:05:33.000000 nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 14:05:33.000000 nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-26 14:05:33.000000 nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-03-26 14:05:33.000000 nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-26 14:05:33.967301 nonebot_plugin_BitTorrent-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      534 2023-03-26 14:05:16.000000 nonebot_plugin_BitTorrent-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:42:13.252030 nonebot_plugin_BitTorrent-0.0.7/
+-rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_BitTorrent-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      305 2023-04-14 13:42:13.251028 nonebot_plugin_BitTorrent-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2022-06-23 16:37:02.000000 nonebot_plugin_BitTorrent-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 13:42:13.244030 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent/
+-rw-rw-rw-   0        0        0      217 2023-04-14 12:38:11.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent/__init__.py
+-rw-rw-rw-   0        0        0     6121 2023-04-14 13:36:51.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:42:13.250030 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/
+-rw-rw-rw-   0        0        0      305 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-14 13:42:13.000000 nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:42:13.252030 nonebot_plugin_BitTorrent-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      534 2023-04-14 13:42:01.000000 nonebot_plugin_BitTorrent-0.0.7/setup.py
```

### Comparing `nonebot_plugin_BitTorrent-0.0.6/LICENSE` & `nonebot_plugin_BitTorrent-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_BitTorrent-0.0.6/README.md` & `nonebot_plugin_BitTorrent-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_BitTorrent-0.0.6/nonebot_plugin_BitTorrent/utils.py` & `nonebot_plugin_BitTorrent-0.0.7/nonebot_plugin_BitTorrent/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import base64
 import random
 import re
 
 import nonebot
 from bs4 import BeautifulSoup
 from httpx import AsyncClient
 from nonebot.adapters.onebot.v11 import Message
@@ -13,36 +14,37 @@
 class BitTorrent:
     def __init__(self) -> None:
         """初始化一些变量, 用env拿到magnet_max_num参数"""
         try:
             self.max_num = nonebot.get_driver().config.magnet_max_num
         except Exception:
             self.max_num = 3
-        self.headers = {
-            "cookie": "",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.5005.124 Safari/537.36 Edg/102.0.1245.44",
-        }
+        # self.headers = {
+        #     "cookie": "",
+        #     "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.5005.124 Safari/537.36 Edg/102.0.1245.44",
+        # }
         self.magnet_url = "https://clm9.me"
 
 
     async def main(self, matcher: Matcher, msg: Message = CommandArg()):
         """主函数, 用于响应命令"""
         keyword = msg.extract_plain_text()
         if keyword == "":
             await matcher.finish("虚空搜索?来点车牌gkd")
         search_url = f"https://clm9.me/search?word={keyword}"
-        try:
-            # 尝试cookie
-            cookie = await self.get_cookie()
-            if cookie != "":
-                self.headers["cookie"] = cookie
-            else:
-                await matcher.finish("获取cookie失败, 可能网络出现问题, 也可能是代码有bug(不可能, 绝对不可能)")
-        except Exception as e:
-            await matcher.finish("获取cookie失败, 下面是错误信息:\n" + str(e))
+
+        # try:
+        #     # 尝试cookie
+        #     cookie = await self.get_cookie()
+        #     if cookie != "":
+        #         self.headers["cookie"] = cookie
+        #     else:
+        #         await matcher.finish("获取cookie失败, 可能网络出现问题, 也可能是代码有bug(不可能, 绝对不可能)")
+        # except Exception as e:
+        #     await matcher.finish("获取cookie失败, 下面是错误信息:\n" + str(e))
         try:
             # 尝试获取消息
             message = await self.get_magnet(search_url)
         except Exception as e:
             # 获取失败的时候返回错误信息
             await matcher.finish("搜索失败, 下面是错误信息:\n" + str(e))
         # 如果搜索到了结果, 则尝试发送, 有些账号好像文本太长cqhttp会显示风控
@@ -55,16 +57,22 @@
             await matcher.finish("没有找到结果捏, 换个关键词试试吧, 多次搜索失败可能是cookie出了问题")
 
 
 
     async def get_magnet(self, url: str) -> str:
         """传入搜索的url, 返回发送的消息"""
         async with AsyncClient() as client:
-            res = await client.get(url=url, headers=self.headers, timeout=30) # 发送请求
-            res = res.text
+            res = await client.get(url=url, timeout=30) # 发送请求
+            if "window.location.href" in res.text and "检测中" in res.text:
+                # 发生了重定向, 重新获取url
+                print(f"重定向\n{res.text}")
+                url = re.findall(r'window.location.href ="(.*?)"', res.text)[0]
+                url = self.magnet_url + url
+                res = await client.get(url=url, timeout=30)
+            res = await self.release_b64(res.text)
             soup = BeautifulSoup(res, "lxml")
             item_lst = soup.find_all(
                 "a", {"class": "SearchListTitle_result_title"})
             async with AsyncClient() as client2:
                 tasks = []
                 # 获取每一个url, 异步访问
                 for item in item_lst:
@@ -77,43 +85,55 @@
         message_list = random.sample(data, num)     # 随机选择一些条目
         message = ""
         # message拼接
         for msg in message_list:
             message = message + msg + "\n"
         print(message)                              # 在控制台输出一下
         return message
+    
+
+    # async def get_cookie(self) -> str:
+    #     """获取cookie"""
+    #     # 临时的访问头
+    #     get_cookie_headers = {"user-agent": self.headers["user-agent"]}
+    #     async with AsyncClient() as client:
+    #         response = await client.post(url=self.magnet_url, data={"act": "challenge"}, headers=get_cookie_headers)
+    #         if response.status_code != 200:  # 如果返回码不是200, 则返回空字符串
+    #             response.raise_for_status()  # 抛出异常
+    #             return ""   # 返回空字符串
+    #         cookies = response.headers.get("Set-Cookie")    # 获取cookie
+    #     if cookies is None:
+    #         return ""   # 获取失败返回空字符串
+    #     if match := re.search("test=([^;]+);", cookies):
+    #         test = match[1]
+    #         return f"ex=1; test={test}"
+    #     else:
+    #         return ""   # 获取失败返回空字符串
 
-    async def get_cookie(self) -> str:
-        """获取cookie"""
-        # 临时的访问头
-        get_cookie_headers = {"user-agent": self.headers["user-agent"]}
-        async with AsyncClient() as client:
-            response = await client.post(url=self.magnet_url, data={"act": "challenge"}, headers=get_cookie_headers)
-            if response.status_code != 200:  # 如果返回码不是200, 则返回空字符串
-                response.raise_for_status()  # 抛出异常
-                return ""   # 返回空字符串
-            cookies = response.headers.get("Set-Cookie")    # 获取cookie
-        if cookies is None:
-            return ""   # 获取失败返回空字符串
-        if match := re.search("test=([^;]+);", cookies):
-            test = match[1]
-            return f"ex=1; test={test}"
-        else:
-            return ""   # 获取失败返回空字符串
 
 
     async def get_info(self, url: str, client: AsyncClient) -> str:
         """传入一个url, 返回一个字符串"""
-        res = await client.get(url=url, headers=self.headers, timeout=30)
-        res = res.text
+        res = await client.get(url=url, timeout=30)
+        res = await self.release_b64(res.text)
         soup = BeautifulSoup(res, "lxml")
         information_content = soup.find_all("div", {"class": "Information_l_content"})
         magnet = information_content[0].find("a").get("href")           # 这个是磁力链接
         size = list(information_content[1])[4]                          #  这个是文件大小
         size = re.sub(u"\\<.*?\\>", "", str(size))
         name = soup.find_all('div', {'class': 'File_list_info'})        # 访问File_list_info, 目的是为了获取文件名
         name = list(name[0])[0]
         return f"文件名: {name} \n大小: {size}\n链接: {magnet}\n"
     
 
+
+    async def release_b64(self, target: str) -> str:
+        """解除网页的base64加密, 传入get得到的text"""
+        soup = BeautifulSoup(target, "lxml")
+        script = soup.find_all("script")[-1]
+        script = str(script).split('"')[1]
+        return base64.b64decode(script).decode()
+
+    
+
 # 实例化
 bittorrent = BitTorrent()
```

### Comparing `nonebot_plugin_BitTorrent-0.0.6/setup.py` & `nonebot_plugin_BitTorrent-0.0.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_BitTorrent'
 
 setup(
     name=name,  
-    version='0.0.6',
+    version='0.0.7',
     author="Special-Week",
     author_email='2749903559@qq.com',
     description="encapsulate logger",
     python_requires=">=3.8.*",
     packages=find_packages(),
     long_description="nonebot2磁力搜索插件",
     url="https://github.com/Special-Week/nonebot_plugin_BitTorrent",
```

