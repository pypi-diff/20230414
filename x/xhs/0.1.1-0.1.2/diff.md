# Comparing `tmp/xhs-0.1.1.tar.gz` & `tmp/xhs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.1.tar", last modified: Mon Apr 10 14:16:58 2023, max compression
+gzip compressed data, was "xhs-0.1.2.tar", last modified: Fri Apr 14 03:41:24 2023, max compression
```

## Comparing `xhs-0.1.1.tar` & `xhs-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:16:58.464274 xhs-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-10 14:16:45.000000 xhs-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-10 14:16:45.000000 xhs-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 14:16:45.000000 xhs-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-10 14:16:58.464274 xhs-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-10 14:16:45.000000 xhs-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-10 14:16:45.000000 xhs-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-10 14:16:58.464274 xhs-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-10 14:16:45.000000 xhs-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:16:58.460274 xhs-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 14:16:45.000000 xhs-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-10 14:16:45.000000 xhs-0.1.1/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-10 14:16:45.000000 xhs-0.1.1/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-10 14:16:45.000000 xhs-0.1.1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:16:58.460274 xhs-0.1.1/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-10 14:16:45.000000 xhs-0.1.1/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:16:58.464274 xhs-0.1.1/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 14:16:58.000000 xhs-0.1.1/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:41:24.414005 xhs-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 03:41:10.000000 xhs-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 03:41:10.000000 xhs-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 03:41:10.000000 xhs-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-14 03:41:24.414005 xhs-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-14 03:41:10.000000 xhs-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 03:41:10.000000 xhs-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 03:41:24.418005 xhs-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-14 03:41:10.000000 xhs-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:41:24.414005 xhs-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 03:41:10.000000 xhs-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-14 03:41:10.000000 xhs-0.1.2/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-14 03:41:10.000000 xhs-0.1.2/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 03:41:10.000000 xhs-0.1.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:41:24.414005 xhs-0.1.2/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-14 03:41:10.000000 xhs-0.1.2/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:41:24.414005 xhs-0.1.2/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 03:41:24.000000 xhs-0.1.2/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.1.1/CHANGELOG.md` & `xhs-0.1.2/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.1.2
+
+### ADD
+
+- add get user all notes
+
+### Changed
+
+- change properties setter getter
+
 ## 0.1.1
 
 ### ADD
 
 - add search sort and note_type args
 
 ### FIX
```

### Comparing `xhs-0.1.1/LICENSE` & `xhs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.1.1/PKG-INFO` & `xhs-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.1
+Version: 0.1.2
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
@@ -67,14 +67,21 @@
 # search note
 notes = xhs_client.get_note_by_keyword("小红书")
 
 # get home recommend feed
 recommend_type = FeedType.RECOMMEND
 recommend_notes = xhs_client.get_home_feed(recommend_type)
 
+# save notes file in disk
+xhs_client.save_files_from_note_id("63db8819000000001a01ead1",
+                                       r"C:\Users\User\Desktop"
+
+# get user all note detail
+notes = xhs_client.get_user_all_notes("5c2766b500000000050283f1")
+
 # more functions in development
 ```
 
 Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
 
 use signature function:
```

### Comparing `xhs-0.1.1/README.md` & `xhs-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,21 @@
 # search note
 notes = xhs_client.get_note_by_keyword("小红书")
 
 # get home recommend feed
 recommend_type = FeedType.RECOMMEND
 recommend_notes = xhs_client.get_home_feed(recommend_type)
 
+# save notes file in disk
+xhs_client.save_files_from_note_id("63db8819000000001a01ead1",
+                                       r"C:\Users\User\Desktop"
+
+# get user all note detail
+notes = xhs_client.get_user_all_notes("5c2766b500000000050283f1")
+
 # more functions in development
 ```
 
 Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
 
 use signature function:
```

### Comparing `xhs-0.1.1/setup.py` & `xhs-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.1/tests/test_help.py` & `xhs-0.1.2/tests/test_help.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from xhs import help
 
 
 @pytest.fixture
 def header():
     return {
         "cookie": ('webId=e3455f4405340fc431af976dbf3de167;'
-                   "web_session=040069b253793fdd9ccd9bd21c364b0033a638;"),
+                   "web_session=040069b253793fdd9ccd9a5f01364b856d4088"),
         "user-agent": ("Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
                        "AppleWebKit/537.36 (KHTML, like Gecko)"
                        "Chrome/111.0.0.0 Safari/537.36")
     }
 
 
 def test_sign_get(header):
@@ -87,7 +87,13 @@
     }
     print(headers)
     response = requests.post(url, headers=headers, data=payload)
     json_data = response.json()
     print(json_data)
     assert json_data["code"] == 0
     print(json_data["data"])
+
+
+def test_cookie_to_dict():
+    cookie = "a1=1875ee347c84l911yfccaewmv2ntixkksu1c6vyu550000205660;"
+    cookie_dict = help.cookie_str_to_cookie_dict(cookie)
+    assert cookie_dict.get("a1")
```

### Comparing `xhs-0.1.1/tests/test_xhs.py` & `xhs-0.1.2/tests/test_xhs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 
 from .utils import beauty_print
 
 
 @pytest.fixture
 def xhs_client():
     return XhsClient(
-        cookie=('webId=e3455f4405340fc431af976dbf3de167;'
-                "web_session=040069b253793fdd9ccd9a5f01364b856d4088"))
+        cookie=("webId=3ceadc9abfc351b88b07b556afddab35;"
+                "web_session=040069b253793fdd9ccd9a5f01364b856d4088;"))
 
 
-def test_init_with_session_id():
-    cookie = "123123"
+def test_cookie_setter_getter():
+    cookie = "web_session=123"
     xhs_client = XhsClient(cookie)
-    assert xhs_client.get_cookie() == cookie
+    assert xhs_client.cookie == cookie
+    new_cookie = "web_session=456"
+    xhs_client.cookie = new_cookie
+    assert xhs_client.cookie == new_cookie
 
 
 def test_get_note_by_id(xhs_client: XhsClient):
     note_id = "6413cf6b00000000270115b5"
     data = xhs_client.get_note_by_id(note_id)
     beauty_print(data)
     assert data["note_id"] == note_id
@@ -57,14 +60,21 @@
 def test_get_user_notes(xhs_client: XhsClient):
     user_id = "63273a77000000002303cc9b"
     data = xhs_client.get_user_notes(user_id)
     beauty_print(data)
     assert len(data["notes"]) > 0
 
 
+@pytest.mark.skip()
+def test_get_user_all_notes(xhs_client: XhsClient):
+    user_id = "5c2766b500000000050283f1"
+    notes = xhs_client.get_user_all_notes(user_id, 0)
+    beauty_print(notes)
+
+
 def test_get_qrcode(xhs_client: XhsClient):
     data = xhs_client.get_qrcode()
     beauty_print(data)
     assert data["url"].startswith("xhsdiscover://")
 
 
 @pytest.mark.skip()
```

### Comparing `xhs-0.1.1/xhs/core.py` & `xhs-0.1.2/xhs/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import json
 import os
 import re
+import time
 from enum import Enum
+from typing import NamedTuple
 
 import requests
 
 from xhs.exception import DataFetchError
 
-from .help import get_search_id, sign
+from .help import (cookie_jar_to_cookie_str, get_search_id, sign,
+                   update_session_cookies_from_cookie)
 
 
 class FeedType(Enum):
     # 推荐
     RECOMMEND = "homefeed_recommend"
     # 穿搭
     FASION = "homefeed.fashion_v3"
@@ -58,14 +61,31 @@
     ALL = 0
     # only video
     VIDEO = 1
     # only image
     IMAGE = 2
 
 
+class Note(NamedTuple):
+    """note typle"""
+    note_id: str
+    title: str
+    desc: str
+    type: str
+    user: dict
+    img_urls: list
+    video_url: str
+    tag_list: list
+    at_user_list: list
+    collected_count: str
+    comment_count: str
+    liked_count: str
+    share_count: str
+
+
 def download_file(url: str, filename: str):
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
         with open(filename, 'wb') as f:
             for chunk in r.iter_content(chunk_size=8192):
                 f.write(chunk)
 
@@ -76,70 +96,71 @@
 
 class XhsClient:
     def __init__(self,
                  cookie=None,
                  user_agent=None,
                  timeout=10,
                  proxies=None):
-        """constructor
-
-        :param cookie: get it form your website, defaults to None
-        :type cookie: str, optional
-        :param user_agent: requests user agent, defaults to None
-        :type user_agent: str, optional
-        :param timeout: requests timeout, defaults to None
-        :type timeout: int, optional
-        :param proxies: requests proxies, defaults to None
-        :type proxies: dict, optional
-        """
-        self._user_agent = user_agent or ("Mozilla/5.0 "
-                                          "(Windows NT 10.0; Win64; x64) "
-                                          "AppleWebKit/537.36 "
-                                          "(KHTML, like Gecko) "
-                                          "Chrome/111.0.0.0 Safari/537.36")
+        """constructor"""
         self._cookie = cookie
         self._proxies = proxies
         self._session: requests.Session = requests.session()
+        update_session_cookies_from_cookie(self._session, cookie)
         self._timeout = timeout
         self._host = "https://edith.xiaohongshu.com"
+        user_agent = user_agent or ("Mozilla/5.0 "
+                                    "(Windows NT 10.0; Win64; x64) "
+                                    "AppleWebKit/537.36 "
+                                    "(KHTML, like Gecko) "
+                                    "Chrome/111.0.0.0 Safari/537.36")
+        self._session.headers = {
+            "user-agent": user_agent,
+            "Content-Type": "application/json"
+        }
 
-    def set_cookie(self, cookie: str):
-        self._cookie = cookie
-
-    def get_cookie(self):
-        return self._cookie
-
-    def get_user_agent(self):
-        return self._user_agent
-
-    def set_user_agent(self, user_agent: str):
-        self._user_agent = user_agent
+    @property
+    def cookie(self):
+        return cookie_jar_to_cookie_str(self._session)
+
+    @cookie.setter
+    def cookie(self, cookie: str):
+        update_session_cookies_from_cookie(self._session, cookie)
+
+    @property
+    def session(self):
+        return self._session
+
+    @property
+    def user_agent(self):
+        return self._session.headers.get("user-agent")
+
+    @user_agent.setter
+    def user_agent(self, user_agent: str):
+        self._session.headers.update({"user-agent": user_agent})
 
-    def get_proxies(self):
+    @property
+    def proxies(self):
         return self._proxies
 
-    def set_proxies(self, proxies: dict):
+    @proxies.setter
+    def proxies(self, proxies: dict):
         self._proxies = proxies
 
-    def get_timeout(self):
+    @property
+    def timeout(self):
         return self._timeout
 
-    def set_timeout(self, timeout):
+    @timeout.setter
+    def timeout(self, timeout):
         self._timeout = timeout
 
     def _pre_headers(self, url: str, data=None):
-        assert self._cookie
         signs = sign(url, data)
-        return {
-            "User-Agent": self._user_agent,
-            "cookie": self._cookie,
-            "x-s": signs["x-s"],
-            "x-t": signs["x-t"],
-            "Content-Type": "application/json"
-        }
+        self._session.headers.update({"x-s": signs["x-s"]})
+        self._session.headers.update({"x-t": signs["x-t"]})
 
     def request(self, method, url, **kwargs):
         response = self._session.request(
             method, url, timeout=self._timeout,
             proxies=self._proxies, **kwargs)
         data = response.json()
         if data["success"]:
@@ -148,24 +169,22 @@
             raise DataFetchError(data.get("msg", None))
 
     def get(self, uri: str, params=None):
         final_uri = uri
         if isinstance(params, dict):
             final_uri = (f"{uri}?"
                          f"{'&'.join([f'{k}={v}'for k,v in params.items()])}")
-        headers = self._pre_headers(final_uri)
-        return self.request(method="GET", url=f"{self._host}{final_uri}",
-                            headers=headers)
+        self._pre_headers(final_uri)
+        return self.request(method="GET", url=f"{self._host}{final_uri}")
 
     def post(self, uri: str, data: dict):
-        headers = self._pre_headers(uri, data)
+        self._pre_headers(uri, data)
         json_str = json.dumps(data, separators=(',', ':'), ensure_ascii=False)
         return self.request(method="POST", url=f"{self._host}{uri}",
-                            data=json_str.encode("utf-8"),
-                            headers=headers)
+                            data=json_str.encode("utf-8"))
 
     def get_note_by_id(self, note_id: str):
         """
         :param note_id: note_id you want to fetch
         :type note_id: str
         :return: {"time":1679019883000,"user":{"nickname":"nickname","avatar":"avatar","user_id":"user_id"},"image_list":[{"url":"https://sns-img-qc.xhscdn.com/c8e505ca-4e5f-44be-fe1c-ca0205a38bad","trace_id":"1000g00826s57r6cfu0005ossb1e9gk8c65d0c80","file_id":"c8e505ca-4e5f-44be-fe1c-ca0205a38bad","height":1920,"width":1440}],"tag_list":[{"id":"5be78cdfdb601f000100d0bc","name":"jk","type":"topic"}],"desc":"裙裙","interact_info":{"followed":false,"liked":false,"liked_count":"1732","collected":false,"collected_count":"453","comment_count":"30","share_count":"41"},"at_user_list":[],"last_update_time":1679019884000,"note_id":"6413cf6b00000000270115b5","type":"normal","title":"title"}
         :rtype: dict
@@ -193,25 +212,49 @@
             title = note_id
 
         new_dir_path = os.path.join(dir_path, title)
         if not os.path.exists(new_dir_path):
             os.mkdir(new_dir_path)
 
         if note["type"] == NoteType.VIDEO.value:
-            video = next(filter(lambda value: len(value), note["video"]["media"]["stream"].values()))[0]
-            video_url = video["master_url"]
+            video_url = self._get_video_url_from_note(note)
             video_filename = os.path.join(new_dir_path, f"{title}.mp4")
             download_file(video_url, video_filename)
         else:
-            imgs = note["image_list"]
-            for index, img in enumerate(imgs):
-                img_url = get_img_url_by_trace_id(img["trace_id"])
+            img_urls = self._get_img_urls_from_note(note)
+            for index, img_url in enumerate(img_urls):
                 img_file_name = os.path.join(new_dir_path, f"{title}{index}.png")
                 download_file(img_url, img_file_name)
 
+    def _get_img_urls_from_note(self, note) -> list:
+        """get all no watermark img url from note
+
+        :param note: note info
+        :type note: dict
+        :return: images url list
+        :rtype: list
+        """
+        imgs = note["image_list"]
+        if not len(imgs):
+            return []
+        return [get_img_url_by_trace_id(img["trace_id"]) for img in imgs]
+
+    def _get_video_url_from_note(self, note) -> str:
+        """find video url from note
+
+        :param note: note info
+        :type note: dict
+        :return: video url
+        :rtype: str
+        """
+        if not note.get("video"):
+            return ""
+        video = next(filter(lambda value: len(value), note["video"]["media"]["stream"].values()))[0]
+        return video["master_url"]
+
     def get_self_info(self):
         uri = "/api/sns/web/v1/user/selfinfo"
         res = self.get(uri)
         return res
 
     def get_user_info(self, user_id: str):
         """
@@ -267,22 +310,72 @@
             "search_id": get_search_id(),
             "sort": sort.value,
             "note_type": note_type.value
         }
         return self.post(uri, data)
 
     def get_user_notes(self, user_id: str, cursor: str = ""):
+        """get user notes just have simple info
+
+        :param user_id: user_id you want to fetch
+        :type user_id: str
+        :param cursor: return info has this argument, defaults to ""
+        :type cursor: str, optional
+        :return: {cursor:"", has_more:true,notes:[{cover:{},display_title:"",interact_info:{},note_id:"",type:"video"}]}
+        :rtype: dict
+        """
         uri = "/api/sns/web/v1/user_posted"
         params = {
             "num": 30,
             "cursor": cursor,
             "user_id": user_id
         }
         return self.get(uri, params)
 
+    def get_user_all_notes(self, user_id: str, crawl_interval: int = 1) -> list[Note]:
+        """get user all notes with more info
+
+        :param user_id: user_id you want to fetch
+        :type user_id: str
+        :param crawl_interval: sleep seconds, defaults to 1
+        :type crawl_interval: int, optional
+        :return: note info list
+        :rtype: list[Note]
+        """
+        has_more = True
+        cursor = ""
+        result = []
+        while has_more:
+            res = self.get_user_notes(user_id, cursor)
+            has_more = res["has_more"]
+            cursor = res["cursor"]
+            note_ids = map(lambda note: note["note_id"], res["notes"])
+
+            for note_id in note_ids:
+                note = self.get_note_by_id(note_id)
+                interact_info = note["interact_info"]
+                note_info = Note(
+                    note_id=note["note_id"],
+                    title=note["title"],
+                    desc=note["desc"],
+                    type=note["type"],
+                    user=note["user"],
+                    img_urls=self._get_img_urls_from_note(note),
+                    video_url=self._get_video_url_from_note(note),
+                    tag_list=note["tag_list"],
+                    at_user_list=note["at_user_list"],
+                    collected_count=interact_info["collected_count"],
+                    comment_count=interact_info["comment_count"],
+                    liked_count=interact_info["liked_count"],
+                    share_count=interact_info["share_count"],
+                )
+                result.append(note_info)
+                time.sleep(crawl_interval)
+        return result
+
     def comment_note(self, note_id: str, content: str):
         """comment a note
 
         :return: {"time":1680834576180,"toast":"评论已发布","comment":{"id":"id","note_id":"note_id","status":2,"liked":false,"show_tags":["is_author"],"ip_location":"ip_location","content":"content","at_users":[],"like_count":"0","user_info":{"image":"**","user_id":"user_id","nickname":"nickname"},"create_time":create_time}}
         :rtype: dict
         """
         uri = "/api/sns/web/v1/comment/post"
```

### Comparing `xhs-0.1.1/xhs/help.py` & `xhs-0.1.2/xhs/help.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import hashlib
 import json
 import random
 import time
 
+import requests
+
 
 def sign(uri, data=None, ctime=None):
     """
     takes in a URI (uniform resource identifier), an optional data dictionary, and an optional ctime parameter. It returns a dictionary containing two keys: "x-s" and "x-t".
     """
     def h(n):
         m = ""
@@ -70,7 +72,25 @@
     return int(number, 36)
 
 
 def get_search_id():
     e = int(time.time() * 1000) << 64
     t = int(random.uniform(0, 2147483646))
     return base36encode((e + t))
+
+
+def cookie_str_to_cookie_dict(cookie_str: str):
+    cookie_blocks = [cookie_block.split("=")
+                     for cookie_block in cookie_str.split(";") if cookie_block]
+    return {cookie[0]: cookie[1] for cookie in cookie_blocks}
+
+
+def cookie_jar_to_cookie_str(session: requests.Session):
+    cookie_dict = requests.utils.dict_from_cookiejar(session.cookies)
+    return ";".join([f"{key}={value}" for key, value in cookie_dict.items()])
+
+
+def update_session_cookies_from_cookie(session: requests.Session, cookie: str):
+    cookies = session.cookies
+    new_cookies = requests.utils.add_dict_to_cookiejar(
+        cookies, cookie_str_to_cookie_dict(cookie))
+    session.cookies = new_cookies
```

### Comparing `xhs-0.1.1/xhs.egg-info/PKG-INFO` & `xhs-0.1.2/xhs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.1
+Version: 0.1.2
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
@@ -67,14 +67,21 @@
 # search note
 notes = xhs_client.get_note_by_keyword("小红书")
 
 # get home recommend feed
 recommend_type = FeedType.RECOMMEND
 recommend_notes = xhs_client.get_home_feed(recommend_type)
 
+# save notes file in disk
+xhs_client.save_files_from_note_id("63db8819000000001a01ead1",
+                                       r"C:\Users\User\Desktop"
+
+# get user all note detail
+notes = xhs_client.get_user_all_notes("5c2766b500000000050283f1")
+
 # more functions in development
 ```
 
 Please refer to the [document(WIP)](https://reajason.github.io/xhs/) for more API references.
 
 use signature function:
```

