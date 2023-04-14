# Comparing `tmp/vnpy_binance_pro-2023.4.13.1.tar.gz` & `tmp/vnpy_binance_pro-2023.4.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_binance_pro-2023.4.13.1.tar", last modified: Thu Apr 13 10:20:10 2023, max compression
+gzip compressed data, was "vnpy_binance_pro-2023.4.14.1.tar", last modified: Fri Apr 14 07:31:37 2023, max compression
```

## Comparing `vnpy_binance_pro-2023.4.13.1.tar` & `vnpy_binance_pro-2023.4.14.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 10:20:10.389105 vnpy_binance_pro-2023.4.13.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-13 07:25:05.000000 vnpy_binance_pro-2023.4.13.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-13 10:20:10.389219 vnpy_binance_pro-2023.4.13.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1165 2023-04-13 10:17:44.000000 vnpy_binance_pro-2023.4.13.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1028 2023-04-13 10:20:10.389785 vnpy_binance_pro-2023.4.13.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-13 07:25:05.000000 vnpy_binance_pro-2023.4.13.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 10:20:10.386283 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1460 2023-04-13 07:27:31.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31285 2023-04-13 07:36:35.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro/binance_inverse_gateway.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    28484 2023-04-13 09:40:18.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro/binance_spot_gateway.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31615 2023-04-13 09:57:46.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro/binance_usdt_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-13 10:20:10.388874 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-13 10:20:10.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      429 2023-04-13 10:20:10.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 10:20:10.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 10:20:10.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-04-13 10:20:10.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       17 2023-04-13 10:20:10.000000 vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-14 07:31:37.638879 vnpy_binance_pro-2023.4.14.1/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-13 07:25:05.000000 vnpy_binance_pro-2023.4.14.1/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-14 07:31:37.638978 vnpy_binance_pro-2023.4.14.1/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1165 2023-04-13 10:17:44.000000 vnpy_binance_pro-2023.4.14.1/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1028 2023-04-14 07:31:37.639464 vnpy_binance_pro-2023.4.14.1/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-13 07:25:05.000000 vnpy_binance_pro-2023.4.14.1/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-14 07:31:37.635753 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1460 2023-04-13 07:27:31.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31285 2023-04-13 07:36:35.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_inverse_gateway.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    28895 2023-04-14 04:01:41.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_spot_gateway.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31615 2023-04-14 05:30:18.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_usdt_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-14 07:31:37.638687 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      429 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-13 10:20:10.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       17 2023-04-14 07:31:37.000000 vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/top_level.txt
```

### Comparing `vnpy_binance_pro-2023.4.13.1/LICENSE` & `vnpy_binance_pro-2023.4.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.13.1/PKG-INFO` & `vnpy_binance_pro-2023.4.14.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_binance_pro
-Version: 2023.4.13.1
+Version: 2023.4.14.1
 Summary: BINANCE gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-binance-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_binance_pro-2023.4.13.1/README.md` & `vnpy_binance_pro-2023.4.14.1/README.md`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.13.1/setup.cfg` & `vnpy_binance_pro-2023.4.14.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_binance_pro
-version = 2023.4.13.1
+version = 2023.4.14.1
 url = https://github.com/monk-after-90s/vnpy-binance-pro
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = BINANCE gateway for vn.py quant trading framework.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro/__init__.py` & `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro/binance_inverse_gateway.py` & `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_inverse_gateway.py`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro/binance_spot_gateway.py` & `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_spot_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,30 +258,30 @@
 
         if security in [Security.SIGNED, Security.API_KEY]:
             request.headers = headers
 
         return request
 
     def connect(
-        self,
-        key: str,
-        secret: str,
-        proxy_host: str,
-        proxy_port: int,
-        server: str
+            self,
+            key: str,
+            secret: str,
+            proxy_host: str,
+            proxy_port: int,
+            server: str
     ) -> None:
         """连接REST服务器"""
         self.key = key
         self.secret = secret.encode()
         self.proxy_port = proxy_port
         self.proxy_host = proxy_host
         self.server = server
 
         self.connect_time = (
-            int(datetime.now(CHINA_TZ).strftime("%y%m%d%H%M%S")) * self.order_count
+                int(datetime.now(CHINA_TZ).strftime("%y%m%d%H%M%S")) * self.order_count
         )
 
         if self.server == "REAL":
             self.init(REST_HOST, proxy_host, proxy_port)
         else:
             self.init(TESTNET_REST_HOST, proxy_host, proxy_port)
 
@@ -544,15 +544,15 @@
         order.status = Status.REJECTED
         self.gateway.on_order(order)
 
         msg: str = f"委托失败，状态码：{status_code}，信息：{request.response.text}"
         self.gateway.write_log(msg)
 
     def on_send_order_error(
-        self, exception_type: type, exception_value: Exception, tb, request: Request
+            self, exception_type: type, exception_value: Exception, tb, request: Request
     ) -> None:
         """委托下单回报函数报错回报"""
         order: OrderData = request.extra
         order.status = Status.REJECTED
         self.gateway.on_order(order)
 
         if not issubclass(exception_type, (ConnectionError, SSLError)):
@@ -585,47 +585,56 @@
         self.trade_ws_api.connect(url, self.proxy_host, self.proxy_port)
 
     def on_keep_user_stream(self, data: dict, request: Request) -> None:
         """延长listenKey有效期回报"""
         pass
 
     def on_keep_user_stream_error(
-        self, exception_type: type, exception_value: Exception, tb, request: Request
+            self, exception_type: type, exception_value: Exception, tb, request: Request
     ) -> None:
         """延长listenKey有效期函数报错回报"""
         # 当延长listenKey有效期时，忽略超时报错
         if not issubclass(exception_type, TimeoutError):
             self.on_error(exception_type, exception_value, tb, request)
 
     def query_history(self, req: HistoryRequest) -> List[BarData]:
         """查询历史数据"""
         history: List[BarData] = []
         limit: int = 1000
         start_time: int = int(datetime.timestamp(req.start))
 
+        sleep_seconds = 0.5
         while True:
             # 创建查询参数
             params: dict = {
                 "symbol": req.symbol.upper(),
                 "interval": INTERVAL_VT2BINANCE[req.interval],
                 "limit": limit,
-                "startTime": start_time * 1000,         # 转换成毫秒
+                "startTime": start_time * 1000,  # 转换成毫秒
             }
 
             if req.end:
                 end_time: int = int(datetime.timestamp(req.end))
-                params["endTime"] = end_time * 1000     # 转换成毫秒
+                params["endTime"] = end_time * 1000  # 转换成毫秒
 
             resp: Response = self.request(
                 "GET",
                 "/api/v3/klines",
                 data={"security": Security.NONE},
                 params=params
             )
 
+            if resp.status_code == 429:
+                self.gateway.write_log(f"{resp.status_code=},{resp.text=}")
+                self.gateway.write_log(f"{sleep_seconds=} for retring connection")
+                time.sleep(sleep_seconds)
+                sleep_seconds *= 2
+                continue
+            else:
+                sleep_seconds = 0.5
             # 如果请求失败则终止循环
             if resp.status_code // 100 != 2:
                 msg: str = f"获取历史数据失败，状态码：{resp.status_code}，信息：{resp.text}"
                 self.gateway.write_log(msg)
                 break
             else:
                 data: dict = resp.json()
@@ -694,20 +703,20 @@
         if packet["e"] == "outboundAccountPosition":
             self.on_account(packet)
         elif packet["e"] == "executionReport":
             self.on_order(packet)
         elif packet["e"] == "listenKeyExpired":
             self.on_listen_key_expired()
 
-    def on_listen_key_expired(self) ->None:
+    def on_listen_key_expired(self) -> None:
         """ListenKey过期"""
         self.gateway.write_log("listenKey过期")
         self.disconnect()
 
-    def disconnect(self) ->None:
+    def disconnect(self) -> None:
         """"主动断开webscoket链接"""
         self._active = False
         ws = self._ws
         if ws:
             coro = ws.close()
             run_coroutine_threadsafe(coro, self._loop)
```

### Comparing `vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro/binance_usdt_gateway.py` & `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro/binance_usdt_gateway.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -691,16 +691,16 @@
                 path=path,
                 data={"security": Security.NONE},
                 params=params
             )
             # 限速控制
             if resp.status_code == 429:
                 self.gateway.write_log(f"{resp.status_code=},{resp.text=}")
-                time.sleep(sleep_seconds)
                 self.gateway.write_log(f"{sleep_seconds=} for retring connection")
+                time.sleep(sleep_seconds)
                 sleep_seconds *= 2
                 continue
             else:
                 sleep_seconds = 0.5
             # 如果请求失败则终止循环
             if resp.status_code // 100 != 2:
                 msg: str = f"获取历史数据失败，状态码：{resp.status_code}，信息：{resp.text}"
```

### Comparing `vnpy_binance_pro-2023.4.13.1/vnpy_binance_pro.egg-info/PKG-INFO` & `vnpy_binance_pro-2023.4.14.1/vnpy_binance_pro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-binance-pro
-Version: 2023.4.13.1
+Version: 2023.4.14.1
 Summary: BINANCE gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-binance-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

