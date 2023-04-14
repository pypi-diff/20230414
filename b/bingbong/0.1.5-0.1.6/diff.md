# Comparing `tmp/bingbong-0.1.5-py3-none-any.whl.zip` & `tmp/bingbong-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 9992 bytes, number of entries: 14
--rw-rw-rw-  2.0 unx       53 b- defN 23-Apr-13 23:18 pingpong/__init__.py
--rw-rw-rw-  2.0 unx      853 b- defN 23-Apr-12 04:50 pingpong/alpaca.py
+Zip file size: 10910 bytes, number of entries: 15
+-rw-rw-rw-  2.0 unx       53 b- defN 23-Apr-14 05:21 pingpong/__init__.py
+-rw-rw-rw-  2.0 unx     1234 b- defN 23-Apr-14 05:21 pingpong/alpaca.py
+-rw-rw-rw-  2.0 unx     1229 b- defN 23-Apr-14 05:21 pingpong/dolly.py
 -rw-rw-rw-  2.0 unx      583 b- defN 23-Apr-12 04:44 pingpong/gradio.py
--rw-rw-rw-  2.0 unx      662 b- defN 23-Apr-12 04:40 pingpong/pingpong.py
+-rw-rw-rw-  2.0 unx     1046 b- defN 23-Apr-14 05:14 pingpong/pingpong.py
 -rw-rw-rw-  2.0 unx      173 b- defN 23-Apr-12 04:36 pingpong/context/__init__.py
 -rw-rw-rw-  2.0 unx      589 b- defN 23-Apr-12 00:59 pingpong/context/auto_summary_strategy.py
 -rw-rw-rw-  2.0 unx      711 b- defN 23-Apr-13 23:18 pingpong/context/last_window_strategy.py
 -rw-rw-rw-  2.0 unx      840 b- defN 23-Apr-12 04:54 pingpong/context/search_window_strategy.py
 -rw-rw-rw-  2.0 unx      119 b- defN 23-Apr-11 14:54 pingpong/context/strategy.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-13 23:23 bingbong-0.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     3346 b- defN 23-Apr-13 23:23 bingbong-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-13 23:23 bingbong-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-13 23:23 bingbong-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1149 b- defN 23-Apr-13 23:23 bingbong-0.1.5.dist-info/RECORD
-14 files, 20536 bytes uncompressed, 8068 bytes compressed:  60.7%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-14 05:22 bingbong-0.1.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     3346 b- defN 23-Apr-14 05:22 bingbong-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-14 05:22 bingbong-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-14 05:22 bingbong-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1225 b- defN 23-Apr-14 05:22 bingbong-0.1.6.dist-info/RECORD
+15 files, 22606 bytes uncompressed, 8876 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: pingpong/__init__.py
 Comment: 
 
 Filename: pingpong/alpaca.py
 Comment: 
 
+Filename: pingpong/dolly.py
+Comment: 
+
 Filename: pingpong/gradio.py
 Comment: 
 
 Filename: pingpong/pingpong.py
 Comment: 
 
 Filename: pingpong/context/__init__.py
@@ -21,23 +24,23 @@
 
 Filename: pingpong/context/search_window_strategy.py
 Comment: 
 
 Filename: pingpong/context/strategy.py
 Comment: 
 
-Filename: bingbong-0.1.5.dist-info/LICENSE
+Filename: bingbong-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: bingbong-0.1.5.dist-info/METADATA
+Filename: bingbong-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: bingbong-0.1.5.dist-info/WHEEL
+Filename: bingbong-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: bingbong-0.1.5.dist-info/top_level.txt
+Filename: bingbong-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: bingbong-0.1.5.dist-info/RECORD
+Filename: bingbong-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingpong/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 
 from .pingpong import PingPong
```

## pingpong/alpaca.py

```diff
@@ -11,17 +11,33 @@
 
 """
 
   @classmethod
   def prompt(cls, pingpong):
     return f"""### Instruction: {pingpong.ping}
 
-### Response: {pingpong.pong}"""
+### Response: {"" if pingpong.pong is None else pingpong.pong}"""
 
 class AlpacaChatPPManager(PPManager):
+  def add_ping(self, ping, fmt: PromptFmt=AlpacaPromptFmt):
+    allowed = super().add_ping(ping, fmt)
+
+    if allowed:
+      prompts = f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.
+
+### Instruction:
+{ping}
+{fmt.ctx(self.ctx)}
+### Response:
+"""
+      return prompts
+
+    return None
+
+
   def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=AlpacaPromptFmt):
     if to_idx == -1 or to_idx >= len(self.pingpongs):
       to_idx = len(self.pingpongs)
 
     results = fmt.ctx(self.ctx)
 
     for idx, pingpong in enumerate(self.pingpongs[from_idx:to_idx]):
```

## pingpong/pingpong.py

```diff
@@ -1,12 +1,15 @@
 class PingPong:
   def __init__(self, ping, pong):
     self.ping = ping
     self.pong = pong
 
+  def __repr__(self):
+    return f"ping: {self.ping}, pong: {self.pong}"
+
 class PromptFmt:
   @classmethod
   def ctx(cls, context):
     pass
 
   @classmethod
   def prompt(cls, pingpong):
@@ -18,14 +21,25 @@
     pass
 
 class PPManager:
   def __init__(self, ctx: str=""):
     self.ctx = ctx
     self.pingpongs = []
 
+  def add_ping(self, ping, fmt: PromptFmt):
+    if len(self.pingpongs) == 0 \
+      or (len(self.pingpongs) >= 1 and self.pingpongs[-1].pong is not None):
+      self.pingpongs.append(PingPong(ping, None))
+      return True
+    return False
+    
+
+  def add_pong(self, pong):
+    self.pingpongs[-1].pong = pong
+
   def add_pingpong(self, pingpong):
     self.pingpongs.append(pingpong)
 
   def pop_pingpong(self):
     return self.pingpongs.pop()
 
   def build_prompts(self, from_idx: int, to_idx: int, fmt: PromptFmt):
```

## Comparing `bingbong-0.1.5.dist-info/LICENSE` & `bingbong-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bingbong-0.1.5.dist-info/METADATA` & `bingbong-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1.5
+Version: 0.1.6
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `bingbong-0.1.5.dist-info/RECORD` & `bingbong-0.1.6.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-pingpong/__init__.py,sha256=cMKJbuKnaa4KVzJmLOHtB09ZdveKi_9XV7_Q8PWClJw,53
-pingpong/alpaca.py,sha256=WhlMCAalGBREDJtnafqHWq6zKr3IHzy3q9m0_5HHAEA,853
+pingpong/__init__.py,sha256=IhwGQDasqkDMSI8eymIkN8bsjcEY1dr3mAQx7OSFstU,53
+pingpong/alpaca.py,sha256=C70bD8DJh1pDt1tvuwbVUPEMaI7wEu-gBJGSrRP_Eq0,1234
+pingpong/dolly.py,sha256=6a89oTk3zH12Z6hWpEFP5ZeCZ1GdCe3DoOvR1ut9nZg,1229
 pingpong/gradio.py,sha256=PhSVAkx9YH4i8xuKuIa2pvxTtrunbPvtDltFtVFA6R4,583
-pingpong/pingpong.py,sha256=REMKK9bPR9Q_IH-DB8paxBtDlX8dwi2PrG1X7YthozA,662
+pingpong/pingpong.py,sha256=W4miUWWb0wGnFFl3sIHJpnrciMf-pbFh4da5KSBNoyQ,1046
 pingpong/context/__init__.py,sha256=ksYP7nq8inYK7SHDwpd7Hs_h87gPKdP9Ac6E5w0X6zM,173
 pingpong/context/auto_summary_strategy.py,sha256=s2lrlGKzLFNBGdLMAkaC6d2VY8aJSdgtrwa_Rvmt3Fc,589
 pingpong/context/last_window_strategy.py,sha256=37Gu94VVIMlj-pK3r7NMrOPp_XufMYsSthf5-ZJNw00,711
 pingpong/context/search_window_strategy.py,sha256=OPd2xxiI9FrzU4w2R5luaDEKiNEj4KYr_EF53Qi6l_Q,840
 pingpong/context/strategy.py,sha256=xGoy7T92gYubrwekz0Kz2Vxv10njgXG44K48bC9BqAU,119
-bingbong-0.1.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-bingbong-0.1.5.dist-info/METADATA,sha256=PwEMv6b1hPL52WSOvxi0G7V97zi6CmlVaQZgCPTrMu8,3346
-bingbong-0.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bingbong-0.1.5.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
-bingbong-0.1.5.dist-info/RECORD,,
+bingbong-0.1.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+bingbong-0.1.6.dist-info/METADATA,sha256=6fJyRJfSvB1nVIXThsY62voNiBtGk-RBfIVDTJPzNcs,3346
+bingbong-0.1.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bingbong-0.1.6.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
+bingbong-0.1.6.dist-info/RECORD,,
```

