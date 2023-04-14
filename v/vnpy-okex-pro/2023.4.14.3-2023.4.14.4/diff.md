# Comparing `tmp/vnpy-okex-pro-2023.4.14.3.tar.gz` & `tmp/vnpy-okex-pro-2023.4.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy-okex-pro-2023.4.14.3.tar", last modified: Thu Apr 13 09:32:43 2023, max compression
+gzip compressed data, was "vnpy-okex-pro-2023.4.14.4.tar", last modified: Fri Apr 14 05:58:33 2023, max compression
```

## Comparing `vnpy-okex-pro-2023.4.14.3.tar` & `vnpy-okex-pro-2023.4.14.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 09:32:43.834563 vnpy-okex-pro-2023.4.14.3/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.3/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-13 09:32:43.834656 vnpy-okex-pro-2023.4.14.3/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1619 2023-04-13 06:39:53.000000 vnpy-okex-pro-2023.4.14.3/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1014 2023-04-13 09:32:43.835108 vnpy-okex-pro-2023.4.14.3/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.3/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 09:32:43.831550 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1248 2023-04-13 06:38:53.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    33594 2023-04-13 09:07:29.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/okex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 09:32:43.834373 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      312 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 06:46:06.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       37 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       14 2023-04-13 09:32:43.000000 vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-14 05:58:33.751630 vnpy-okex-pro-2023.4.14.4/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.4/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-14 05:58:33.751747 vnpy-okex-pro-2023.4.14.4/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1619 2023-04-13 06:39:53.000000 vnpy-okex-pro-2023.4.14.4/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1014 2023-04-14 05:58:33.752255 vnpy-okex-pro-2023.4.14.4/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-13 01:56:35.000000 vnpy-okex-pro-2023.4.14.4/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-14 05:58:33.749593 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1248 2023-04-13 06:38:53.000000 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    33949 2023-04-14 01:49:08.000000 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro/okex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-14 05:58:33.751443 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2575 2023-04-14 05:58:33.000000 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      312 2023-04-14 05:58:33.000000 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-14 05:58:33.000000 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 06:46:06.000000 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       37 2023-04-14 05:58:33.000000 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       14 2023-04-14 05:58:33.000000 vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro.egg-info/top_level.txt
```

### Comparing `vnpy-okex-pro-2023.4.14.3/LICENSE` & `vnpy-okex-pro-2023.4.14.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.3/PKG-INFO` & `vnpy-okex-pro-2023.4.14.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-okex-pro
-Version: 2023.4.14.3
+Version: 2023.4.14.4
 Summary: OKEX gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-okex-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading,ctp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy-okex-pro-2023.4.14.3/README.md` & `vnpy-okex-pro-2023.4.14.4/README.md`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.3/setup.cfg` & `vnpy-okex-pro-2023.4.14.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy-okex-pro
-version = 2023.4.14.3
+version = 2023.4.14.4
 url = https://github.com/monk-after-90s/vnpy-okex-pro
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = OKEX gateway for vn.py quant trading framework.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/__init__.py` & `vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro/okex_gateway.py` & `vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro/okex_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,65 +417,72 @@
                 interval = time.time() - last_req_ts
                 if interval < 0.1:  # 间隔太短
                     sleep_seconds = 0.1 - interval
                     self.gateway.write_log(f"{sleep_seconds=}")
                     time.sleep(sleep_seconds)
             # 从服务器获取响应
             last_req_ts = time.time()
-            resp: Response = self.request(
-                "GET",
-                path,
-                params=params
-            )
-            # 如果请求失败则终止循环
-            if resp.status_code // 100 != 2:
-                msg = f"获取历史数据失败，状态码：{resp.status_code}，信息：{resp.text}"
-                self.gateway.write_log(msg)
-
-                if json.loads(resp.text)['code'] == '50011':
-                    time.sleep(0.5)
-                    self.gateway.write_log("重试")
-                    continue
-                else:
-                    break
-            else:
-                data: dict = resp.json()
 
-                if not data["data"]:
-                    # m = data["msg"]
-                    msg = f"获取历史数据结束"
+            try:
+                resp: Response = self.request(
+                    "GET",
+                    path,
+                    params=params
+                )
+            except:
+                time.sleep(5)
+                self.gateway.write_log("请求报错后重试")
+                continue
+            else:
+                # 如果请求失败则终止循环
+                if resp.status_code // 100 != 2:
+                    msg = f"获取历史数据失败，状态码：{resp.status_code}，信息：{resp.text}"
                     self.gateway.write_log(msg)
-                    break
 
-                data["data"].sort(key=lambda item: -int(item[0]))
+                    if json.loads(resp.text)['code'] == '50011':
+                        time.sleep(0.5)
+                        self.gateway.write_log("重试")
+                        continue
+                    else:
+                        break
+                else:
+                    data: dict = resp.json()
 
-                for bar_list in data["data"]:
-                    ts, o, h, l, c, vol, volCcy, volCcyQuote, confirm = bar_list
-                    dt = parse_timestamp(ts)
-                    bar: BarData = BarData(
-                        symbol=req.symbol,
-                        exchange=req.exchange,
-                        datetime=dt,
-                        interval=req.interval,
-                        volume=float(vol),
-                        open_price=float(o),
-                        high_price=float(h),
-                        low_price=float(l),
-                        close_price=float(c),
-                        gateway_name=self.gateway_name
-                    )
-                    buf[bar.datetime] = bar
-
-                begin: str = data["data"][-1][0]
-                end: str = data["data"][0][0]
-                msg: str = f"获取历史数据成功，{req.symbol} - {req.interval.value}，{parse_timestamp(begin)} - {parse_timestamp(end)}"
-                self.gateway.write_log(msg)
+                    if not data["data"]:
+                        # m = data["msg"]
+                        msg = f"获取历史数据结束"
+                        self.gateway.write_log(msg)
+                        break
+
+                    data["data"].sort(key=lambda item: -int(item[0]))
+
+                    for bar_list in data["data"]:
+                        ts, o, h, l, c, vol, volCcy, volCcyQuote, confirm = bar_list
+                        dt = parse_timestamp(ts)
+                        bar: BarData = BarData(
+                            symbol=req.symbol,
+                            exchange=req.exchange,
+                            datetime=dt,
+                            interval=req.interval,
+                            volume=float(vol),
+                            open_price=float(o),
+                            high_price=float(h),
+                            low_price=float(l),
+                            close_price=float(c),
+                            gateway_name=self.gateway_name
+                        )
+                        buf[bar.datetime] = bar
+
+                    begin: str = data["data"][-1][0]
+                    end: str = data["data"][0][0]
+                    msg: str = f"获取历史数据成功，{req.symbol} - {req.interval.value}，{parse_timestamp(begin)} - {parse_timestamp(end)}"
+                    self.gateway.write_log(msg)
 
-                # 更新结束时间
-                end_time = begin
+                    # 更新结束时间
+                    end_time = begin
 
         index: List[datetime] = list(buf.keys())
         index.sort()
 
         history: List[BarData] = [buf[i] for i in index]
         return history
```

### Comparing `vnpy-okex-pro-2023.4.14.3/vnpy_okex_pro.egg-info/PKG-INFO` & `vnpy-okex-pro-2023.4.14.4/vnpy_okex_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-okex-pro
-Version: 2023.4.14.3
+Version: 2023.4.14.4
 Summary: OKEX gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-okex-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading,ctp
 Classifier: Development Status :: 5 - Production/Stable
```

